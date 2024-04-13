# Comparing `tmp/pylivemaker-1.2.0.tar.gz` & `tmp/pylivemaker-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylivemaker-1.2.0.tar", last modified: Sat Jan 13 12:33:44 2024, max compression
+gzip compressed data, was "pylivemaker-1.2.1.tar", last modified: Sat Apr 13 08:43:55 2024, max compression
```

## Comparing `pylivemaker-1.2.0.tar` & `pylivemaker-1.2.1.tar`

### file list

```diff
@@ -1,344 +1,344 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 12:33:44.339121 pylivemaker-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 12:33:44.283122 pylivemaker-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/.github/labels.yml
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/.github/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/.github/renovate.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 12:33:44.283122 pylivemaker-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/.github/workflows/constraints.txt
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/COPYING
--rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-01-13 12:33:44.339121 pylivemaker-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 12:33:44.287122 pylivemaker-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 12:33:44.279122 pylivemaker-1.2.0/docs/_static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 12:33:44.331122 pylivemaker-1.2.0/docs/_static/LiveNovel/
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/backlogbar.gif
--rw-r--r--   0 runner    (1001) docker     (127)   117925 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/calc.html
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/calccom.html
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/cgchar.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/chartlist.html
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/check.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/command.html
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/cond.html
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/const.html
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/faq_chart.html
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/faq_graphic.html
--rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/faq_project.html
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/faq_text.html
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/faq_var.html
--rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/file.html
--rw-r--r--   0 runner    (1001) docker     (127)   146508 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/graphic.html
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/histbar1.gif
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/histbar2.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/histbar3.gif
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/inptext.html
--rw-r--r--   0 runner    (1001) docker     (127)   155316 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/interface.html
--rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/jump.html
--rw-r--r--   0 runner    (1001) docker     (127)   130761 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_cgmode.png
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_cond01.png
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_cond02.png
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_cond03.png
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_cond04.png
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_cond05.png
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_inptext01.png
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_inptext02.png
--rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_inptext03.png
--rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_inptext04.png
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_inptext05.png
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_inptext06.png
--rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump1.png
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump10.png
--rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump11.png
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump12.png
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump13.png
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump14.png
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump15.png
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump2.png
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump3.png
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump4.png
--rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump5.png
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump6.png
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump7.png
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump8.png
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump9.png
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_number.png
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open01.gif
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open02.gif
--rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open03.gif
--rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open04.gif
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open05.gif
--rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open06.gif
--rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open07.gif
--rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open08.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open09.gif
--rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open10.gif
--rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open11.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open12.gif
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open13.gif
--rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open14.gif
--rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open15.gif
--rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open16.gif
--rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open17.gif
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open18.gif
--rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open20.gif
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open21.gif
--rw-r--r--   0 runner    (1001) docker     (127)    16818 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open22.gif
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open23.gif
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open24.gif
--rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open25.gif
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg01.png
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg02.png
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg03.png
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg04.png
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg05.png
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg06.png
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg07.png
--rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg08.png
--rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg09.png
--rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg10.png
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg11.png
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg12.png
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr01.png
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr02.png
--rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr03.png
--rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr04.png
--rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr05.png
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr06.png
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr07.png
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr08.png
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr09.png
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr10.png
--rw-r--r--   0 runner    (1001) docker     (127)    10138 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr11.png
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr12.png
--rw-r--r--   0 runner    (1001) docker     (127)    17175 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial01.png
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial02.png
--rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial03.png
--rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial04.png
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial05.png
--rw-r--r--   0 runner    (1001) docker     (127)      237 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial06.png
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial07.png
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial08.png
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial09.png
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial10.png
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial11.png
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial12.png
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial13.png
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial14.png
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial15.png
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial16.png
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial17.png
--rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial18.png
--rw-r--r--   0 runner    (1001) docker     (127)    19967 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial19.png
--rw-r--r--   0 runner    (1001) docker     (127)    17388 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial20.png
--rw-r--r--   0 runner    (1001) docker     (127)    19690 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial21.png
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial22.png
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial23.png
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial24.png
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial25.png
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial26.png
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial27.png
--rw-r--r--   0 runner    (1001) docker     (127)    19254 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial28.png
--rw-r--r--   0 runner    (1001) docker     (127)    51466 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial29.png
--rw-r--r--   0 runner    (1001) docker     (127)    23089 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial30.png
--rw-r--r--   0 runner    (1001) docker     (127)    48904 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial31.png
--rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial32.png
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial33.png
--rw-r--r--   0 runner    (1001) docker     (127)    44958 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial34.png
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial35.png
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial36.png
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial37.png
--rw-r--r--   0 runner    (1001) docker     (127)    51498 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial38.png
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial39.png
--rw-r--r--   0 runner    (1001) docker     (127)    51844 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial40.png
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial42.png
--rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial43.png
--rw-r--r--   0 runner    (1001) docker     (127)    45576 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial44.png
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial45.png
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial46.png
--rw-r--r--   0 runner    (1001) docker     (127)    38120 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial47.png
--rw-r--r--   0 runner    (1001) docker     (127)    29402 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial48.png
--rw-r--r--   0 runner    (1001) docker     (127)    27592 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial49.png
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial50.png
--rw-r--r--   0 runner    (1001) docker     (127)    43910 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial54.png
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial55.png
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial56.png
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial57.png
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial58.png
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial59.png
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial61.png
--rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial62.png
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial63.png
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial64.png
--rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial65.png
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial66.png
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial67.png
--rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial68.png
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial69.png
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial70.png
--rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial71.png
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial72.png
--rw-r--r--   0 runner    (1001) docker     (127)    29183 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial73.png
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial74.png
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial75.png
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial76.png
--rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial77.png
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial78.png
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial79.png
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial80.png
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial81.png
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial82.png
--rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial83.png
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial84.png
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial85.png
--rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial86.png
--rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial87.png
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_var01.gif
--rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/ln_var02.gif
--rw-r--r--   0 runner    (1001) docker     (127)    29457 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/media.html
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/menu_chart.html
--rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/menu_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/menu_file.html
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/menu_font.html
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/menu_project.html
--rw-r--r--   0 runner    (1001) docker     (127)    38158 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/menu_scenario.html
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/menu_var.html
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/menu_view.html
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/new.gif
--rw-r--r--   0 runner    (1001) docker     (127)    14364 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/node.html
--rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/object.html
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/openchart.html
--rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/openscenario.html
--rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/optdlg.gif
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/optinptext.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/option.html
--rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/option1.html
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/option10.html
--rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/option11.html
--rw-r--r--   0 runner    (1001) docker     (127)    38169 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/option2.html
--rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/option3.html
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/option4.html
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/option5.html
--rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/option6.html
--rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/option7.html
--rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/option8.html
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/option9.html
--rw-r--r--   0 runner    (1001) docker     (127)      581 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/option_frame.html
--rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/prop.html
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/quake1.gif
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/quake2.gif
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/quake3.gif
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/screen.html
--rw-r--r--   0 runner    (1001) docker     (127)    53897 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/script.html
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/scrollbar.gif
--rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/selimg.html
--rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/selstr.html
--rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/sequence.html
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/slider_bar.gif
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/slider_btn.gif
--rw-r--r--   0 runner    (1001) docker     (127)      998 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/slider_thumb.gif
--rw-r--r--   0 runner    (1001) docker     (127)    80993 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/text.html
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/topics.html
--rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial01.html
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial02.html
--rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial03.html
--rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial04.html
--rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial05.html
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial06.html
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial07.html
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial08.html
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial09.html
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial10.html
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial11.html
--rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial12.html
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial13.html
--rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial14.html
--rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial15.html
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial16.html
--rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial17.html
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial18.html
--rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial19.html
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/var.html
--rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/varlist.html
--rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/_static/LiveNovel/スクリプト例.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)    20008 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/cli.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     4916 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/livemaker.cli.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/livemaker.lsb.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/livemaker.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 12:33:44.331122 pylivemaker-1.2.0/docs/livenovel/
--rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/livenovel/basic.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/livenovel/faq.rst
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/livenovel/tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/livenovel.rst
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-01-13 12:33:44.339121 pylivemaker-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 12:33:44.279122 pylivemaker-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 12:33:44.331122 pylivemaker-1.2.0/src/livemaker/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    19535 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/GalImagePlugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-01-13 12:33:44.000000 pylivemaker-1.2.0/src/livemaker/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    40085 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/archive.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 12:33:44.335121 pylivemaker-1.2.0/src/livemaker/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/cli/lmar.py
--rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/cli/lmgraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/cli/lmlpb.py
--rw-r--r--   0 runner    (1001) docker     (127)    47103 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/cli/lmlsb.py
--rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/cli/lmpatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/lpb.py
--rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/lpm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 12:33:44.335121 pylivemaker-1.2.0/src/livemaker/lsb/
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/lsb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61095 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/lsb/command.py
--rw-r--r--   0 runner    (1001) docker     (127)    33523 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/lsb/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     7347 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/lsb/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    25190 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/lsb/lmscript.py
--rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/lsb/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)    60240 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/lsb/novel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/lsb/translate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/src/livemaker/scramble.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 12:33:44.339121 pylivemaker-1.2.0/src/pylivemaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-01-13 12:33:44.000000 pylivemaker-1.2.0/src/pylivemaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-01-13 12:33:44.000000 pylivemaker-1.2.0/src/pylivemaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-13 12:33:44.000000 pylivemaker-1.2.0/src/pylivemaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-01-13 12:33:44.000000 pylivemaker-1.2.0/src/pylivemaker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-01-13 12:33:44.000000 pylivemaker-1.2.0/src/pylivemaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-01-13 12:33:44.000000 pylivemaker-1.2.0/src/pylivemaker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 12:33:44.335121 pylivemaker-1.2.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-13 12:33:44.339121 pylivemaker-1.2.0/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/tests/data/00000001.lsb
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/tests/data/gamemain.lsb
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/tests/data/live.lpb
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/tests/data/save.dat
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/tests/data/test.dat
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/tests/data/test.exe
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/tests/test_badpadding.py
--rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-01-13 12:33:21.000000 pylivemaker-1.2.0/tests/test_pylivemaker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:55.657197 pylivemaker-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:55.597197 pylivemaker-1.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/.github/labels.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/.github/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/.github/renovate.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:55.597197 pylivemaker-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/.github/workflows/constraints.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3489 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/COPYING
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-13 08:43:55.657197 pylivemaker-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:55.601197 pylivemaker-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:55.593197 pylivemaker-1.2.1/docs/_static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:55.645197 pylivemaker-1.2.1/docs/_static/LiveNovel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/backlogbar.gif
+-rw-r--r--   0 runner    (1001) docker     (127)   117925 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/calc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2600 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/calccom.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/cgchar.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/chartlist.html
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/check.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/command.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/cond.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/const.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/faq_chart.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/faq_graphic.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/faq_project.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/faq_text.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/faq_var.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1410 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/file.html
+-rw-r--r--   0 runner    (1001) docker     (127)   146508 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/graphic.html
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/histbar1.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/histbar2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/histbar3.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/inptext.html
+-rw-r--r--   0 runner    (1001) docker     (127)   155316 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/interface.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6993 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/jump.html
+-rw-r--r--   0 runner    (1001) docker     (127)   130761 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_cgmode.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_cond01.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_cond02.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_cond03.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_cond04.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_cond05.png
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_inptext01.png
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_inptext02.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7822 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_inptext03.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5408 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_inptext04.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_inptext05.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_inptext06.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump10.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2787 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump11.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump12.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump13.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump14.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump15.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump2.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump4.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3683 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump5.png
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump6.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump7.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump8.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump9.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_number.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open01.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open02.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4031 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open03.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     6720 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open04.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open05.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open06.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4561 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open07.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     5696 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open08.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7081 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open09.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open10.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open11.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7401 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open12.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open13.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     8916 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open14.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4968 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open15.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    10262 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open16.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open17.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open18.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open20.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open21.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    16818 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open22.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open23.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open24.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open25.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg01.png
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg02.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg03.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg04.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg05.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg06.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg07.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3082 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg08.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg09.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3929 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg10.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg11.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr01.png
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr02.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr03.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5248 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr04.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr05.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr06.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr07.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr08.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr09.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr10.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10138 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr11.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr12.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17175 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial01.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial02.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6261 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial03.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4668 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial04.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial05.png
+-rw-r--r--   0 runner    (1001) docker     (127)      237 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial06.png
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial07.png
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial08.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial09.png
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial10.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial11.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial12.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial13.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial14.png
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial15.png
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial16.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial17.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4427 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial18.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19967 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial19.png
+-rw-r--r--   0 runner    (1001) docker     (127)    17388 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial20.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19690 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial21.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial22.png
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial23.png
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial24.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial25.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial26.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial27.png
+-rw-r--r--   0 runner    (1001) docker     (127)    19254 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial28.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51466 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial29.png
+-rw-r--r--   0 runner    (1001) docker     (127)    23089 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial30.png
+-rw-r--r--   0 runner    (1001) docker     (127)    48904 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial31.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial32.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial33.png
+-rw-r--r--   0 runner    (1001) docker     (127)    44958 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial34.png
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial35.png
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial36.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial37.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51498 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial38.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial39.png
+-rw-r--r--   0 runner    (1001) docker     (127)    51844 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial40.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial42.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial43.png
+-rw-r--r--   0 runner    (1001) docker     (127)    45576 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial44.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial45.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial46.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38120 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial47.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29402 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial48.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27592 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial49.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial50.png
+-rw-r--r--   0 runner    (1001) docker     (127)    43910 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial54.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial55.png
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial56.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial57.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial58.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial59.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial61.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6441 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial62.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial63.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial64.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1104 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial65.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial66.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial67.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2134 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial68.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial69.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial70.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4347 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial71.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial72.png
+-rw-r--r--   0 runner    (1001) docker     (127)    29183 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial73.png
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial74.png
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial75.png
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial76.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5700 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial77.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial78.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial79.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial80.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial81.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial82.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7628 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial83.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial84.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2652 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial85.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial86.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial87.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_var01.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     6820 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/ln_var02.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    29457 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/media.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/menu_chart.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/menu_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7845 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/menu_file.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/menu_font.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/menu_project.html
+-rw-r--r--   0 runner    (1001) docker     (127)    38158 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/menu_scenario.html
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/menu_var.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/menu_view.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/new.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    14364 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/node.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8688 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/object.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/openchart.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/openscenario.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3306 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/optdlg.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/optinptext.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/option.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11667 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/option1.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/option10.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2646 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/option11.html
+-rw-r--r--   0 runner    (1001) docker     (127)    38169 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/option2.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14212 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/option3.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/option4.html
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/option5.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5491 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/option6.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6067 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/option7.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11345 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/option8.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/option9.html
+-rw-r--r--   0 runner    (1001) docker     (127)      581 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/option_frame.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/prop.html
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/quake1.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/quake2.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/quake3.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/screen.html
+-rw-r--r--   0 runner    (1001) docker     (127)    53897 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/script.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/scrollbar.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    12085 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/selimg.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9523 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/selstr.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14793 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/sequence.html
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/slider_bar.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/slider_btn.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/slider_thumb.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    80993 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/text.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/topics.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5484 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial01.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial02.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2532 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial03.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial04.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2971 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial05.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial06.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial07.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial08.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial09.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial10.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial11.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5329 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial12.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial13.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial14.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7230 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial15.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial16.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4661 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial17.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial18.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5754 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial19.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/var.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4333 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/varlist.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4667 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/_static/LiveNovel/スクリプト例.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    20008 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/cli.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4916 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/livemaker.cli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/livemaker.lsb.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/livemaker.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:55.649197 pylivemaker-1.2.1/docs/livenovel/
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/livenovel/basic.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/livenovel/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/livenovel/tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/livenovel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7266 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-13 08:43:55.657197 pylivemaker-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:55.593197 pylivemaker-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:55.649197 pylivemaker-1.2.1/src/livemaker/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    19554 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/GalImagePlugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-13 08:43:55.000000 pylivemaker-1.2.1/src/livemaker/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40085 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/archive.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:55.649197 pylivemaker-1.2.1/src/livemaker/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3972 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5450 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/cli/lmar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6454 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/cli/lmgraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4169 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/cli/lmlpb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47103 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/cli/lmlsb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7203 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/cli/lmpatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1777 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7004 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/lpb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6688 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/lpm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:55.653197 pylivemaker-1.2.1/src/livemaker/lsb/
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/lsb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61095 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/lsb/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33523 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/lsb/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7347 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/lsb/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25190 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/lsb/lmscript.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15627 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/lsb/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60240 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/lsb/novel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/lsb/translate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3876 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/src/livemaker/scramble.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:55.653197 pylivemaker-1.2.1/src/pylivemaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3946 2024-04-13 08:43:55.000000 pylivemaker-1.2.1/src/pylivemaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11438 2024-04-13 08:43:55.000000 pylivemaker-1.2.1/src/pylivemaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 08:43:55.000000 pylivemaker-1.2.1/src/pylivemaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-13 08:43:55.000000 pylivemaker-1.2.1/src/pylivemaker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-13 08:43:55.000000 pylivemaker-1.2.1/src/pylivemaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 08:43:55.000000 pylivemaker-1.2.1/src/pylivemaker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:55.653197 pylivemaker-1.2.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:55.653197 pylivemaker-1.2.1/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     4138 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/tests/data/00000001.lsb
+-rw-r--r--   0 runner    (1001) docker     (127)     3071 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/tests/data/gamemain.lsb
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/tests/data/live.lpb
+-rw-r--r--   0 runner    (1001) docker     (127)      431 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/tests/data/save.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/tests/data/test.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/tests/data/test.exe
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/tests/test_badpadding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-04-13 08:43:36.000000 pylivemaker-1.2.1/tests/test_pylivemaker.py
```

### Comparing `pylivemaker-1.2.0/.github/labels.yml` & `pylivemaker-1.2.1/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/.github/release-drafter.yml` & `pylivemaker-1.2.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/.github/workflows/release.yml` & `pylivemaker-1.2.1/.github/workflows/release.yml`

 * *Files 13% similar despite different names*

```diff
@@ -35,14 +35,14 @@
 
       - name: Build package
         run: |
           python -m build
 
       - name: Publish package on PyPI
         if: ${{ github.event_name == 'release' }}
