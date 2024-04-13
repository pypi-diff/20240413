# Comparing `tmp/latex_rubber-1.6.4.tar.gz` & `tmp/latex_rubber-1.6.5.tar.gz`

## Comparing `latex_rubber-1.6.4.tar` & `latex_rubber-1.6.5.tar`

### file list

```diff
@@ -1,74 +1,284 @@
--rw-r--r--   0        0        0    74904 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/rubber.html
--rw-r--r--   0        0        0    48721 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/rubber.info
--rw-r--r--   0        0        0   178373 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/rubber.pdf
--rw-r--r--   0        0        0    42055 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/rubber.texi
--rw-r--r--   0        0        0    42677 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/rubber.txt
--rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/man-en/rubber-info.1
--rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/man-en/rubber.1
--rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/man-fr/rubber-info.1
--rw-r--r--   0        0        0    21029 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/doc/man-fr/rubber.1
--rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/misc/zsh-completion
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/__init__.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/biblio.py
--rw-r--r--   0        0        0    26287 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/cmdline.py
--rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/contents.py
--rw-r--r--   0        0        0     9270 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/convert.py
--rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/depend.py
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/dvip_tool.py
--rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/environment.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/index.py
--rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/module_interface.py
--rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/rules.ini
--rw-r--r--   0        0        0    14742 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/tex.py
--rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/util.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/__init__.py
--rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/compressor.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/eps_gz.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/fig2dev.py
--rw-r--r--   0        0        0    48052 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/latex.py
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/literate.py
--rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/mpost.py
--rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/converters/shell.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/__init__.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/aleph.py
--rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/asymptote.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/backref.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/beamer.py
--rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/biblatex.py
--rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/bibtex.py
--rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/bibtopic.py
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/combine.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/dvipdfm.py
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/dvips.py
--rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/epsfig.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/glossaries.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/gnuplottex.py
--rw-r--r--   0        0        0     7513 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/graphics.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/graphicx.py -> graphics.py
--rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/hyperref.py
--rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/index.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/listings.py
--rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/ltxtable.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/lualatex.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/makeidx.py
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/minitoc-hyper.py -> minitoc.py
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/minitoc.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/moreverb.py
--rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/multibib.py
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/nomencl.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/ntheorem.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/omega.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/pdftex.py
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/ps2pdf.py
--rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/pythontex.py
--rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/verbatim.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/vtex.py
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/xelatex.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/rubber/latex_modules/xr.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/COPYING
--rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/README.md
--rw-r--r--   0        0        0    10043 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/hatch_build.py
--rw-r--r--   0        0        0     1190 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/pyproject.toml
--rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 latex_rubber-1.6.4/PKG-INFO
+-rw-r--r--   0        0        0    15543 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/NEWS
+-rw-r--r--   0        0        0    74904 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/doc/rubber/rubber.html
+-rw-r--r--   0        0        0    48721 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/doc/rubber/rubber.info
+-rw-r--r--   0        0        0   176272 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/doc/rubber/rubber.pdf
+-rw-r--r--   0        0        0    42055 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/doc/rubber/rubber.texi
+-rw-r--r--   0        0        0    42055 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/doc/rubber/rubber.texi.in
+-rw-r--r--   0        0        0    42677 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/doc/rubber/rubber.txt
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/man/fr/man1/rubber-info.1
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/man/fr/man1/rubber-info.1.in
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/man/fr/man1/rubber-pipe.1
+-rw-r--r--   0        0        0    21029 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/man/fr/man1/rubber.1
+-rw-r--r--   0        0        0    20999 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/man/fr/man1/rubber.1.in
+-rw-r--r--   0        0        0     2565 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/man/man1/rubber-info.1
+-rw-r--r--   0        0        0     2535 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/man/man1/rubber-info.1.in
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/man/man1/rubber-pipe.1
+-rw-r--r--   0        0        0    18467 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/man/man1/rubber.1
+-rw-r--r--   0        0        0    18437 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/man/man1/rubber.1.in
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/misc/zsh-completion
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/__init__.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/biblio.py
+-rw-r--r--   0        0        0    26287 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/cmdline.py
+-rw-r--r--   0        0        0     4265 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/contents.py
+-rw-r--r--   0        0        0     9270 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/convert.py
+-rw-r--r--   0        0        0    11277 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/depend.py
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/dvip_tool.py
+-rw-r--r--   0        0        0     4782 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/environment.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/index.py
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/module_interface.py
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/rules.ini
+-rw-r--r--   0        0        0    14742 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/tex.py
+-rw-r--r--   0        0        0    10336 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/util.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/converters/__init__.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/converters/compressor.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/converters/eps_gz.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/converters/fig2dev.py
+-rw-r--r--   0        0        0    48052 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/converters/latex.py
+-rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/converters/literate.py
+-rw-r--r--   0        0        0     7804 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/converters/mpost.py
+-rw-r--r--   0        0        0      761 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/converters/shell.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/__init__.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/aleph.py
+-rw-r--r--   0        0        0     4204 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/asymptote.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/backref.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/beamer.py
+-rw-r--r--   0        0        0     4274 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/biblatex.py
+-rw-r--r--   0        0        0      863 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/bibtex.py
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/bibtopic.py
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/combine.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/dvipdfm.py
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/dvips.py
+-rw-r--r--   0        0        0     1298 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/epsfig.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/glossaries.py
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/gnuplottex.py
+-rw-r--r--   0        0        0     7513 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/graphics.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/graphicx.py -> graphics.py
+-rw-r--r--   0        0        0      370 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/hyperref.py
+-rw-r--r--   0        0        0     3602 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/index.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/listings.py
+-rw-r--r--   0        0        0      620 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/ltxtable.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/lualatex.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/makeidx.py
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/minitoc-hyper.py -> minitoc.py
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/minitoc.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/moreverb.py
+-rw-r--r--   0        0        0     2544 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/multibib.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/nomencl.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/ntheorem.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/omega.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/pdftex.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/ps2pdf.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/pythontex.py
+-rw-r--r--   0        0        0      669 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/verbatim.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/vtex.py
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/xelatex.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/rubber/latex_modules/xr.py
+-rwxr-xr-x   0        0        0     3268 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/run.sh
+-rw-r--r--   0        0        0      300 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/asymptote-aux-overwritten/doc.tex
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/asymptote-dvi/doc.tex
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/asymptote-dvipdfm/doc.tex
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/asymptote-dvips/doc.tex
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/asymptote-dvips-ps2pdf/doc.tex
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/asymptote-inline-dvi/doc.tex
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/asymptote-inline-dvipdfm/doc.tex
+-rw-r--r--   0        0        0      172 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/asymptote-inline-dvips/doc.tex
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/asymptote-inline-dvips-ps2pdf/doc.tex
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/asymptote-inline-pdftex/doc.tex
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/asymptote-pdftex/doc.tex
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/asymptote-twice/doc.tex
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/backref-hyperref/doc.tex
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/beamer/arguments
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/beamer/doc.tex
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-addres-oa/doc.tex
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-addres-oa/expected
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-basic/doc.tex
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-basic/expected
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-biber-fails/doc.tex
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-biber-fails/fragment
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-bibtex/doc.tex
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-bibtex/expected
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-bibtex-fails/doc.tex
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-bibtex-fails/fragment
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-inplace-cwd/doc.tex
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-inplace-cwd/fragment
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-inplace-subdir/doc.tex
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-inplace-subdir/fragment
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-multiple-res/biblio2.bib
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-multiple-res/doc.tex
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-multiple-res/expected
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-path-dir/doc.tex
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/biblatex-path-dir/fragment
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-basic/doc.tex
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-basic/expected
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-bibtex8/doc.tex
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-bibtex8/expected
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-fails/doc.tex
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-fails/fragment
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-inplace-cwd/doc.tex
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-inplace-cwd/fragment
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-inplace-subdir/doc.tex
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-inplace-subdir/fragment
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-no-line-no/doc.tex
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-no-line-no/fragment
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-path-dir/doc.tex
+-rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-path-dir/fragment
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-warning/doc.tex
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-warning/expected
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtex-warning/faulty.bib
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/bibtopic/doc.tex
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/combine/combine1.tex
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/combine/doc.tex
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/cweb-latex/arguments
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/cweb-latex/document
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/cweb-latex/wcltx.bib
+-rw-r--r--   0        0        0    10241 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/cweb-latex/wcltx.w
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/dvips-bad-options/doc.tex
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/dvips-bad-options/fragment
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/dvips-fails/doc.tex
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/dvips-fails/fragment
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/epsfig-epsffile/doc.tex
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/epsfig-psfig/doc.tex
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/fig2dev-dvi/doc.tex
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/fig2dev-dvi/figure.fig
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/fig2dev-path/doc.tex
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/fig2dev-path/figure.fig
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/fig2dev-path/fragment
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/fig2dev-path-inplace/doc.tex
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/fig2dev-path-inplace/figure.fig
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/fig2dev-path-inplace/fragment
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/fig2dev-path-into/doc.tex
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/fig2dev-path-into/figure.fig
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/fig2dev-path-into/fragment
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/glossaries/doc.tex
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/graphics/doc.tex
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/graphics-epsgz/doc.tex
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/graphics-epsgz/fragment
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/graphicx/doc.tex
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/graphicx-dotted-files/doc.tex
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/graphicx-dotted-files/empty1.0.png
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/graphicx-dotted-files/fragment
+-rw-r--r--   0        0        0      121 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/graphicx-star/doc.tex
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/hash-not-mtime/doc.tex
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/hash-not-mtime/fragment
+-rw-r--r--   0        0        0       90 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/help/fragment
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/hooks-input-file/bar.tex
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/hooks-input-file/doc.tex
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/hooks-input-file/foo.fig
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/hyperref-backref/doc.tex
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/hyperref-backref/expected
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/hyperref-basic/doc.tex
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/include/doc.tex
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/includeonly/break.tex
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/includeonly/doc.tex
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/includeonly/lorem.tex
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/includeonly-command-line/arguments
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/includeonly-command-line/break.tex
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/includeonly-command-line/doc.tex
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/includeonly-command-line/lorem.tex
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/index-basic/doc.tex
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/index-basic/expected
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/info/doc.tex
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/info/fragment
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/info-deps/doc.tex
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/info-deps/fragment
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/info-index-error/doc.tex
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/info-index-error/fragment
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/info-into/doc.tex
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/info-into/fragment
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/inputenc-latin1/doc.tex
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/inputenc-latin9/doc.tex
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/inputenc-utf8/doc.tex
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/knitr/arguments
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/knitr/doc.Rtex
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/knitr/document
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/listings-basic/doc.tex
+-rw-r--r--   0        0        0      303 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/listings-comment-lstinputlisting/doc.tex
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/listings-comment-lstinputlisting/lst-depends-wrong-parse.tex
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/listings-comment-lstinputlisting/lst-depends-wrong-parse2.tex
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/logfile-excessive/doc.tex
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-dvi/doc.tex
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-dvi/expected
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-dvi-gz/arguments
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-dvi-gz/doc.tex
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-dvi-gz/expected
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-dvipdfm/doc.tex
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-dvipdfm/expected
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-dvips/doc.tex
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-dvips/expected
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-dvips-ps2pdf/doc.tex
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-dvips-ps2pdf/expected
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-minus-dee/arguments
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-minus-dee/doc.tex
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-pdftex/doc.tex
+-rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-pdftex-bzip2/arguments
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/loremipsum-pdftex-bzip2/doc.tex
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/ltxtable/doc.tex
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/ltxtable/ltxtable1.tex
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/lualatex/doc.tex
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/makeidx/doc.tex
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/makeidx-order-german/doc.tex
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/makeidx-order-german/umlaut.ist
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/makeidx-order-letter/doc.tex
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/metapost/doc.tex
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/metapost/metapost.mp
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/metapost-error/doc.tex
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/metapost-error/fragment
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/metapost-error/metapost.mp
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/metapost-input/doc.tex
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/metapost-input/included.mp
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/metapost-input/metapost.mp
+-rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/minitoc/doc.tex
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/moreverb/doc.tex
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/multibib/doc.tex
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/multibib/expected
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/multibib-path-dir/doc.tex
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/multibib-path-dir/fragment
+-rw-r--r--   0        0        0      178 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/nomencl/doc.tex
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/ntheorem/doc.tex
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/parser/fragment
+-rw-r--r--   0        0        0     1970 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/parser/parser.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pdfoutput0-auto/doc.tex
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pdfoutput0-auto/expected
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pdfoutput0-pdftex/doc.tex
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pdfoutput0-pdftex/expected
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pdfoutput1-auto/doc.tex
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pdfoutput1-auto/expected
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pdfoutput1-pdftex/doc.tex
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pdfoutput1-pdftex/expected
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pipe/doc.tex
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pipe/fragment
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pipe-keep/doc.tex
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pipe-keep/fragment
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pstricks-pd/arguments
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pstricks-pd/doc.tex
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pythontex/arguments
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/pythontex/doc.tex
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/rebuild-on-missing-end-product/doc.tex
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/rebuild-on-missing-end-product/fragment
+-rwxr-xr-x   0        0        0      292 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/report-issues/fragment
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/report-issues/main.tex
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/rubber-read-directive/doc.tex
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/rubber-read-directive/read_directives.rub
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/shared/biblio.bib
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/shared/biblioa.bib
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/shared/bibliob.bib
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/shared/brokenbib.bib
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/shared/ipsum.tex
+-rw-r--r--   0        0        0      461 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/shared/sample.eps
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/synctex-cmdline/arguments
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/synctex-cmdline/doc.tex
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/synctex-cmdline/expected
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/synctex-directive/doc.tex
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/synctex-directive/expected
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/synctex-macro/doc.tex
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/synctex-macro/expected
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/toc/doc.tex
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/toc/expected
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/tests/verbatim/doc.tex
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/COPYING
+-rw-r--r--   0        0        0     6730 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/README.md
+-rw-r--r--   0        0        0    10379 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/hatch_build.py
+-rw-r--r--   0        0        0     1294 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/pyproject.toml
+-rw-r--r--   0        0        0     7128 2020-02-02 00:00:00.000000 latex_rubber-1.6.5/PKG-INFO
```

