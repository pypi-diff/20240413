# Comparing `tmp/blurry_cli-0.6.2.tar.gz` & `tmp/blurry_cli-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "blurry_cli-0.6.2.tar", max compression
+gzip compressed data, was "blurry_cli-0.7.0.tar", max compression
```

## Comparing `blurry_cli-0.6.2.tar` & `blurry_cli-0.7.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1068 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/LICENSE
--rw-r--r--   0        0        0     1782 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/README.md
--rw-r--r--   0        0        0     9576 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/__init__.py
--rw-r--r--   0        0        0       32 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/__main__.py
--rw-r--r--   0        0        0      526 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/async_typer.py
--rw-r--r--   0        0        0      872 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/cli.py
--rw-r--r--   0        0        0      111 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/constants.py
--rw-r--r--   0        0        0     3537 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/images.py
--rw-r--r--   0        0        0     7409 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/markdown/__init__.py
--rw-r--r--   0        0        0     1778 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/markdown/front_matter.py
--rw-r--r--   0        0        0        0 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/markdown/renderer_functions/__init__.py
--rw-r--r--   0        0        0      787 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/markdown/renderer_functions/render_video.py
--rw-r--r--   0        0        0     1995 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/open_graph.py
--rw-r--r--   0        0        0      273 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/plugins/__init__.py
--rw-r--r--   0        0        0        0 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/plugins/html_plugins/__init__.py
--rw-r--r--   0        0        0     1124 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/plugins/html_plugins/minify_html_plugin.py
--rw-r--r--   0        0        0        0 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/plugins/markdown_plugins/__init__.py
--rw-r--r--   0        0        0     1119 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/plugins/markdown_plugins/container_plugin.py
--rw-r--r--   0        0        0      683 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/plugins/markdown_plugins/punctuation_plugin.py
--rw-r--r--   0        0        0     1509 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/plugins/markdown_plugins/python_code_plugin.py
--rw-r--r--   0        0        0        0 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/py.typed
--rw-r--r--   0        0        0     2347 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/settings.py
--rw-r--r--   0        0        0     1620 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/sitemap.py
--rw-r--r--   0        0        0      777 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/types.py
--rw-r--r--   0        0        0     4376 2024-03-03 20:03:05.174087 blurry_cli-0.6.2/blurry/utils.py
--rw-r--r--   0        0        0     2146 2024-03-03 20:03:05.178087 blurry_cli-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     3305 1970-01-01 00:00:00.000000 blurry_cli-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/LICENSE
+-rw-r--r--   0        0        0     1782 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/README.md
+-rw-r--r--   0        0        0     9905 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/__init__.py
+-rw-r--r--   0        0        0       32 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/__main__.py
+-rw-r--r--   0        0        0      526 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/async_typer.py
+-rw-r--r--   0        0        0      872 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/cli.py
+-rw-r--r--   0        0        0      111 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/constants.py
+-rw-r--r--   0        0        0     3537 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/images.py
+-rw-r--r--   0        0        0     7427 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/markdown/__init__.py
+-rw-r--r--   0        0        0     1778 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/markdown/front_matter.py
+-rw-r--r--   0        0        0        0 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/markdown/renderer_functions/__init__.py
+-rw-r--r--   0        0        0      787 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/markdown/renderer_functions/render_video.py
+-rw-r--r--   0        0        0     1995 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/open_graph.py
+-rw-r--r--   0        0        0      273 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/plugins/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/plugins/html_plugins/__init__.py
+-rw-r--r--   0        0        0     1124 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/plugins/html_plugins/minify_html_plugin.py
+-rw-r--r--   0        0        0        0 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/plugins/markdown_plugins/__init__.py
+-rw-r--r--   0        0        0     1119 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/plugins/markdown_plugins/container_plugin.py
+-rw-r--r--   0        0        0      683 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/plugins/markdown_plugins/punctuation_plugin.py
+-rw-r--r--   0        0        0     1509 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/plugins/markdown_plugins/python_code_plugin.py
+-rw-r--r--   0        0        0        0 2024-04-13 16:52:36.607078 blurry_cli-0.7.0/blurry/py.typed
+-rw-r--r--   0        0        0     1817 2024-04-13 16:52:36.611078 blurry_cli-0.7.0/blurry/schema_validation.py
+-rw-r--r--   0        0        0     2347 2024-04-13 16:52:36.611078 blurry_cli-0.7.0/blurry/settings.py
+-rw-r--r--   0        0        0     1620 2024-04-13 16:52:36.611078 blurry_cli-0.7.0/blurry/sitemap.py
+-rw-r--r--   0        0        0      777 2024-04-13 16:52:36.611078 blurry_cli-0.7.0/blurry/types.py
+-rw-r--r--   0        0        0     4376 2024-04-13 16:52:36.611078 blurry_cli-0.7.0/blurry/utils.py
+-rw-r--r--   0        0        0     2178 2024-04-13 16:52:36.615078 blurry_cli-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3357 1970-01-01 00:00:00.000000 blurry_cli-0.7.0/PKG-INFO
```

### Comparing `blurry_cli-0.6.2/LICENSE` & `blurry_cli-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/README.md` & `blurry_cli-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/blurry/__init__.py` & `blurry_cli-0.7.0/blurry/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,26 @@
 from typing import Any
 
 from jinja2 import Environment
 from jinja2 import FileSystemLoader
 from jinja2 import select_autoescape
 from livereload import Server
 from rich import print