-        uses: pypa/gh-action-pypi-publish@v1.8.11
+        uses: pypa/gh-action-pypi-publish@v1.8.14
 
       - name: Publish package on TestPyPI
         if: ${{ github.event_name != 'release' }}
-        uses: pypa/gh-action-pypi-publish@v1.8.11
+        uses: pypa/gh-action-pypi-publish@v1.8.14
         with:
           repository_url: https://test.pypi.org/legacy/
```

### Comparing `pylivemaker-1.2.0/.github/workflows/tests.yml` & `pylivemaker-1.2.1/.github/workflows/tests.yml`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
           pip install --constraint=.github/workflows/constraints.txt .[test]
 
       - name: Run tests
         run: |
           pytest --cov=livemaker --cov-report=xml --cov-report=term
 
       - name: Upload coverage data
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v4
         with:
           files: ./coverage.xml
```

### Comparing `pylivemaker-1.2.0/.gitignore` & `pylivemaker-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/.pre-commit-config.yaml` & `pylivemaker-1.2.1/.pre-commit-config.yaml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # See https://pre-commit.com for more information
 # See https://pre-commit.com/hooks.html for more hooks
 repos:
   - repo: https://github.com/psf/black
-    rev: 23.10.1
+    rev: 24.3.0
     hooks:
       - id: black
         language_version: python3
         files: .
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-toml
   - repo: https://github.com/PyCQA/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
       - id: flake8
         language_version: python3
         additional_dependencies:
           - flake8-comprehensions
   - hooks:
       - id: isort
         language_version: python3
     repo: https://github.com/timothycrosley/isort
