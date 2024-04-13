# Comparing `tmp/tempren-1.0.1.tar.gz` & `tmp/tempren-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tempren-1.0.1.tar", max compression
+gzip compressed data, was "tempren-1.1.0.tar", max compression
```

## Comparing `tempren-1.0.1.tar` & `tempren-1.1.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0    32473 2024-04-02 18:39:02.617130 tempren-1.0.1/LICENSE
--rw-r--r--   0        0        0     5282 2024-04-02 18:39:02.617130 tempren-1.0.1/README.md
--rw-r--r--   0        0        0     1799 2024-04-02 18:39:02.617130 tempren-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/__init__.py
--rw-r--r--   0        0        0     3807 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/adhoc.py
--rw-r--r--   0        0        0     2797 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/alias.py
--rwxr-xr-x   0        0        0    22434 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/cli.py
--rw-r--r--   0        0        0     2518 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/discovery.py
--rw-r--r--   0        0        0      431 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/evaluation.py
--rw-r--r--   0        0        0      995 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/exceptions.py
--rw-r--r--   0        0        0     3067 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/factories.py
--rw-r--r--   0        0        0     3207 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/file_filters.py
--rw-r--r--   0        0        0     1689 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/file_sorters.py
--rw-r--r--   0        0        0     6573 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/filesystem.py
--rw-r--r--   0        0        0    13693 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/pipeline.py
--rw-r--r--   0        0        0     4239 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/primitives.py
--rw-r--r--   0        0        0        0 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/__init__.py
--rw-r--r--   0        0        0     3017 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/audio.py
--rw-r--r--   0        0        0    14814 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/core.py
--rw-r--r--   0        0        0     1245 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/filesystem.py
--rw-r--r--   0        0        0     2975 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/gpx.py
--rw-r--r--   0        0        0     1835 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/hash.py
--rw-r--r--   0        0        0     5816 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/image.py
--rw-r--r--   0        0        0     6539 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/text.py
--rw-r--r--   0        0        0     3055 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/tags/video.py
--rw-r--r--   0        0        0        0 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/__init__.py
--rw-r--r--   0        0        0     3143 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/ast.py
--rw-r--r--   0        0        0     3682 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/compiler.py
--rw-r--r--   0        0        0     1182 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/exceptions.py
--rw-r--r--   0        0        0     1202 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/generators.py
--rw-r--r--   0        0        0     1064 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateLexer.g4
--rw-r--r--   0        0        0     6080 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateLexer.interp
--rw-r--r--   0        0        0    20134 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateLexer.py
--rw-r--r--   0        0        0      326 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateLexer.tokens
--rw-r--r--   0        0        0     1184 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateParser.g4
--rw-r--r--   0        0        0     4296 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateParser.interp
--rw-r--r--   0        0        0    38985 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateParser.py
--rw-r--r--   0        0        0      326 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateParser.tokens
--rw-r--r--   0        0        0     1786 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/TagTemplateParserVisitor.py
--rw-r--r--   0        0        0        0 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/__init__.py
--rwxr-xr-x   0        0        0      261 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/generate.sh
--rwxr-xr-x   0        0        0      266 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/grammar/generate_for_grun.sh
--rw-r--r--   0        0        0     8213 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/parser.py
--rw-r--r--   0        0        0     6740 2024-04-02 18:39:02.617130 tempren-1.0.1/tempren/template/registry.py
--rw-r--r--   0        0        0     6971 1970-01-01 00:00:00.000000 tempren-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0    32473 2024-04-13 10:56:30.400575 tempren-1.1.0/LICENSE
+-rw-r--r--   0        0        0     5283 2024-04-13 10:56:30.400575 tempren-1.1.0/README.md
+-rw-r--r--   0        0        0     1817 2024-04-13 10:56:30.400575 tempren-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/__init__.py
+-rw-r--r--   0        0        0     3807 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/adhoc.py
+-rw-r--r--   0        0        0     2797 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/alias.py
+-rwxr-xr-x   0        0        0    22996 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/cli.py
+-rw-r--r--   0        0        0     2518 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/discovery.py
+-rw-r--r--   0        0        0      431 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/evaluation.py
+-rw-r--r--   0        0        0      995 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/exceptions.py
+-rw-r--r--   0        0        0     3067 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/factories.py
+-rw-r--r--   0        0        0     3207 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/file_filters.py
+-rw-r--r--   0        0        0     1879 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/file_sorters.py
+-rw-r--r--   0        0        0     7300 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/filesystem.py
+-rw-r--r--   0        0        0    14729 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/pipeline.py
+-rw-r--r--   0        0        0     4239 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/primitives.py
+-rw-r--r--   0        0        0        0 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/tags/__init__.py
+-rw-r--r--   0        0        0     3017 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/tags/audio.py
+-rw-r--r--   0        0        0    14814 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/tags/core.py
+-rw-r--r--   0        0        0     1864 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/tags/filesystem.py
+-rw-r--r--   0        0        0     2975 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/tags/gpx.py
+-rw-r--r--   0        0        0     1835 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/tags/hash.py
+-rw-r--r--   0        0        0     5816 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/tags/image.py
+-rw-r--r--   0        0        0     6539 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/tags/text.py
+-rw-r--r--   0        0        0     3055 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/tags/video.py
+-rw-r--r--   0        0        0        0 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/__init__.py
+-rw-r--r--   0        0        0     3143 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/ast.py
+-rw-r--r--   0        0        0     3682 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/compiler.py
+-rw-r--r--   0        0        0     1182 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/exceptions.py
+-rw-r--r--   0        0        0     1202 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/generators.py
+-rw-r--r--   0        0        0     1064 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/grammar/TagTemplateLexer.g4
+-rw-r--r--   0        0        0     6080 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/grammar/TagTemplateLexer.interp
+-rw-r--r--   0        0        0    20134 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/grammar/TagTemplateLexer.py
+-rw-r--r--   0        0        0      326 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/grammar/TagTemplateLexer.tokens
+-rw-r--r--   0        0        0     1184 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/grammar/TagTemplateParser.g4
+-rw-r--r--   0        0        0     4296 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/grammar/TagTemplateParser.interp
+-rw-r--r--   0        0        0    38985 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/grammar/TagTemplateParser.py
+-rw-r--r--   0        0        0      326 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/grammar/TagTemplateParser.tokens
+-rw-r--r--   0        0        0     1786 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/grammar/TagTemplateParserVisitor.py
+-rw-r--r--   0        0        0        0 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/grammar/__init__.py
+-rwxr-xr-x   0        0        0      261 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/grammar/generate.sh
+-rwxr-xr-x   0        0        0      266 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/grammar/generate_for_grun.sh
+-rw-r--r--   0        0        0     8213 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/parser.py
+-rw-r--r--   0        0        0     6535 2024-04-13 10:56:30.400575 tempren-1.1.0/tempren/template/registry.py
+-rw-r--r--   0        0        0     6972 1970-01-01 00:00:00.000000 tempren-1.1.0/PKG-INFO
```

### Comparing `tempren-1.0.1/LICENSE` & `tempren-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/README.md` & `tempren-1.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
 ```
 </details>
 
 <details>
 <summary>Sorting files into directories based on their MIME type</summary>
 
 ```commandline