### Comparing `latex_rubber-1.6.4/doc/rubber.html` & `latex_rubber-1.6.5/doc/rubber/rubber.html`

 * *Files 0% similar despite different names*

```diff
@@ -21,18 +21,18 @@
 under the above conditions for modified versions,
 except that this permission notice may be stated in a
 translation approved by the Free Software Foundation.
 
 Copyright © 2002-2006 Emmanuel Beffara.
 
 Copyright © 2006-2015 Sebastian Kapfer. -->
-<title>Rubber Manual 1.6.4</title>
+<title>Rubber Manual 1.6.5</title>
 
-<meta name="description" content="Rubber Manual 1.6.4">
-<meta name="keywords" content="Rubber Manual 1.6.4">
+<meta name="description" content="Rubber Manual 1.6.5">
+<meta name="keywords" content="Rubber Manual 1.6.5">
 <meta name="resource-type" content="document">
 <meta name="distribution" content="global">
 <meta name="Generator" content="makeinfo">
 <meta name="viewport" content="width=device-width,initial-scale=1">
 
 <link href="#Top" rel="start" title="Top">
 <link href="#Introduction" rel="next" title="Introduction">
```

### Comparing `latex_rubber-1.6.4/doc/rubber.info` & `latex_rubber-1.6.5/doc/rubber/rubber.info`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/doc/rubber.pdf` & `latex_rubber-1.6.5/doc/rubber/rubber.pdf`

 * *Files 18% similar despite different names*