-    rev: 5.12.0
+    rev: 5.13.2
```

### Comparing `pylivemaker-1.2.0/CONTRIBUTING.rst` & `pylivemaker-1.2.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/COPYING` & `pylivemaker-1.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/HISTORY.rst` & `pylivemaker-1.2.1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/Makefile` & `pylivemaker-1.2.1/Makefile`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/PKG-INFO` & `pylivemaker-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylivemaker
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python package for manipulating LiveMaker game resources.
 Author: tinfoil
 Author-email: Peter Rowlands <peter@pmrowla.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: documentation, https://pylivemaker.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/pmrowla/pylivemaker
 Project-URL: changelog, https://github.com/pmrowla/pylivemaker/blob/master/HISTORY.rst
```

### Comparing `pylivemaker-1.2.0/README.rst` & `pylivemaker-1.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/Makefile` & `pylivemaker-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/backlogbar.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/backlogbar.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/calc.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/calc.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/calccom.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/calccom.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/cgchar.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/cgchar.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/chartlist.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/chartlist.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/check.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/check.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/command.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/command.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/cond.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/cond.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/const.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/const.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/faq_chart.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/faq_chart.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/faq_graphic.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/faq_graphic.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/faq_project.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/faq_project.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/faq_text.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/faq_text.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/faq_var.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/faq_var.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/file.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/file.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/graphic.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/graphic.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/histbar1.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/histbar1.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/histbar2.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/histbar2.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/histbar3.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/histbar3.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/index.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/index.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/inptext.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/inptext.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/interface.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/interface.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/jump.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/jump.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_cgmode.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_cgmode.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_cond01.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_cond01.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_cond02.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_cond02.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_cond03.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_cond03.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_cond04.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_cond04.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_cond05.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_cond05.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_inptext01.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_inptext01.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_inptext02.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_inptext02.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_inptext03.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_inptext03.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_inptext04.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_inptext04.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_inptext05.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_inptext05.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_inptext06.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_inptext06.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump1.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump1.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump10.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump10.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump11.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump11.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump12.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump12.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump13.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump13.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump14.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump14.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump15.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump15.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump2.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump2.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump3.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump3.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump4.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump4.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump5.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump5.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump6.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump6.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump7.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump7.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump8.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump8.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_jump9.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_jump9.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_number.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_number.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open01.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open01.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open02.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open02.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open03.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open03.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open04.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open04.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open05.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open05.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open06.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open06.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open07.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open07.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open08.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open08.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open09.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open09.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open10.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open10.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open11.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open11.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open12.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open12.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open13.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open13.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open14.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open14.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open15.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open15.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open16.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open16.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open17.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open17.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open18.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open18.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open20.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open20.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open21.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open21.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open22.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open22.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open23.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open23.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open24.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open24.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_open25.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_open25.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg01.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg01.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg02.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg02.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg03.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg03.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg04.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg04.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg05.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg05.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg06.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg06.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg07.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg07.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg08.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg08.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg09.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg09.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg10.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg10.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg11.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg11.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selimg12.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selimg12.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr01.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr01.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr02.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr02.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr03.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr03.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr04.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr04.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr05.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr05.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr06.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr06.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr07.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr07.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr08.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr08.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr09.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr09.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr10.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr10.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr11.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr11.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_selstr12.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_selstr12.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial01.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial01.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial02.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial02.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial03.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial03.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial04.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial04.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial05.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial05.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial08.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial08.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial09.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial09.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial10.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial10.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial11.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial11.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial12.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial12.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial13.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial13.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial14.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial14.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial15.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial15.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial16.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial16.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial17.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial17.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial18.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial18.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial19.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial19.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial20.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial20.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial21.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial21.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial22.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial22.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial23.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial23.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial24.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial24.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial25.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial25.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial26.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial26.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial27.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial27.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial28.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial28.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial29.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial29.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial30.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial30.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial31.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial31.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial32.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial32.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial33.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial33.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial34.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial34.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial35.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial35.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial36.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial36.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial37.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial37.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial38.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial38.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial39.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial39.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial40.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial40.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial42.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial42.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial43.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial43.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial44.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial44.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial45.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial45.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial46.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial46.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial47.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial47.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial48.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial48.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial49.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial49.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial50.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial50.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial54.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial54.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial55.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial55.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial56.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial56.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial57.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial57.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial58.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial58.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial59.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial59.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial61.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial61.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial62.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial62.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial63.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial63.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial64.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial64.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial65.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial65.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial66.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial66.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial67.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial67.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial68.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial68.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial69.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial69.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial70.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial70.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial71.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial71.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial72.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial72.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial73.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial73.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial76.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial76.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial77.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial77.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial78.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial78.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial79.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial79.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial80.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial80.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial81.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial81.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial82.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial82.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial83.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial83.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial84.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial84.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial85.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial85.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial86.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial86.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_turorial87.png` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_turorial87.png`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_var01.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_var01.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/ln_var02.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/ln_var02.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/media.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/media.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/menu_chart.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/menu_chart.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/menu_edit.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/menu_edit.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/menu_file.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/menu_file.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/menu_font.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/menu_font.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/menu_project.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/menu_project.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/menu_scenario.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/menu_scenario.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/menu_var.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/menu_var.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/menu_view.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/menu_view.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/new.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/new.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/node.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/node.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/object.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/object.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/openchart.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/openchart.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/openscenario.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/openscenario.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/optdlg.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/optdlg.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/optinptext.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/optinptext.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/option.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/option.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/option1.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/option1.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/option10.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/option10.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/option11.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/option11.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/option2.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/option2.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/option3.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/option3.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/option4.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/option4.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/option5.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/option5.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/option6.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/option6.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/option7.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/option7.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/option8.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/option8.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/option9.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/option9.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/option_frame.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/option_frame.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/prop.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/prop.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/quake1.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/quake1.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/quake2.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/quake2.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/quake3.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/quake3.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/screen.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/screen.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/script.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/script.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/scrollbar.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/scrollbar.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/selimg.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/selimg.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/selstr.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/selstr.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/sequence.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/sequence.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/slider_bar.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/slider_bar.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/slider_btn.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/slider_btn.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/slider_thumb.gif` & `pylivemaker-1.2.1/docs/_static/LiveNovel/slider_thumb.gif`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/text.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/text.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/topics.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/topics.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial01.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial01.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial02.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial02.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial03.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial03.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial04.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial04.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial05.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial05.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial06.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial06.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial07.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial07.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial08.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial08.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial09.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial09.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial10.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial10.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial11.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial11.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial12.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial12.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial13.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial13.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial14.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial14.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial15.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial15.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial16.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial16.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial17.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial17.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial18.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial18.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/tutorial19.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/tutorial19.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/var.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/var.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/varlist.html` & `pylivemaker-1.2.1/docs/_static/LiveNovel/varlist.html`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/_static/LiveNovel/スクリプト例.txt` & `pylivemaker-1.2.1/docs/_static/LiveNovel/スクリプト例.txt`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/cli.rst` & `pylivemaker-1.2.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/conf.py` & `pylivemaker-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/installation.rst` & `pylivemaker-1.2.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/livemaker.cli.rst` & `pylivemaker-1.2.1/docs/livemaker.cli.rst`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/livemaker.lsb.rst` & `pylivemaker-1.2.1/docs/livemaker.lsb.rst`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/livemaker.rst` & `pylivemaker-1.2.1/docs/livemaker.rst`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/livenovel/basic.rst` & `pylivemaker-1.2.1/docs/livenovel/basic.rst`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/livenovel/faq.rst` & `pylivemaker-1.2.1/docs/livenovel/faq.rst`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/livenovel/tutorial.rst` & `pylivemaker-1.2.1/docs/livenovel/tutorial.rst`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/livenovel.rst` & `pylivemaker-1.2.1/docs/livenovel.rst`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/make.bat` & `pylivemaker-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/docs/usage.rst` & `pylivemaker-1.2.1/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/pyproject.toml` & `pylivemaker-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/GalImagePlugin.py` & `pylivemaker-1.2.1/src/livemaker/GalImagePlugin.py`

 * *Files 0% similar despite different names*