+from rich.console import Console
 
 from blurry.async_typer import AsyncTyper
 from blurry.cli import print_blurry_name
 from blurry.cli import print_plugin_table
 from blurry.constants import ENV_VAR_PREFIX
 from blurry.images import generate_images_for_srcset
 from blurry.markdown import convert_markdown_file_to_html
 from blurry.open_graph import open_graph_meta_tags
 from blurry.plugins import discovered_html_plugins
 from blurry.plugins import discovered_jinja_filter_plugins
+from blurry.schema_validation import validate_front_matter_as_schema
 from blurry.settings import get_build_directory
 from blurry.settings import get_content_directory
 from blurry.settings import get_templates_directory
 from blurry.settings import SETTINGS
 from blurry.settings import update_settings
 from blurry.sitemap import write_sitemap_file
 from blurry.types import DirectoryFileData
@@ -42,14 +44,16 @@
 
 
 def json_converter_with_dates(item: Any) -> None | str:
     if isinstance(item, datetime):
         return item.strftime("%Y-%M-%D")
 
 
+warning_console = Console(stderr=True, style="bold yellow")
+
 print_blurry_name()
 print_plugin_table()
 
 
 app = AsyncTyper()
 
 
@@ -143,14 +147,17 @@
             continue
         schema_variables[key] = value
 
     schema_data = json.dumps(
         format_schema_data(schema_variables),
         default=json_converter_with_dates,
     )
+
+    validate_front_matter_as_schema(file_data.path, front_matter, warning_console)
+
     schema_type_tag = f'<script type="application/ld+json">{schema_data}</script>'
 
     template_context = {
         "body": file_data.body,
         "schema_data": schema_data,
         "schema_type_tag": schema_type_tag,
         "open_graph_tags": open_graph_meta_tags(file_data.front_matter),
@@ -232,16 +239,18 @@
                 )
             )
 
     content_dir_relative = CONTENT_DIR.relative_to(Path.cwd())
     print(f"Blurring {len(markdown_tasks)} Markdown files from: {content_dir_relative}")
 
     await asyncio.gather(*markdown_tasks)
+    loop = asyncio.new_event_loop()
+    asyncio.set_event_loop(loop)
     for non_markdown_task in non_markdown_tasks:
-        await asyncio.to_thread(lambda: asyncio.run(non_markdown_task))
+        await asyncio.to_thread(lambda: loop.run_until_complete(non_markdown_task))
 
     end = datetime.now()
 
     difference = end - start
     print(f"Built site in {difference.total_seconds()} seconds")
```

### Comparing `blurry_cli-0.6.2/blurry/async_typer.py` & `blurry_cli-0.7.0/blurry/async_typer.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/blurry/cli.py` & `blurry_cli-0.7.0/blurry/cli.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/blurry/images.py` & `blurry_cli-0.7.0/blurry/images.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/blurry/markdown/__init__.py` & `blurry_cli-0.7.0/blurry/markdown/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             image_widths = get_widths_for_image_width(image_width)
 
             attributes["sizes"] = generate_sizes_string(image_widths)
             attributes["srcset"] = generate_srcset_string(src, image_widths)
             avif_srcset = generate_srcset_string(
                 src.replace(extension, "avif"), image_widths
             )