#### Comparing `latex_rubber-1.6.4/doc/rubber.pdf` & `latex_rubber-1.6.5/doc/rubber/rubber.pdf`

 * *Document info*

```diff
@@ -1,6 +1,6 @@
-CreationDate: "D:20240410175245+02'00'"
+CreationDate: "D:20240413155624+02'00'"
 Creator: 'TeX'
-ModDate: "D:20240410175245+02'00'"
-PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.22 (TeX Live 2021 Gentoo Linux) kpathsea version 6.3.3'
-Producer: 'pdfTeX-1.40.22'
+ModDate: "D:20240413155624+02'00'"
+PTEX.Fullbanner: 'This is pdfTeX, Version 3.141592653-2.6-1.40.25 (TeX Live 2023 Gentoo Linux) kpathsea version 6.3.5'
+Producer: 'pdfTeX-1.40.25'
 Trapped: '/False'
```

#### pdftotext {} -

```diff
@@ -1,9 +1,9 @@
 Rubber
-Documentation for version 1.6.4
+Documentation for version 1.6.5
 
 Sebastian Kapfer
 
 Permission is granted to make and distribute verbatim copies of this manual provided the
 copyright notice and this permission notice are preserved on all copies.
 Permission is granted to copy and distribute modified versions of this manual under the
 conditions for verbatim copying, provided also that the sections entitled “Copying” and
@@ -14,80 +14,46 @@
 may be stated in a translation approved by the Free Software Foundation.
 Copyright c 2002–2006 Emmanuel Beffara.
 Copyright c 2006–2015 Sebastian Kapfer.
 
 i
 
 Table of Contents
-1
-
-Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 1
-
-2
-
-Command lines . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
-2.1
-2.2
-
-3
-
-Directives . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6
-3.1
-3.2
-
-4
-
-Syntax for rubber and rubber-pipe . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
-Syntax for rubber-info . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
-
-General directives . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6
-Variables . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
-
-Modules . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
-4.1
-
-Supported Packages . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
-4.1.1 BibLaTeX support . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10
-4.1.2 BibTeX support . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10
-4.1.3 Index generation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10
-4.2 Post-processors . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11
-4.2.1 Dvips and Dvipdfm . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 12
-4.2.2 Source file expansion. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 12
-4.3 Changing compilers. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 12
-
-5
-
-Graphics conversion. . . . . . . . . . . . . . . . . . . . . . . . . . . . 14
-5.1
-5.2
-5.3
-
-6
-
-Encoding issues . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 17
-6.1
-6.2
-6.3
-
-7
-
-Conversion algorithm . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 14
-Standard conversion rules . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 15
-Syntax of rules.ini . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 15
-
-Design choices about input and output encoding.. . . . . . . . . . . . . . . 17
-Conversion of legacy sources to UTF-8 . . . . . . . . . . . . . . . . . . . . . . . . . 17
-Handling of unconverted legacy sources . . . . . . . . . . . . . . . . . . . . . . . . 17
-
-Index . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 19
-7.1
-7.2
-
-Index of directives . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 19
-Index of modules . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 19
+1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 1
+2 Command lines. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
+2.1 Syntax for rubber and rubber-pipe . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 2
+2.2 Syntax for rubber-info . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 4
+
+3 Directives . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6
+3.1 General directives . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6
+3.2 Variables . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 7
+
+4 Modules . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
+4.1 Supported Packages . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9
+4.1.1 BibLaTeX support. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10
+4.1.2 BibTeX support . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10
+4.1.3 Index generation. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10
+4.2 Post-processors . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 11
+4.2.1 Dvips and Dvipdfm. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 12
+4.2.2 Source file expansion . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 12
+4.3 Changing compilers . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 12
+
+5 Graphics conversion . . . . . . . . . . . . . . . . . . . . . . . . . . . . 14
+5.1 Conversion algorithm . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 14
+5.2 Standard conversion rules . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 15
+5.3 Syntax of rules.ini . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 15
+
+6 Encoding issues . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 17
+6.1 Design choices about input and output encoding. . . . . . . . . . . . . . . . 17
+6.2 Conversion of legacy sources to UTF-8 . . . . . . . . . . . . . . . . . . . . . . . . . . 17
+6.3 Handling of unconverted legacy sources . . . . . . . . . . . . . . . . . . . . . . . . . 17
+
+7 Index . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 19
+7.1 Index of directives . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 19
+7.2 Index of modules . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 19
 
 1
 
 1 Introduction
 The purpose of Rubber is to make the building of a document automated, from the source
 files to the final document file, replacing the work of a Makefile.
 The basis is a routine that compiles a LaTeX source the right number of times to resolve
@@ -286,16 +252,15 @@
 all
 
 all of the above.
 
 2.2 Syntax for rubber-info
 The command-line syntax for rubber-info is the following:
 rubber-info [options] [action] source
-The options are all those accepted by rubber and rubber-pipe, as described in
-Section 2.1 [rubber command line], page 2. The action specified what kind of information
+The options are all those accepted by rubber and rubber-pipe, as described in Section 2.1 [rubber command line], page 2. The action specified what kind of information
 
 Chapter 2: Command lines
 
 5
 
 has to be extracted. At most one such argument must be present on the command line,
 --check is assumed if none is present. The possible actions are:
@@ -436,16 +401,15 @@
 
 Chapter 3: Directives
 
 8
 
 engine
 
-Deprecated. Please use a module to change the compiler, as described in
-Section 4.3 [Compiler choice], page 12.
+Deprecated. Please use a module to change the compiler, as described in Section 4.3 [Compiler choice], page 12.
 
 file
 
 Deprecated. The name of the current file (this is set during parsing).
 
 job
 
@@ -654,16 +618,15 @@
 dvipdfm.options <options>
 dvips.options <options>
 Pass the specified options to the driver. The argument is a space-separated list
 of options that are passed before the DVI file’s name.
 
 4.2.2 Source file expansion
 The module expand produces a LaTeX source from the original one by expanding included
-files and packages. If the main file is foo.tex then then expanded file will be named
-foo-final.tex. This file will be self-contained, in particular it will not need BibTeXing nor
+files and packages. If the main file is foo.tex then then expanded file will be named foofinal.tex. This file will be self-contained, in particular it will not need BibTeXing nor
 user-defined packages, as may be required when preparing the final version of a document
 for publication.
 As additional effect, this module removes all comments from the source file (including
 those that may contain Rubber directives). It also removes any text that may be present
 after \end{document}.
 Please note that this module is rather experimental.
 The following options control how the expansion is done:
@@ -859,15 +822,15 @@
 appropriate option when saving from your favorite editor, or with a dedicated tool. For
 example, the following commands translate doc.tex from the latin1 encoding.
 cp doc.tex doc.tex.bak
 iconv doc.tex.bak -f latin1 -o doc.tex -t utf-8
 You should then update the inputenc line, check that the compilation goes well, and
 finally remove the doc.tex.bak backup.
 Legacy US-ASCII sources, only containing bytes betwen 0 and 127 and relying on TeX
-constructs like \’e to encode local characters, are valid UTF-8 sources, and will be decoded
+constructs like \'e to encode local characters, are valid UTF-8 sources, and will be decoded
 correctly. No conversion is needed.
 More generally, conversion from usual (8-bits, US-ASCII-compatible) encodings will only
 replace bytes from 128 to 255 with new UTF-8 byte sequences, but US-ASCII bytes will
 remain unchanged.
 
 6.3 Handling of unconverted legacy sources
 For various reasons, some sources cannot be converted. Rubber attempts to deal with them,
```