```diff
@@ -296,14 +296,15 @@
 
         i = 0
         for name, layer_count, mode, layermode, rawmode, box, palette in frames:
             tile = None
             offset = offsets[i]
             tile = [(self.decoder, box, offset, (info, layermode, rawmode, i))]
             frames[i] = name, mode, box, palette, tile
+            i += 1
         self.fp.seek(info["offset"])
         self.frames = frames
         self._frame = None
         self.seek(0)
 
     @property
     def is_animated(self):
```

### Comparing `pylivemaker-1.2.0/src/livemaker/__init__.py` & `pylivemaker-1.2.1/src/livemaker/__init__.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/archive.py` & `pylivemaker-1.2.1/src/livemaker/archive.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/cli/__init__.py` & `pylivemaker-1.2.1/src/livemaker/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/cli/cli.py` & `pylivemaker-1.2.1/src/livemaker/cli/cli.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/cli/lmar.py` & `pylivemaker-1.2.1/src/livemaker/cli/lmar.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/cli/lmgraph.py` & `pylivemaker-1.2.1/src/livemaker/cli/lmgraph.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/cli/lmlpb.py` & `pylivemaker-1.2.1/src/livemaker/cli/lmlpb.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/cli/lmlsb.py` & `pylivemaker-1.2.1/src/livemaker/cli/lmlsb.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/cli/lmpatch.py` & `pylivemaker-1.2.1/src/livemaker/cli/lmpatch.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/exceptions.py` & `pylivemaker-1.2.1/src/livemaker/exceptions.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/lpb.py` & `pylivemaker-1.2.1/src/livemaker/lpb.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/lpm.py` & `pylivemaker-1.2.1/src/livemaker/lpm.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/lsb/__init__.py` & `pylivemaker-1.2.1/src/livemaker/lsb/__init__.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/lsb/command.py` & `pylivemaker-1.2.1/src/livemaker/lsb/command.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/lsb/core.py` & `pylivemaker-1.2.1/src/livemaker/lsb/core.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/lsb/graph.py` & `pylivemaker-1.2.1/src/livemaker/lsb/graph.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/lsb/lmscript.py` & `pylivemaker-1.2.1/src/livemaker/lsb/lmscript.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/lsb/menu.py` & `pylivemaker-1.2.1/src/livemaker/lsb/menu.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/lsb/novel.py` & `pylivemaker-1.2.1/src/livemaker/lsb/novel.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/lsb/translate.py` & `pylivemaker-1.2.1/src/livemaker/lsb/translate.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/project.py` & `pylivemaker-1.2.1/src/livemaker/project.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/livemaker/scramble.py` & `pylivemaker-1.2.1/src/livemaker/scramble.py`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/src/pylivemaker.egg-info/PKG-INFO` & `pylivemaker-1.2.1/src/pylivemaker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pylivemaker
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python package for manipulating LiveMaker game resources.
 Author: tinfoil
 Author-email: Peter Rowlands <peter@pmrowla.com>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: documentation, https://pylivemaker.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/pmrowla/pylivemaker
 Project-URL: changelog, https://github.com/pmrowla/pylivemaker/blob/master/HISTORY.rst
```

### Comparing `pylivemaker-1.2.0/src/pylivemaker.egg-info/SOURCES.txt` & `pylivemaker-1.2.1/src/pylivemaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/tests/data/00000001.lsb` & `pylivemaker-1.2.1/tests/data/00000001.lsb`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/tests/data/gamemain.lsb` & `pylivemaker-1.2.1/tests/data/gamemain.lsb`

 * *Files identical despite different names*

### Comparing `pylivemaker-1.2.0/tests/test_pylivemaker.py` & `pylivemaker-1.2.1/tests/test_pylivemaker.py`

 * *Files identical despite different names*

