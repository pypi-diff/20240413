# Comparing `tmp/panpdf-0.1.6.tar.gz` & `tmp/panpdf-0.1.7.tar.gz`

## Comparing `panpdf-0.1.6.tar` & `panpdf-0.1.7.tar`

### file list

```diff
@@ -1,67 +1,68 @@
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 panpdf-0.1.6/.gitattributes
--rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 panpdf-0.1.6/mkdocs.yml
--rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 panpdf-0.1.6/ruff_defaults.toml
--rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 panpdf-0.1.6/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 panpdf-0.1.6/.devcontainer/postCreate.sh
--rw-r--r--   0        0        0   118258 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/a.pdf
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/defaults.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/include-after-body.tex
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/include-before-body.tex
--rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/include-in-header.tex
--rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/images/figure.pdf
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/images/figure.tex
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/images/header.pdf
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/images/header.tex
--rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/src/1.md
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 panpdf-0.1.6/examples/src/2.md
--rw-r--r--   0        0        0    37281 2020-02-02 00:00:00.000000 panpdf-0.1.6/notebooks/pdf.ipynb
--rw-r--r--   0        0        0    60992 2020-02-02 00:00:00.000000 panpdf-0.1.6/notebooks/pgf.ipynb
--rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 panpdf-0.1.6/notebooks/png.ipynb
--rw-r--r--   0        0        0    55134 2020-02-02 00:00:00.000000 panpdf-0.1.6/notebooks/svg.ipynb
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/__init__.py
--rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/formatters.py
--rw-r--r--   0        0        0     8776 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/main.py
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/stores.py
--rw-r--r--   0        0        0     9600 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/__init__.py
--rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/attribute.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/crossref.py
--rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/filter.py
--rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/jupyter.py
--rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/layout.py
--rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/verbatim.py
--rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 panpdf-0.1.6/src/panpdf/filters/zotero.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/__init__.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/conftest.py
--rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/test_converters.py
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/test_formatters.py
--rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/test_main.py
--rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/test_stores.py
--rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/test_tools.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/conftest.py
--rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/test_attribute.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/test_crossref.py
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/test_filter.py
--rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/test_jupyter.py
--rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/test_layout.py
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/test_verbatim.py
--rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/filters/test_zotero.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/__init__.py
--rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/test_nbformat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/__init__.py
--rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_cite.py
--rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_code.py
--rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_figure.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_math.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_metadata.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_raw.py
--rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_section.py
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_table.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 panpdf-0.1.6/tests/libraries/panflute/test_tex.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 panpdf-0.1.6/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 panpdf-0.1.6/LICENSE.txt
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 panpdf-0.1.6/README.md
--rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 panpdf-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 panpdf-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 panpdf-0.1.7/.gitattributes
+-rw-r--r--   0        0        0     1126 2020-02-02 00:00:00.000000 panpdf-0.1.7/mkdocs.yml
+-rw-r--r--   0        0        0     6064 2020-02-02 00:00:00.000000 panpdf-0.1.7/ruff_defaults.toml
+-rw-r--r--   0        0        0      926 2020-02-02 00:00:00.000000 panpdf-0.1.7/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 panpdf-0.1.7/.devcontainer/postCreate.sh
+-rw-r--r--   0        0        0      604 2020-02-02 00:00:00.000000 panpdf-0.1.7/.devcontainer/starship.toml
+-rw-r--r--   0        0        0   118258 2020-02-02 00:00:00.000000 panpdf-0.1.7/examples/a.pdf
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 panpdf-0.1.7/examples/defaults.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.7/examples/include-after-body.tex
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.7/examples/include-before-body.tex
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 panpdf-0.1.7/examples/include-in-header.tex
+-rw-r--r--   0        0        0     3126 2020-02-02 00:00:00.000000 panpdf-0.1.7/examples/images/figure.pdf
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.1.7/examples/images/figure.tex
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 panpdf-0.1.7/examples/images/header.pdf
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 panpdf-0.1.7/examples/images/header.tex
+-rw-r--r--   0        0        0      545 2020-02-02 00:00:00.000000 panpdf-0.1.7/examples/src/1.md
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 panpdf-0.1.7/examples/src/2.md
+-rw-r--r--   0        0        0    37281 2020-02-02 00:00:00.000000 panpdf-0.1.7/notebooks/pdf.ipynb
+-rw-r--r--   0        0        0    60992 2020-02-02 00:00:00.000000 panpdf-0.1.7/notebooks/pgf.ipynb
+-rw-r--r--   0        0        0    29602 2020-02-02 00:00:00.000000 panpdf-0.1.7/notebooks/png.ipynb
+-rw-r--r--   0        0        0    55134 2020-02-02 00:00:00.000000 panpdf-0.1.7/notebooks/svg.ipynb
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 panpdf-0.1.7/src/panpdf/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.7/src/panpdf/__init__.py
+-rw-r--r--   0        0        0     1884 2020-02-02 00:00:00.000000 panpdf-0.1.7/src/panpdf/formatters.py
+-rw-r--r--   0        0        0     8776 2020-02-02 00:00:00.000000 panpdf-0.1.7/src/panpdf/main.py
+-rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 panpdf-0.1.7/src/panpdf/stores.py
+-rw-r--r--   0        0        0     9654 2020-02-02 00:00:00.000000 panpdf-0.1.7/src/panpdf/tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.7/src/panpdf/filters/__init__.py
+-rw-r--r--   0        0        0     4518 2020-02-02 00:00:00.000000 panpdf-0.1.7/src/panpdf/filters/attribute.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.1.7/src/panpdf/filters/crossref.py
+-rw-r--r--   0        0        0     1246 2020-02-02 00:00:00.000000 panpdf-0.1.7/src/panpdf/filters/filter.py
+-rw-r--r--   0        0        0     5085 2020-02-02 00:00:00.000000 panpdf-0.1.7/src/panpdf/filters/jupyter.py
+-rw-r--r--   0        0        0     4335 2020-02-02 00:00:00.000000 panpdf-0.1.7/src/panpdf/filters/layout.py
+-rw-r--r--   0        0        0     2996 2020-02-02 00:00:00.000000 panpdf-0.1.7/src/panpdf/filters/verbatim.py
+-rw-r--r--   0        0        0     3997 2020-02-02 00:00:00.000000 panpdf-0.1.7/src/panpdf/filters/zotero.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/__init__.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/conftest.py
+-rw-r--r--   0        0        0     1947 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/test_converters.py
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/test_formatters.py
+-rw-r--r--   0        0        0     4473 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/test_main.py
+-rw-r--r--   0        0        0     3238 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/test_stores.py
+-rw-r--r--   0        0        0     8284 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/test_tools.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/filters/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/filters/conftest.py
+-rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/filters/test_attribute.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/filters/test_crossref.py
+-rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/filters/test_filter.py
+-rw-r--r--   0        0        0     4798 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/filters/test_jupyter.py
+-rw-r--r--   0        0        0     4712 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/filters/test_layout.py
+-rw-r--r--   0        0        0     2607 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/filters/test_verbatim.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/filters/test_zotero.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/libraries/__init__.py
+-rw-r--r--   0        0        0      622 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/libraries/test_nbformat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/libraries/panflute/__init__.py
+-rw-r--r--   0        0        0      640 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/libraries/panflute/test_cite.py
+-rw-r--r--   0        0        0     1379 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/libraries/panflute/test_code.py
+-rw-r--r--   0        0        0     6171 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/libraries/panflute/test_figure.py
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/libraries/panflute/test_math.py
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/libraries/panflute/test_metadata.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/libraries/panflute/test_raw.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/libraries/panflute/test_section.py
+-rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/libraries/panflute/test_table.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 panpdf-0.1.7/tests/libraries/panflute/test_tex.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 panpdf-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 panpdf-0.1.7/LICENSE.txt
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 panpdf-0.1.7/README.md
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 panpdf-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 panpdf-0.1.7/PKG-INFO
```