### Comparing `latex_rubber-1.6.4/doc/rubber.texi` & `latex_rubber-1.6.5/doc/rubber/rubber.texi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 \input texinfo
 @c %**start of header
 @setfilename rubber.info
-@settitle Rubber Manual 1.6.4
+@settitle Rubber Manual 1.6.5
 @c %**end of header
 
 @copying
 Permission is granted to make and distribute verbatim
 copies of this manual provided the copyright notice and
 this permission notice are preserved on all copies.
 
@@ -27,15 +27,15 @@
 Copyright @copyright{} 2002--2006 Emmanuel Beffara.
 
 Copyright @copyright{} 2006--2015 Sebastian Kapfer.
 @end copying
 
 @titlepage
 @title Rubber
-@subtitle Documentation for version 1.6.4
+@subtitle Documentation for version 1.6.5
 @author Sebastian Kapfer
 @page
 @vskip 0pt plus 1fill
 @insertcopying
 @end titlepage
 
 @iftex
```

### Comparing `latex_rubber-1.6.4/doc/rubber.txt` & `latex_rubber-1.6.5/doc/rubber/rubber.txt`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/doc/man-en/rubber-info.1` & `latex_rubber-1.6.5/man/man1/rubber-info.1`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 Stupidly enumerate all LaTeX warnings, i.e. all the lines in the log file that
 contain the string "Warning".
 .PP
 
 .SH BUGS
 There are surely a some...
 