-$ tempren -d --path "%Capitalize(){%Mime(subtype)}/%Name()" ~/Downloads
+$ tempren -dr --path "%Capitalize(){%Mime(subtype)}/%Name()" ~/Downloads
 Renamed: dotnet-install.sh
      to: X-shellscript/dotnet-install.sh
 Renamed: openrgb_0.7_amd64_buster_6128731.deb
      to: Vnd.debian.binary-package/openrgb_0.7_amd64_buster_6128731.deb
 Renamed: prometheus-2.26.0.linux-amd64.tar.gz
      to: Gzip/prometheus-2.26.0.linux-amd64.tar.gz
 Renamed: nldb remote.zip
```

### Comparing `tempren-1.0.1/pyproject.toml` & `tempren-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tempren"
-version = "1.0.1"
+version = "1.1.0"
 description = "Template-based renaming utility"
 readme = "README.md"
 license = "GPL-3.0-or-later"
 authors = ["Paweł Żukowski <p.z.idlecode@gmail.com>"]
 homepage = "https://github.com/idle-code/tempren"
 keywords = ["batch-renaming", "cli", "filename"]
 classifiers = [
@@ -39,14 +39,15 @@
 [tool.poetry.dev-dependencies]
 pytest = "^7.4.4"
 pytest-cov = "^4.1"
 coverage = "^7.2.7"
 pre-commit = "^3.5"
 mypy = "^1.4.1"
 pylint = "^3.0.2"
+black = "^24.4.0"
 
 [tool.poetry.extras]
 video = ["pymediainfo"]
 
 [tool.poetry.scripts]
 tempren = "tempren.cli:throwing_main"
```

### Comparing `tempren-1.0.1/tempren/adhoc.py` & `tempren-1.1.0/tempren/adhoc.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/alias.py` & `tempren-1.1.0/tempren/alias.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/cli.py` & `tempren-1.1.0/tempren/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 from tempren.exceptions import FileNotSupportedError, TemplateEvaluationError
 from tempren.filesystem import DestinationAlreadyExistsError
 from tempren.primitives import CategoryName, QualifiedTagName, TagName
 from tempren.template.exceptions import TagError, TemplateError
 
 from .pipeline import (
+    ConfigurationError,
     ConflictResolutionStrategy,
     FilterType,
     InvalidDestinationError,
     OperationMode,
     RuntimeConfiguration,
     build_pipeline,
     build_tag_registry,
@@ -130,14 +131,15 @@
     if not adhoc_tags:
         return dict()
     list_of_tuples = list(chain(*adhoc_tags))
     names = list(map(lambda pair: pair[0], list_of_tuples))
     unique_names = set(names)
     if len(names) > len(unique_names):
         repeating_names = [name for name in unique_names if names.count(name) > 1]
+        # TODO: Test
         for duplicate_name in repeating_names:
             executables_with_the_same_name = list(
                 map(
                     lambda pair: str(pair[1]),
                     filter(lambda pair: pair[0] == duplicate_name, list_of_tuples),
                 )
             )
@@ -155,14 +157,16 @@
     if not aliases:
         return dict()
     list_of_tuples = list(chain(*aliases))
     names = list(map(lambda pair: pair[0], list_of_tuples))
     unique_names = set(names)
     if len(names) > len(unique_names):
         repeating_names = [name for name in unique_names if names.count(name) > 1]
+        # TODO: Test
+        # TODO: Refactor - the same code is found in validate_adhoc_tags
         for duplicate_name in repeating_names:
             patterns_with_the_same_name = list(
                 map(
                     lambda pair: str(pair[1]),
                     filter(lambda pair: pair[0] == duplicate_name, list_of_tuples),
                 )
             )
@@ -171,15 +175,15 @@
                 ErrorCode.USAGE_ERROR,
                 f"Aliases for patterns {' and '.join(patterns_with_the_same_name)} cannot have the same name {duplicate_name}",
             )
 
     return dict(list_of_tuples)
 
 
-class SystemExitError(Exception):
+class SystemExitError(Exception):  # TODO: Use ConfigurationError instead
     status: int
 
     def __init__(self, status: int, message: Optional[str]):
         super().__init__(message)
         self.status = status
 
 
@@ -196,17 +200,18 @@
         )
         log.info("Available tags:")
         for category_name in sorted(registry.category_map.keys()):
             log.info(f"{category_name.capitalize()}:")
             category = registry.category_map[category_name]
 
             all_category_tags = sorted(category.tag_map.items())