### Comparing `panpdf-0.1.6/mkdocs.yml` & `panpdf-0.1.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/ruff_defaults.toml` & `panpdf-0.1.7/ruff_defaults.toml`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/.devcontainer/devcontainer.json` & `panpdf-0.1.7/.devcontainer/devcontainer.json`

 * *Files 23% similar despite different names*

```diff
@@ -2,79 +2,57 @@
 00000010: 7064 6622 2c0a 2020 2269 6d61 6765 223a  pdf",.  "image":
 00000020: 2022 7465 786c 6976 652f 7465 786c 6976   "texlive/texliv
 00000030: 6522 2c0a 2020 2266 6561 7475 7265 7322  e",.  "features"
 00000040: 3a20 7b0a 2020 2020 2267 6863 722e 696f  : {.    "ghcr.io
 00000050: 2f64 6576 636f 6e74 6169 6e65 7273 2f66  /devcontainers/f
 00000060: 6561 7475 7265 732f 636f 6d6d 6f6e 2d75  eatures/common-u
 00000070: 7469 6c73 3a32 223a 207b 0a20 2020 2020  tils:2": {.     
-00000080: 2022 636f 6e66 6967 7572 655a 7368 4173   "configureZshAs
-00000090: 4465 6661 756c 7453 6865 6c6c 223a 2022  DefaultShell": "
-000000a0: 7472 7565 222c 0a20 2020 2020 2022 7573  true",.      "us
-000000b0: 6572 6e61 6d65 223a 2022 7061 6e70 6466  ername": "panpdf
-000000c0: 220a 2020 2020 7d2c 0a20 2020 2022 6768  ".    },.    "gh
-000000d0: 6372 2e69 6f2f 6465 7663 6f6e 7461 696e  cr.io/devcontain
-000000e0: 6572 732d 636f 6e74 7269 622f 6665 6174  ers-contrib/feat
-000000f0: 7572 6573 2f68 6174 6368 3a32 223a 207b  ures/hatch:2": {
-00000100: 7d2c 0a20 2020 2022 6768 6372 2e69 6f2f  },.    "ghcr.io/
-00000110: 6465 7663 6f6e 7461 696e 6572 732d 636f  devcontainers-co
-00000120: 6e74 7269 622f 6665 6174 7572 6573 2f70  ntrib/features/p
-00000130: 616e 646f 633a 3122 3a20 7b7d 2c0a 2020  andoc:1": {},.  
-00000140: 2020 2267 6863 722e 696f 2f64 6576 636f    "ghcr.io/devco
-00000150: 6e74 6169 6e65 7273 2d63 6f6e 7472 6962  ntainers-contrib
-00000160: 2f66 6561 7475 7265 732f 7374 6172 7368  /features/starsh
-00000170: 6970 3a31 223a 207b 7d0a 2020 7d2c 0a20  ip:1": {}.  },. 
-00000180: 2022 7265 6d6f 7465 5573 6572 223a 2022   "remoteUser": "
-00000190: 7061 6e70 6466 222c 0a20 2022 636f 6e74  panpdf",.  "cont
-000001a0: 6169 6e65 7245 6e76 223a 207b 0a20 2020  ainerEnv": {.   
-000001b0: 2022 545a 223a 2022 4173 6961 2f54 6f6b   "TZ": "Asia/Tok
-000001c0: 796f 222c 0a20 2020 2022 5a4f 5445 524f  yo",.    "ZOTERO
-000001d0: 5f4c 4942 5241 5259 5f49 4422 3a20 2224  _LIBRARY_ID": "$
-000001e0: 7b6c 6f63 616c 456e 763a 5a4f 5445 524f  {localEnv:ZOTERO
-000001f0: 5f4c 4942 5241 5259 5f49 447d 222c 0a20  _LIBRARY_ID}",. 
-00000200: 2020 2022 5a4f 5445 524f 5f41 5049 5f4b     "ZOTERO_API_K
-00000210: 4559 223a 2022 247b 6c6f 6361 6c45 6e76  EY": "${localEnv
-00000220: 3a5a 4f54 4552 4f5f 4150 495f 4b45 597d  :ZOTERO_API_KEY}
-00000230: 220a 2020 7d2c 0a20 2022 7265 6d6f 7465  ".  },.  "remote
-00000240: 456e 7622 3a20 7b0a 2020 2020 2250 4154  Env": {.    "PAT
-00000250: 4822 3a20 2224 7b63 6f6e 7461 696e 6572  H": "${container
-00000260: 456e 763a 5041 5448 7d3a 2f75 7372 2f6c  Env:PATH}:/usr/l
-00000270: 6f63 616c 2f70 792d 7574 696c 732f 6269  ocal/py-utils/bi
-00000280: 6e22 0a20 207d 2c0a 2020 2f2f 2022 6d6f  n".  },.  // "mo
-00000290: 756e 7473 223a 205b 0a20 202f 2f20 2020  unts": [.  //   
-000002a0: 2273 6f75 7263 653d 247b 6c6f 6361 6c45  "source=${localE
-000002b0: 6e76 3a48 4f4d 457d 2f2e 636f 6e66 6967  nv:HOME}/.config
-000002c0: 2c74 6172 6765 743d 2f68 6f6d 652f 7061  ,target=/home/pa
-000002d0: 6e70 6466 2f2e 6c6f 6361 6c5f 636f 6e66  npdf/.local_conf
-000002e0: 6967 2c74 7970 653d 6269 6e64 2c63 6f6e  ig,type=bind,con
-000002f0: 7369 7374 656e 6379 3d63 6163 6865 6422  sistency=cached"
-00000300: 0a20 202f 2f20 5d2c 0a20 2022 6375 7374  .  // ],.  "cust
-00000310: 6f6d 697a 6174 696f 6e73 223a 207b 0a20  omizations": {. 
-00000320: 2020 2022 7673 636f 6465 223a 207b 0a20     "vscode": {. 
-00000330: 2020 2020 2022 7365 7474 696e 6773 223a       "settings":
-00000340: 207b 0a20 2020 2020 2020 202f 2f20 2274   {.        // "t
-00000350: 6572 6d69 6e61 6c2e 696e 7465 6772 6174  erminal.integrat
-00000360: 6564 2e64 6566 6175 6c74 5072 6f66 696c  ed.defaultProfil
-00000370: 652e 6c69 6e75 7822 3a20 2262 6173 6822  e.linux": "bash"
-00000380: 0a20 2020 2020 207d 2c0a 2020 2020 2020  .      },.      
-00000390: 2265 7874 656e 7369 6f6e 7322 3a20 5b0a  "extensions": [.
-000003a0: 2020 2020 2020 2020 2263 6861 726c 6965          "charlie
-000003b0: 726d 6172 7368 2e72 7566 6622 2c0a 2020  rmarsh.ruff",.  
-000003c0: 2020 2020 2020 2267 6974 6875 622e 7673        "github.vs
-000003d0: 636f 6465 2d67 6974 6875 622d 6163 7469  code-github-acti
-000003e0: 6f6e 7322 2c0a 2020 2020 2020 2020 226d  ons",.        "m
-000003f0: 732d 7079 7468 6f6e 2e70 7974 686f 6e22  s-python.python"
-00000400: 2c0a 2020 2020 2020 2020 226d 732d 7079  ,.        "ms-py
-00000410: 7468 6f6e 2e76 7363 6f64 652d 7079 6c61  thon.vscode-pyla
-00000420: 6e63 6522 2c0a 2020 2020 2020 2020 226d  nce",.        "m
-00000430: 732d 746f 6f6c 7361 692e 6a75 7079 7465  s-toolsai.jupyte
-00000440: 7222 0a20 2020 2020 205d 0a20 2020 207d  r".      ].    }
-00000450: 0a20 207d 2c0a 2020 2270 6f73 7443 7265  .  },.  "postCre
-00000460: 6174 6543 6f6d 6d61 6e64 223a 2022 2e64  ateCommand": ".d
-00000470: 6576 636f 6e74 6169 6e65 722f 706f 7374  evcontainer/post
-00000480: 4372 6561 7465 2e73 6822 0a0a 2020 2f2f  Create.sh"..  //
-00000490: 2055 7365 2027 666f 7277 6172 6450 6f72   Use 'forwardPor
-000004a0: 7473 2720 746f 206d 616b 6520 6120 6c69  ts' to make a li
-000004b0: 7374 206f 6620 706f 7274 7320 696e 7369  st of ports insi
-000004c0: 6465 2074 6865 2063 6f6e 7461 696e 6572  de the container
-000004d0: 2061 7661 696c 6162 6c65 206c 6f63 616c   available local
-000004e0: 6c79 2e0a 2020 2f2f 2022 666f 7277 6172  ly..  // "forwar
-000004f0: 6450 6f72 7473 223a 205b 5d2c 0a7d 0a    dPorts": [],.}.
+00000080: 2022 696e 7374 616c 6c5a 7368 223a 2066   "installZsh": f
+00000090: 616c 7365 2c0a 2020 2020 2020 2275 7365  alse,.      "use
+000000a0: 726e 616d 6522 3a20 2270 616e 7064 6622  rname": "panpdf"
+000000b0: 0a20 2020 207d 2c0a 2020 2020 2267 6863  .    },.    "ghc
+000000c0: 722e 696f 2f64 6576 636f 6e74 6169 6e65  r.io/devcontaine
+000000d0: 7273 2d63 6f6e 7472 6962 2f66 6561 7475  rs-contrib/featu
+000000e0: 7265 732f 6861 7463 683a 3222 3a20 7b7d  res/hatch:2": {}
+000000f0: 2c0a 2020 2020 2267 6863 722e 696f 2f64  ,.    "ghcr.io/d
+00000100: 6576 636f 6e74 6169 6e65 7273 2d63 6f6e  evcontainers-con
+00000110: 7472 6962 2f66 6561 7475 7265 732f 7061  trib/features/pa
+00000120: 6e64 6f63 3a31 223a 207b 7d2c 0a20 2020  ndoc:1": {},.   
+00000130: 2022 6768 6372 2e69 6f2f 6465 7663 6f6e   "ghcr.io/devcon
+00000140: 7461 696e 6572 732d 636f 6e74 7269 622f  tainers-contrib/
+00000150: 6665 6174 7572 6573 2f73 7461 7273 6869  features/starshi
+00000160: 703a 3122 3a20 7b7d 0a20 207d 2c0a 2020  p:1": {}.  },.  
+00000170: 2272 656d 6f74 6555 7365 7222 3a20 2270  "remoteUser": "p
+00000180: 616e 7064 6622 2c0a 2020 2263 6f6e 7461  anpdf",.  "conta
+00000190: 696e 6572 456e 7622 3a20 7b0a 2020 2020  inerEnv": {.    
+000001a0: 225a 4f54 4552 4f5f 4c49 4252 4152 595f  "ZOTERO_LIBRARY_
+000001b0: 4944 223a 2022 247b 6c6f 6361 6c45 6e76  ID": "${localEnv
+000001c0: 3a5a 4f54 4552 4f5f 4c49 4252 4152 595f  :ZOTERO_LIBRARY_
+000001d0: 4944 7d22 2c0a 2020 2020 225a 4f54 4552  ID}",.    "ZOTER
+000001e0: 4f5f 4150 495f 4b45 5922 3a20 2224 7b6c  O_API_KEY": "${l
+000001f0: 6f63 616c 456e 763a 5a4f 5445 524f 5f41  ocalEnv:ZOTERO_A
+00000200: 5049 5f4b 4559 7d22 0a20 207d 2c0a 2020  PI_KEY}".  },.  
+00000210: 2272 656d 6f74 6545 6e76 223a 207b 0a20  "remoteEnv": {. 
+00000220: 2020 2022 5041 5448 223a 2022 247b 636f     "PATH": "${co
+00000230: 6e74 6169 6e65 7245 6e76 3a50 4154 487d  ntainerEnv:PATH}
+00000240: 3a2f 7573 722f 6c6f 6361 6c2f 7079 2d75  :/usr/local/py-u
+00000250: 7469 6c73 2f62 696e 220a 2020 7d2c 0a20  tils/bin".  },. 
+00000260: 2022 6375 7374 6f6d 697a 6174 696f 6e73   "customizations
+00000270: 223a 207b 0a20 2020 2022 7673 636f 6465  ": {.    "vscode
+00000280: 223a 207b 0a20 2020 2020 2022 7365 7474  ": {.      "sett
+00000290: 696e 6773 223a 207b 7d2c 0a20 2020 2020  ings": {},.     
+000002a0: 2022 6578 7465 6e73 696f 6e73 223a 205b   "extensions": [
+000002b0: 0a20 2020 2020 2020 2022 6368 6172 6c69  .        "charli
+000002c0: 6572 6d61 7273 682e 7275 6666 222c 0a20  ermarsh.ruff",. 
+000002d0: 2020 2020 2020 2022 6769 7468 7562 2e76         "github.v
+000002e0: 7363 6f64 652d 6769 7468 7562 2d61 6374  scode-github-act
+000002f0: 696f 6e73 222c 0a20 2020 2020 2020 2022  ions",.        "
+00000300: 6d73 2d70 7974 686f 6e2e 7079 7468 6f6e  ms-python.python
+00000310: 222c 0a20 2020 2020 2020 2022 6d73 2d70  ",.        "ms-p
+00000320: 7974 686f 6e2e 7673 636f 6465 2d70 796c  ython.vscode-pyl
+00000330: 616e 6365 222c 0a20 2020 2020 2020 2022  ance",.        "
+00000340: 6d73 2d74 6f6f 6c73 6169 2e6a 7570 7974  ms-toolsai.jupyt
+00000350: 6572 220a 2020 2020 2020 5d0a 2020 2020  er".      ].    
+00000360: 7d0a 2020 7d2c 0a20 2022 706f 7374 4372  }.  },.  "postCr
+00000370: 6561 7465 436f 6d6d 616e 6422 3a20 222e  eateCommand": ".
+00000380: 6465 7663 6f6e 7461 696e 6572 2f70 6f73  devcontainer/pos
+00000390: 7443 7265 6174 652e 7368 220a 7d0a       tCreate.sh".}.
```