-This page documents Rubber version 1.6.4.
+This page documents Rubber version 1.6.5.
 The program and this man-page are maintained by Florian Schmaus <flo@geekplace.eu>.
 The homepage for Rubber can be found at https://gitlab.com/latex-rubber/rubber.
 
 .SH SEE ALSO
 The full documentation for
 .B rubber
 is maintained as a Texinfo manual.  If the
```

### Comparing `latex_rubber-1.6.4/doc/man-en/rubber.1` & `latex_rubber-1.6.5/man/man1/rubber.1`

 * *Files 0% similar despite different names*

```diff
@@ -636,15 +636,15 @@
 module, which may be used to specify the list of bibliographies the command
 applies to.
 .PP
 .
 .SH BUGS
 There are surely a some...
 .PP
-This page documents Rubber version 1.6.4.
+This page documents Rubber version 1.6.5.
 The program and this man-page are maintained by Florian Schmaus <flo@geekplace.eu>.
 The homepage for Rubber can be found at https://gitlab.com/latex-rubber/rubber.
 .
 .SH SEE ALSO
 The full documentation for
 .B rubber
 is maintained as a Texinfo manual.  If the
```

### Comparing `latex_rubber-1.6.4/doc/man-fr/rubber-info.1` & `latex_rubber-1.6.5/man/fr/man1/rubber-info.1`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 Affiche stupidement la liste de tous les avertissements de LaTeX, c'est-à-dire
 toutes les lignes du fichier log qui contiennent « Warning ».
 .PP
 
 .SH BUGS
 Il y en a surement quelques uns...
 
-Cette page se rapporte à la version 1.6.4 de Rubber. Le programme et cette
+Cette page se rapporte à la version 1.6.5 de Rubber. Le programme et cette
 documentation sont maintenus par Florian Schmaus <flo@geekplace.eu>.
 La page web du programme se trouve à l'adresse https://gitlab.com/latex-rubber/rubber.
 
 .SH VOIR AUSSI
 La documentation complète de
 .B rubber
 est maintenue en tant que manuel en Texinfo. Si les programmes
```