-            source_tag = '<source srcset="{}" sizes="{}" />'.format(
+            source_tag = '<source srcset="{}" sizes="{}" type="image/avif" />'.format(
                 avif_srcset, attributes["sizes"]
             )
 
         attributes_str = " ".join(
             f'{name}="{value}"' for name, value in attributes.items()
         )
```

### Comparing `blurry_cli-0.6.2/blurry/markdown/front_matter.py` & `blurry_cli-0.7.0/blurry/markdown/front_matter.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/blurry/markdown/renderer_functions/render_video.py` & `blurry_cli-0.7.0/blurry/markdown/renderer_functions/render_video.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/blurry/open_graph.py` & `blurry_cli-0.7.0/blurry/open_graph.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/blurry/plugins/html_plugins/minify_html_plugin.py` & `blurry_cli-0.7.0/blurry/plugins/html_plugins/minify_html_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/blurry/plugins/markdown_plugins/container_plugin.py` & `blurry_cli-0.7.0/blurry/plugins/markdown_plugins/container_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/blurry/plugins/markdown_plugins/punctuation_plugin.py` & `blurry_cli-0.7.0/blurry/plugins/markdown_plugins/punctuation_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/blurry/plugins/markdown_plugins/python_code_plugin.py` & `blurry_cli-0.7.0/blurry/plugins/markdown_plugins/python_code_plugin.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/blurry/settings.py` & `blurry_cli-0.7.0/blurry/settings.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/blurry/sitemap.py` & `blurry_cli-0.7.0/blurry/sitemap.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/blurry/types.py` & `blurry_cli-0.7.0/blurry/types.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/blurry/utils.py` & `blurry_cli-0.7.0/blurry/utils.py`

 * *Files identical despite different names*

### Comparing `blurry_cli-0.6.2/pyproject.toml` & `blurry_cli-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "blurry-cli"
-version = "0.6.2"
+version = "0.7.0"
 description = "A Mistune-based static site generator for Python"
 authors = ["John Franey <franey@duck.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/blurry-dev/blurry"
 keywords = ["static-site-generator", "seo", "pagespeed"]
 classifiers = [
@@ -31,21 +31,22 @@
 mistune = "^3.0.0rc5"
 python = "^3.10"
 rich = "^13.3.3"
 selectolax = "^0.3.6"
 toml = "^0.10.2"
 typer = "^0.6.1"
 htmlmin2 = "^0.1.13"
+pydantic2-schemaorg = "^0.1.1"
 
 [tool.poetry.scripts]
 blurry = 'blurry:main'
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
-nox = "^2023.4.22"
+nox = "^2024.03.02"
 pyright = "^1.1.311"
 pytest = "^6.2.2"
 pytest-cov = "^2.11.1"
 pytest-watch = "^4.2.0"
 ruff = "^0.1.5"
 
 [build-system]
```

### Comparing `blurry_cli-0.6.2/PKG-INFO` & `blurry_cli-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: blurry-cli
-Version: 0.6.2
+Version: 0.7.0
 Summary: A Mistune-based static site generator for Python
 Home-page: https://github.com/blurry-dev/blurry
 License: MIT
 Keywords: static-site-generator,seo,pagespeed
 Author: John Franey
 Author-email: franey@duck.com
 Requires-Python: >=3.10,<4.0
@@ -23,14 +23,15 @@
 Requires-Dist: Jinja2 (>=3.0.0,<4.0.0)
 Requires-Dist: PyLD (>=2.0.3,<3.0.0)
 Requires-Dist: Wand (>=0.6.6,<0.7.0)
 Requires-Dist: ffmpeg-python (>=0.2.0,<0.3.0)
 Requires-Dist: htmlmin2 (>=0.1.13,<0.2.0)
 Requires-Dist: livereload (>=2.6.3,<3.0.0)
 Requires-Dist: mistune (>=3.0.0rc5,<4.0.0)
+Requires-Dist: pydantic2-schemaorg (>=0.1.1,<0.2.0)
 Requires-Dist: rich (>=13.3.3,<14.0.0)
 Requires-Dist: selectolax (>=0.3.6,<0.4.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typer (>=0.6.1,<0.7.0)
 Project-URL: Repository, https://github.com/blurry-dev/blurry
 Description-Content-Type: text/markdown
```