### Comparing `panpdf-0.1.6/examples/a.pdf` & `panpdf-0.1.7/examples/a.pdf`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/examples/defaults.yaml` & `panpdf-0.1.7/examples/defaults.yaml`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/examples/include-in-header.tex` & `panpdf-0.1.7/examples/include-in-header.tex`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/examples/images/figure.pdf` & `panpdf-0.1.7/examples/images/figure.pdf`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/examples/images/header.pdf` & `panpdf-0.1.7/examples/images/header.pdf`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/examples/src/1.md` & `panpdf-0.1.7/examples/src/1.md`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/notebooks/pdf.ipynb` & `panpdf-0.1.7/notebooks/pdf.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/notebooks/pgf.ipynb` & `panpdf-0.1.7/notebooks/pgf.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/notebooks/png.ipynb` & `panpdf-0.1.7/notebooks/png.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/notebooks/svg.ipynb` & `panpdf-0.1.7/notebooks/svg.ipynb`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/src/panpdf/formatters.py` & `panpdf-0.1.7/src/panpdf/formatters.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/src/panpdf/main.py` & `panpdf-0.1.7/src/panpdf/main.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/src/panpdf/stores.py` & `panpdf-0.1.7/src/panpdf/stores.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/src/panpdf/tools.py` & `panpdf-0.1.7/src/panpdf/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,15 @@
 from rich.console import Console
 from rich.progress import Progress, SpinnerColumn, TimeElapsedColumn
 
 if TYPE_CHECKING:
     from asyncio.streams import StreamReader
     from collections.abc import Callable, Iterable, Iterator
 