### Comparing `latex_rubber-1.6.4/doc/man-fr/rubber.1` & `latex_rubber-1.6.5/man/fr/man1/rubber.1`

 * *Files 0% similar despite different names*

```diff
@@ -657,15 +657,15 @@
 qui permet de spécifier la liste des bibliographies auxquelles s’applique la
 commande.
 .PP
 .
 .SH BUGS
 Il y en a surement quelques uns...
 .PP
-Cette page se rapporte à la version 1.6.4 de Rubber. Le programme et cette
+Cette page se rapporte à la version 1.6.5 de Rubber. Le programme et cette
 documentation sont maintenus par Florian Schmaus <flo@geekplace.eu>.
 La page web du programme se trouve à l’adresse https://gitlab.com/latex-rubber/rubber.
 .
 .SH VOIR AUSSI
 La documentation complète de
 .B rubber
 est maintenue en tant que manuel en Texinfo.
```

### Comparing `latex_rubber-1.6.4/misc/zsh-completion` & `latex_rubber-1.6.5/misc/zsh-completion`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/biblio.py` & `latex_rubber-1.6.5/rubber/biblio.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/cmdline.py` & `latex_rubber-1.6.5/rubber/cmdline.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/contents.py` & `latex_rubber-1.6.5/rubber/contents.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/convert.py` & `latex_rubber-1.6.5/rubber/convert.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/depend.py` & `latex_rubber-1.6.5/rubber/depend.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/dvip_tool.py` & `latex_rubber-1.6.5/rubber/dvip_tool.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/environment.py` & `latex_rubber-1.6.5/rubber/environment.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/index.py` & `latex_rubber-1.6.5/rubber/index.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/module_interface.py` & `latex_rubber-1.6.5/rubber/module_interface.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/rules.ini` & `latex_rubber-1.6.5/rubber/rules.ini`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/tex.py` & `latex_rubber-1.6.5/rubber/tex.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/util.py` & `latex_rubber-1.6.5/rubber/util.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/converters/compressor.py` & `latex_rubber-1.6.5/rubber/converters/compressor.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/converters/eps_gz.py` & `latex_rubber-1.6.5/rubber/converters/eps_gz.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/converters/fig2dev.py` & `latex_rubber-1.6.5/rubber/converters/fig2dev.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/converters/latex.py` & `latex_rubber-1.6.5/rubber/converters/latex.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/converters/literate.py` & `latex_rubber-1.6.5/rubber/converters/literate.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/converters/mpost.py` & `latex_rubber-1.6.5/rubber/converters/mpost.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/converters/shell.py` & `latex_rubber-1.6.5/rubber/converters/shell.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/asymptote.py` & `latex_rubber-1.6.5/rubber/latex_modules/asymptote.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/beamer.py` & `latex_rubber-1.6.5/rubber/latex_modules/beamer.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/biblatex.py` & `latex_rubber-1.6.5/rubber/latex_modules/biblatex.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/bibtex.py` & `latex_rubber-1.6.5/rubber/latex_modules/bibtex.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/bibtopic.py` & `latex_rubber-1.6.5/rubber/latex_modules/bibtopic.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/combine.py` & `latex_rubber-1.6.5/rubber/latex_modules/combine.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/epsfig.py` & `latex_rubber-1.6.5/rubber/latex_modules/epsfig.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/glossaries.py` & `latex_rubber-1.6.5/rubber/latex_modules/glossaries.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/graphics.py` & `latex_rubber-1.6.5/rubber/latex_modules/graphics.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/index.py` & `latex_rubber-1.6.5/rubber/latex_modules/index.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/listings.py` & `latex_rubber-1.6.5/rubber/latex_modules/listings.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/ltxtable.py` & `latex_rubber-1.6.5/rubber/latex_modules/ltxtable.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/minitoc.py` & `latex_rubber-1.6.5/rubber/latex_modules/minitoc.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/moreverb.py` & `latex_rubber-1.6.5/rubber/latex_modules/moreverb.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/multibib.py` & `latex_rubber-1.6.5/rubber/latex_modules/multibib.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/pdftex.py` & `latex_rubber-1.6.5/rubber/latex_modules/pdftex.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/ps2pdf.py` & `latex_rubber-1.6.5/rubber/latex_modules/ps2pdf.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/pythontex.py` & `latex_rubber-1.6.5/rubber/latex_modules/pythontex.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/verbatim.py` & `latex_rubber-1.6.5/rubber/latex_modules/verbatim.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/vtex.py` & `latex_rubber-1.6.5/rubber/latex_modules/vtex.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/rubber/latex_modules/xr.py` & `latex_rubber-1.6.5/rubber/latex_modules/xr.py`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/COPYING` & `latex_rubber-1.6.5/COPYING`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/README.md` & `latex_rubber-1.6.5/README.md`

 * *Files identical despite different names*