-            if not all_category_tags:
+            if (
+                not all_category_tags
+            ):  # NOCOVER: Empty categories should not be present in the registry
                 # There is no tags in the category
-                # TODO: Empty categories should not be present in the registry
                 continue
             max_name_length = max(
                 [len(tag_name) for tag_name, factory in all_category_tags]
             )
             log.debug(
                 "Longest tag name: %d in category %s", max_name_length, category_name
             )
@@ -241,15 +246,16 @@
                     )
                 else:
                     qualified_name = QualifiedTagName(TagName(raw_tag_name))
 
                 tag_factory = registry.get_tag_factory(qualified_name)
             except TagError as tag_error:
                 parser.exit(ErrorCode.USAGE_ERROR, str(tag_error))
-                raise
+                # noinspection PyUnreachableCode
+                raise  # NOCOVER: required by mypy
             log.info("")
             log.info(indent(tag_factory.configuration_signature, "  "))
             log.info("")
             log.info(tag_factory.short_description)
             if tag_factory.long_description:
                 log.info("")
                 log.info(tag_factory.long_description)
@@ -310,27 +316,26 @@
 
     def _get_help_string(self, action):
         if action.default:
             return "(default) " + action.help
         return action.help
 
 
-# CHECK: use pydantic-cli for argument parsing
 def process_cli_configuration(argv: List[str]) -> RuntimeConfiguration:
     log.debug("Parsing command line arguments")
     parser = argparse.ArgumentParser(
         prog="tempren",
         description="Template-based renaming utility",
         fromfile_prefix_chars="@",
         add_help=False,
         formatter_class=DefaultOptionsHelpFormatter,
     )
 
     parser.add_argument(
-        "-d",
+        "-dr",
         "--dry-run",
         action="store_true",
         help="Do not perform any renaming - just show expected operation results",
     )
     parser.add_argument(
         "-r",
         "--recursive",
@@ -381,53 +386,33 @@
     operation_mode.add_argument(
         "-n",
         "--name",
         action="store_const",
         dest="mode",
         const=OperationMode.name,
         default=OperationMode.name,
-        help="Use template to generate file name",
+        help="Use template to generate file name only",
+    )
+    operation_mode.add_argument(
+        "-d",
+        "--directory",
+        action="store_const",
+        dest="mode",
+        const=OperationMode.directory,
+        help="Use template to generate directory names only",
     )
     operation_mode.add_argument(
         "-p",
         "--path",
         action="store_const",
         dest="mode",
         const=OperationMode.path,
         help="Use template to generate relative file path",
     )
 
-    conflict_resolution_group = parser.add_argument_group("conflict resolution")
-    conflict_resolution = conflict_resolution_group.add_mutually_exclusive_group()
-    conflict_resolution.add_argument(
-        "-cs",
-        "--conflict-stop",
-        action="store_true",
-        default=True,
-        help="Keep source file name intact and stop",
-    )
-    conflict_resolution.add_argument(
-        "-ci",
-        "--conflict-ignore",
-        action="store_true",
-        help="Keep source file name intact and continue",
-    )
-    conflict_resolution.add_argument(
-        "-co",
-        "--conflict-override",
-        action="store_true",
-        help="Override destination file",
-    )
-    conflict_resolution.add_argument(
-        "-cm",
-        "--conflict-manual",
-        action="store_true",
-        help="Prompt user to resolve conflict manually (choose an option or provide new filename)",
-    )
-
     filtering_group = parser.add_argument_group("filtering")
     filter_mode = filtering_group.add_mutually_exclusive_group()
     filter_mode.add_argument(
         "-fg",
         "--filter-glob",
         type=str,
         metavar="filter_expression",
@@ -465,14 +450,42 @@
     sorting_group.add_argument(
         "-si",
         "--sort-invert",
         action="store_true",
         help="Reverse sorting order",
     )
 
+    conflict_resolution_group = parser.add_argument_group("conflict resolution")
+    conflict_resolution = conflict_resolution_group.add_mutually_exclusive_group()
+    conflict_resolution.add_argument(
+        "-cs",
+        "--conflict-stop",
+        action="store_true",
+        default=True,
+        help="Keep source file name intact and stop",
+    )
+    conflict_resolution.add_argument(
+        "-ci",
+        "--conflict-ignore",
+        action="store_true",
+        help="Keep source file name intact and continue",
+    )
+    conflict_resolution.add_argument(
+        "-co",
+        "--conflict-override",
+        action="store_true",
+        help="Override destination file",
+    )
+    conflict_resolution.add_argument(
+        "-cm",
+        "--conflict-manual",
+        action="store_true",
+        help="Prompt user to resolve conflict manually (choose an option or provide new filename)",
+    )
+
     parser.add_argument(
         "template",
         type=nonempty_string,
         help="Template used to generate new filename/path",
     )
     parser.add_argument(
         "path",
@@ -646,14 +659,17 @@
         log.info("Done")
         return ErrorCode.SUCCESS
     # TODO: Clean up exception hierarchy
     except SystemExitError as exc:
         if exc.status != 0:
             log.error(exc)
         return exc.status
+    except ConfigurationError as exc:
+        log.error(exc)
+        return ErrorCode.USAGE_ERROR
     except TemplateEvaluationError as template_evaluation_error:
         render_template_evaluation_error(template_evaluation_error)
         return ErrorCode.TEMPLATE_EVALUATION_ERROR
     except TemplateError as template_error:
         render_template_error(template_error)
         return ErrorCode.TEMPLATE_SYNTAX_ERROR
     except DestinationAlreadyExistsError as exc:
```

### Comparing `tempren-1.0.1/tempren/discovery.py` & `tempren-1.1.0/tempren/discovery.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/exceptions.py` & `tempren-1.1.0/tempren/exceptions.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/factories.py` & `tempren-1.1.0/tempren/factories.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/file_filters.py` & `tempren-1.1.0/tempren/file_filters.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/file_sorters.py` & `tempren-1.1.0/tempren/file_sorters.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,7 +39,12 @@
             assert self.pattern.source_representation is not None
             raise TemplateEvaluationError(
                 file,
                 self.pattern.source_representation,
                 evaluation_error.expression,
                 evaluation_error.message,
             )
+
+
+class PathDepthSorter(FileSorter):
+    def __call__(self, files: Iterable[File]) -> Iterable[File]:
+        return sorted(files, key=lambda f: (len(f.relative_path.parts),), reverse=True)
```

### Comparing `tempren-1.0.1/tempren/filesystem.py` & `tempren-1.1.0/tempren/filesystem.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,14 +84,34 @@
                 yield from self._gather_in(dir_entry)
             else:
                 yield File(
                     self._start_directory, dir_entry.relative_to(self._start_directory)
                 )
 
 
+class RecursiveDirectoryGatherer(FilesystemGatherer):
+    def __init__(self, start_directory: Path):
+        self._start_directory = start_directory.absolute()
+
+    def gather_files(self) -> Iterable[File]:
+        yield from self._gather_in(self._start_directory)
+
+    def _gather_in(self, directory: Path) -> Iterable[File]:
+        print(f"Gathering in {directory}")
+        for dir_entry in directory.iterdir():
+            if not self._include_path_in_result(dir_entry):
+                continue
+
+            if dir_entry.is_dir():
+                yield File(
+                    self._start_directory, dir_entry.relative_to(self._start_directory)
+                )
+                yield from self._gather_in(dir_entry)
+
+
 class ExplicitFileGatherer(FileGatherer):
     def __init__(self, files: List[Path]):
         self._files_to_provide = files
 
     def gather_files(self) -> Iterable[File]:
         for file in self._files_to_provide:
             yield File(file.parent.absolute(), Path(file.name))
```

### Comparing `tempren-1.0.1/tempren/pipeline.py` & `tempren-1.1.0/tempren/pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,28 @@
     FileFilterInverter,
     GlobFilenameFileFilter,
     GlobPathFileFilter,
     RegexFilenameFileFilter,
     RegexPathFileFilter,
     TemplateFileFilter,
 )
-from tempren.file_sorters import TemplateFileSorter
+from tempren.file_sorters import PathDepthSorter, TemplateFileSorter
 from tempren.filesystem import (
     CombinedFileGatherer,
     DestinationAlreadyExistsError,
     DryRunRenamer,
     ExplicitFileGatherer,
     FileGatherer,
     FileMover,
     FileRenamer,
     FileRenamerType,
     FlatFileGatherer,
     InvalidDestinationError,
     PrintingRenamerWrapper,
+    RecursiveDirectoryGatherer,
     RecursiveFileGatherer,
 )
 from tempren.primitives import CategoryName, File, PathGenerator, Pattern, TagName
 from tempren.template.compiler import TemplateCompiler
 from tempren.template.exceptions import InvalidFilenameError, TemplateError
 from tempren.template.generators import TemplateNameGenerator, TemplatePathGenerator
 from tempren.template.registry import TagRegistry
@@ -44,14 +45,15 @@
     regex = "regex"
     glob = "glob"
 
 
 class OperationMode(Enum):
     name = "name"
     path = "path"
+    directory = "directory"
 
 
 # TODO: Find a way to keep documentation close to the enum values and use it in argparser/generated help
 class ConflictResolutionStrategy(Enum):
     stop = "stop"
     """Stop renaming and show an error"""
 
@@ -156,15 +158,15 @@
                     "Error generated when renaming %r: %r",
                     file,
                     error,
                 )
                 raise
 
             if new_relative_path == file.relative_path:
-                self.log.info(
+                self.log.debug(
                     "Skipping renaming of: '%s' (source and destination are the same)",
                     new_relative_path,
                 )
                 continue
 
             new_absolute_path = (file.input_directory / new_relative_path).resolve()
             if not str(new_absolute_path).startswith(str(file.input_directory)):
@@ -279,80 +281,98 @@
     registry: TagRegistry,
     manual_conflict_resolver: ManualConflictResolver,  # TODO: Move to the RuntimeConfiguration
 ) -> Pipeline:
     log.debug("Building pipeline")
     pipeline = Pipeline()
 
     file_gatherers: List[FileGatherer] = []
+
     input_directories = filter(lambda p: p.is_dir(), config.input_paths)
-    for directory in input_directories:
+    input_files = list(filter(lambda p: p.is_file(), config.input_paths))
+    if config.mode == OperationMode.directory:
+        if any(input_files):
+            log.warning("Ignoring file paths provided in directory mode")
+
         if config.recursive:
-            file_gatherers.append(RecursiveFileGatherer(directory))
+            for directory in input_directories:
+                file_gatherers.append(RecursiveDirectoryGatherer(directory))
         else:
-            file_gatherers.append(FlatFileGatherer(directory))
+            file_gatherers.append(ExplicitFileGatherer(input_directories))
+    else:
+        for directory in input_directories:
+            if config.recursive:
+                file_gatherers.append(RecursiveFileGatherer(directory))
+            else:
+                file_gatherers.append(FlatFileGatherer(directory))
+
+        if any(input_files):
+            file_gatherers.append(ExplicitFileGatherer(input_files))
 
-    input_files = list(filter(lambda p: p.is_file(), config.input_paths))
-    if any(input_files):
-        file_gatherers.append(ExplicitFileGatherer(input_files))
     pipeline.file_gatherer = CombinedFileGatherer(file_gatherers)
     pipeline.file_gatherer.include_hidden = config.include_hidden
 
     compiler = TemplateCompiler(registry)
 
     def _compile_template(template_text: str) -> Pattern:
         try:
             return compiler.compile(template_text)
         except TemplateError as template_error:
             template_error.template = template_text
             raise template_error
 
     bound_pattern = _compile_template(config.template)
 
-    if config.mode == OperationMode.name:
+    if config.mode == OperationMode.name or config.mode == OperationMode.directory:
         pipeline.path_generator = TemplateNameGenerator(bound_pattern)
         if config.filter:
             if config.filter_type == FilterType.regex:
                 pipeline.file_filter = RegexFilenameFileFilter(config.filter)
             elif config.filter_type == FilterType.glob:
                 pipeline.file_filter = GlobFilenameFileFilter(config.filter)
             elif config.filter_type == FilterType.template:
                 bound_filter_pattern = _compile_template(config.filter)
                 pipeline.file_filter = TemplateFileFilter(bound_filter_pattern)
             else:
-                raise NotImplementedError("Unknown filter type")
+                raise NotImplementedError("Unknown filter type: " + str(config.filter))
     elif config.mode == OperationMode.path:
         pipeline.path_generator = TemplatePathGenerator(bound_pattern)
         if config.filter:
             if config.filter_type == FilterType.regex:
                 pipeline.file_filter = RegexPathFileFilter(config.filter)
             elif config.filter_type == FilterType.glob:
                 pipeline.file_filter = GlobPathFileFilter(config.filter)
             elif config.filter_type == FilterType.template:
                 bound_filter_pattern = _compile_template(config.filter)
                 pipeline.file_filter = TemplateFileFilter(bound_filter_pattern)
             else:
-                raise NotImplementedError("Unknown filter type")
+                raise NotImplementedError("Unknown filter type: " + str(config.filter))
     else:
-        raise NotImplementedError("Unknown operation mode")
+        raise NotImplementedError("Unknown operation mode: " + str(config.mode))
 
     if config.filter_invert and config.filter is not None:
         pipeline.file_filter = FileFilterInverter(pipeline.file_filter)
 
-    if config.sort:
+    if config.mode == OperationMode.directory:
+        # FIXME: This workaround allows us to mitigate conflicts arising from
+        #        trying to rename child directories after their parent has been renamed
+        if config.sort:
+            raise ConfigurationError("Sorting is not available in directory mode")
+        pipeline.sorter = PathDepthSorter()
+    elif config.sort:
         bound_sorter_pattern = _compile_template(config.sort)
         pipeline.sorter = TemplateFileSorter(bound_sorter_pattern, config.sort_invert)
 
     pipeline.conflict_strategy = config.conflict_strategy
     pipeline.manual_conflict_resolver = manual_conflict_resolver
 
     if config.dry_run:
         pipeline.renamer = DryRunRenamer()
-        # FIXME: Use DryRunMover for path mode?
+        # FIXME: Use custom DryRunMover for path mode?
     else:
-        if config.mode == OperationMode.name:
+        if config.mode == OperationMode.name or config.mode == OperationMode.directory:
             pipeline.renamer = FileRenamer()
         elif config.mode == OperationMode.path:
             pipeline.renamer = FileMover()
         else:
             raise NotImplementedError("Unknown operation mode")
 
     pipeline.renamer = PrintingRenamerWrapper(pipeline.renamer)  # type: ignore
```

### Comparing `tempren-1.0.1/tempren/primitives.py` & `tempren-1.1.0/tempren/primitives.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/tags/audio.py` & `tempren-1.1.0/tempren/tags/audio.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/tags/core.py` & `tempren-1.1.0/tempren/tags/core.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/tags/gpx.py` & `tempren-1.1.0/tempren/tags/gpx.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/tags/hash.py` & `tempren-1.1.0/tempren/tags/hash.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/tags/image.py` & `tempren-1.1.0/tempren/tags/image.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/tags/text.py` & `tempren-1.1.0/tempren/tags/text.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/tags/video.py` & `tempren-1.1.0/tempren/tags/video.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/template/ast.py` & `tempren-1.1.0/tempren/template/ast.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/template/compiler.py` & `tempren-1.1.0/tempren/template/compiler.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/template/exceptions.py` & `tempren-1.1.0/tempren/template/exceptions.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/template/generators.py` & `tempren-1.1.0/tempren/template/generators.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/template/grammar/TagTemplateLexer.g4` & `tempren-1.1.0/tempren/template/grammar/TagTemplateLexer.g4`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/template/grammar/TagTemplateLexer.interp` & `tempren-1.1.0/tempren/template/grammar/TagTemplateLexer.interp`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/template/grammar/TagTemplateLexer.py` & `tempren-1.1.0/tempren/template/grammar/TagTemplateLexer.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/template/grammar/TagTemplateParser.g4` & `tempren-1.1.0/tempren/template/grammar/TagTemplateParser.g4`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/template/grammar/TagTemplateParser.interp` & `tempren-1.1.0/tempren/template/grammar/TagTemplateParser.interp`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/template/grammar/TagTemplateParser.py` & `tempren-1.1.0/tempren/template/grammar/TagTemplateParser.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/template/grammar/TagTemplateParserVisitor.py` & `tempren-1.1.0/tempren/template/grammar/TagTemplateParserVisitor.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/template/parser.py` & `tempren-1.1.0/tempren/template/parser.py`

 * *Files identical despite different names*

### Comparing `tempren-1.0.1/tempren/template/registry.py` & `tempren-1.1.0/tempren/template/registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,16 +58,14 @@
         self.register_tag_factory(executable_tag_factory, tag_name)
 
     def register_tag_factory(
         self, tag_factory: TagFactory, tag_name: Optional[TagName] = None
     ):
         if tag_name is None:
             tag_name = tag_factory.tag_name
-        if not tag_name:
-            raise ValueError(f"Invalid tag name '{repr(tag_name)}'")
         if tag_name in self.tag_map:
             raise ValueError(f"Factory for tag '{tag_name}' already registered")
         self.tag_map[tag_name] = tag_factory
 
     def find_tag_factory(self, tag_name: TagName) -> Optional[TagFactory]:
         return self.tag_map.get(tag_name, None)
 
@@ -76,18 +74,14 @@
     log: Logger
     category_map: Dict[CategoryName, TagCategory]
 
     def __init__(self):
         self.log = logging.getLogger(self.__class__.__name__)
         self.category_map = {}
 
-    @property
-    def categories(self) -> List[CategoryName]:
-        return sorted(self.category_map.keys())
-
     def find_category(self, category_name: CategoryName) -> Optional[TagCategory]:
         category = self.category_map.get(category_name, None)
         if category:
             return category
         category_name = CategoryName(category_name.lower())
         return self.category_map.get(category_name, None)
```

### Comparing `tempren-1.0.1/PKG-INFO` & `tempren-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tempren
-Version: 1.0.1
+Version: 1.1.0
 Summary: Template-based renaming utility
 Home-page: https://github.com/idle-code/tempren
 License: GPL-3.0-or-later
 Keywords: batch-renaming,cli,filename
 Author: Paweł Żukowski
 Author-email: p.z.idlecode@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -115,15 +115,15 @@
 ```
 </details>
 
 <details>
 <summary>Sorting files into directories based on their MIME type</summary>
 
 ```commandline
-$ tempren -d --path "%Capitalize(){%Mime(subtype)}/%Name()" ~/Downloads
+$ tempren -dr --path "%Capitalize(){%Mime(subtype)}/%Name()" ~/Downloads
 Renamed: dotnet-install.sh
      to: X-shellscript/dotnet-install.sh
 Renamed: openrgb_0.7_amd64_buster_6128731.deb
      to: Vnd.debian.binary-package/openrgb_0.7_amd64_buster_6128731.deb
 Renamed: prometheus-2.26.0.linux-amd64.tar.gz
      to: Gzip/prometheus-2.26.0.linux-amd64.tar.gz
 Renamed: nldb remote.zip
```