-console = Console()
-
+console = Console(log_time=False, log_path=False)
 
 PANDOC_PATH: list[Path] = []
 
 
 def get_pandoc_path(pandoc_cmd: str = "pandoc") -> Path:
     if PANDOC_PATH:
         return PANDOC_PATH[0]
@@ -162,14 +161,15 @@
     transient: bool = False,
     verbose: bool = False,
 ) -> int | None:
     with Progress(
         SpinnerColumn(),
         *Progress.get_default_columns(),
         TimeElapsedColumn(),
+        console=console,
         transient=transient,
     ) as progress:
         task = progress.add_task(description, total=None)
 
         def stdout(output: str) -> None:
             progress.log(f"[green]{output}".rstrip())
```

### Comparing `panpdf-0.1.6/src/panpdf/filters/attribute.py` & `panpdf-0.1.7/src/panpdf/filters/attribute.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/src/panpdf/filters/crossref.py` & `panpdf-0.1.7/src/panpdf/filters/crossref.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/src/panpdf/filters/filter.py` & `panpdf-0.1.7/src/panpdf/filters/filter.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/src/panpdf/filters/jupyter.py` & `panpdf-0.1.7/src/panpdf/filters/jupyter.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/src/panpdf/filters/layout.py` & `panpdf-0.1.7/src/panpdf/filters/layout.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/src/panpdf/filters/verbatim.py` & `panpdf-0.1.7/src/panpdf/filters/verbatim.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/src/panpdf/filters/zotero.py` & `panpdf-0.1.7/src/panpdf/filters/zotero.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/conftest.py` & `panpdf-0.1.7/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/test_converters.py` & `panpdf-0.1.7/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/test_formatters.py` & `panpdf-0.1.7/tests/test_formatters.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/test_main.py` & `panpdf-0.1.7/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/test_stores.py` & `panpdf-0.1.7/tests/test_stores.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/test_tools.py` & `panpdf-0.1.7/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/filters/test_attribute.py` & `panpdf-0.1.7/tests/filters/test_attribute.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/filters/test_crossref.py` & `panpdf-0.1.7/tests/filters/test_crossref.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/filters/test_filter.py` & `panpdf-0.1.7/tests/filters/test_filter.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/filters/test_jupyter.py` & `panpdf-0.1.7/tests/filters/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/filters/test_layout.py` & `panpdf-0.1.7/tests/filters/test_layout.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/filters/test_zotero.py` & `panpdf-0.1.7/tests/filters/test_zotero.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/libraries/test_nbformat.py` & `panpdf-0.1.7/tests/libraries/test_nbformat.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/libraries/panflute/test_cite.py` & `panpdf-0.1.7/tests/libraries/panflute/test_cite.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/libraries/panflute/test_code.py` & `panpdf-0.1.7/tests/libraries/panflute/test_code.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/libraries/panflute/test_figure.py` & `panpdf-0.1.7/tests/libraries/panflute/test_figure.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/libraries/panflute/test_math.py` & `panpdf-0.1.7/tests/libraries/panflute/test_math.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/libraries/panflute/test_metadata.py` & `panpdf-0.1.7/tests/libraries/panflute/test_metadata.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/libraries/panflute/test_raw.py` & `panpdf-0.1.7/tests/libraries/panflute/test_raw.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/libraries/panflute/test_section.py` & `panpdf-0.1.7/tests/libraries/panflute/test_section.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/libraries/panflute/test_table.py` & `panpdf-0.1.7/tests/libraries/panflute/test_table.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/tests/libraries/panflute/test_tex.py` & `panpdf-0.1.7/tests/libraries/panflute/test_tex.py`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/LICENSE.txt` & `panpdf-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/README.md` & `panpdf-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/pyproject.toml` & `panpdf-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `panpdf-0.1.6/PKG-INFO` & `panpdf-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: panpdf
-Version: 0.1.6
+Version: 0.1.7
 Summary: PDF documentation generator
 Project-URL: Documentation, https://daizutabi.github.io/panpdf
 Project-URL: Source, https://github.com/daizutabi/panpdf
 Project-URL: Issues, https://github.com/daizutabi/panpdf/issues
 Author-email: daizutabi <daizutabi@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