### Comparing `latex_rubber-1.6.4/hatch_build.py` & `latex_rubber-1.6.5/hatch_build.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,22 +29,22 @@
     Builds Rubber documentaton by (1) substituting placeholders
     and (2) calling out to GNU Texinfo for rendering.
     """
 
     # A file f is generated from f.in by replacing @author@, @version@ by
     # sensible values (as ./configure does in the autoconf world).
     _FILES_WITH_SUBSTITUTIONS = (
-        join("doc", "man-en", "rubber.1"),
-        join("doc", "man-en", "rubber-info.1"),
-        join("doc", "man-fr", "rubber.1"),
-        join("doc", "man-fr", "rubber-info.1"),
-        join("doc", "rubber.texi"),
+        join("man", "man1", "rubber.1"),
+        join("man", "man1", "rubber-info.1"),
+        join("man", "fr", "man1", "rubber.1"),
+        join("man", "fr", "man1", "rubber-info.1"),
+        join("doc", "rubber", "rubber.texi"),
     )
 
-    _MANUAL_BASENAME = join("doc", "rubber.")
+    _MANUAL_BASENAME = join("doc", "rubber", "rubber.")
 
     _DOC_RECIPES = (
         ("html", ("makeinfo", "--html", "--no-split")),
         ("info", ("makeinfo", "--info")),
         ("pdf", ("texi2dvi", "--pdf", "--quiet", "--tidy")),
         ("txt", ("makeinfo", "--plaintext")),
     )
@@ -194,14 +194,21 @@
                 for filename in doc_builder.iterate_filenames():
                     build_data["force_include"][abspath(filename)] = join(
                         wheel_data_prefix, filename)
 
                 build_data["force_include"][abspath(join("misc", "zsh-completion"))] = join(
                     wheel_data_prefix, "zsh", "site-functions", "_rubber")
 
+                for filename in [
+                        join("man", "man1", "rubber-pipe.1"),
+                        join("man", "fr", "man1", "rubber-pipe.1"),
+                ]:
+                    build_data["force_include"][abspath(filename)] = join(
+                        wheel_data_prefix, filename)
+
         return super().initialize(version, build_data)
 
 
 def _run_clean_command(config):
     from hatchling.metadata.core import ProjectMetadata
     from hatchling.plugin.manager import PluginManager
```

### Comparing `latex_rubber-1.6.4/pyproject.toml` & `latex_rubber-1.6.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -26,16 +26,21 @@
 rubber-pipe = "rubber.cmdline:main_rubber_pipe"
 
 [tool.hatch.version]
 path = "rubber/version.py"
 
 [tool.hatch.build.targets.sdist]
 include = [
+    "*.in",
+    "/man/fr/man1/rubber-pipe.1",
+    "/man/man1/rubber-pipe.1",
     "/misc/zsh-completion",
+    "/NEWS",
     "/rubber",
+    "/tests",
 ]
 
 [tool.hatch.build.targets.wheel]
 packages = ["rubber"]
 
 # These two empty sections enable the custom build hook
 # in file `hatch_build.py`.
```

### Comparing `latex_rubber-1.6.4/PKG-INFO` & `latex_rubber-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: latex-rubber
-Version: 1.6.4
+Version: 1.6.5
 Summary: an automated system for building LaTeX documents
 Project-URL: Homepage, https://gitlab.com/latex-rubber/rubber
 Author-email: Sebastian Kapfer <sebastian.kapfer@fau.de>
 Maintainer-email: Florian Schmaus <flo@geekplace.eu>
 License: GPL-3.0-or-later
 License-File: COPYING
 Requires-Python: >=3.8
```

