# Comparing `tmp/musical_games-0.5.2.tar.gz` & `tmp/musical_games-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "musical_games-0.5.2.tar", last modified: Tue Feb 15 13:40:26 2022, max compression
+gzip compressed data, was "musical_games-0.6.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `musical_games-0.5.2.tar` & `musical_games-0.6.1.tar`

### file list

```diff
@@ -1,111 +1,91 @@
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.626608 musical_games-0.5.2/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     7707 2016-07-03 13:55:58.000000 musical_games-0.5.2/LICENSE
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      244 2021-11-21 14:25:44.000000 musical_games-0.5.2/MANIFEST.in
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1138 2022-02-15 13:40:26.626608 musical_games-0.5.2/PKG-INFO
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      343 2019-04-02 11:33:52.000000 musical_games-0.5.2/README.rst
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.618608 musical_games-0.5.2/docs/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     6790 2016-07-03 13:55:58.000000 musical_games-0.5.2/docs/Makefile
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      154 2018-08-01 14:00:31.000000 musical_games-0.5.2/docs/authors.rst
--rwxrwxr-x   0 robbert   (1000) robbert   (1000)     7987 2018-08-01 14:02:02.000000 musical_games-0.5.2/docs/conf.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     3219 2018-08-01 14:00:31.000000 musical_games-0.5.2/docs/contributing.rst
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      119 2018-08-01 14:00:31.000000 musical_games-0.5.2/docs/history.rst
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      516 2018-08-01 14:00:31.000000 musical_games-0.5.2/docs/index.rst
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      209 2018-08-01 14:00:31.000000 musical_games-0.5.2/docs/installation.rst
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     6473 2016-07-03 13:55:58.000000 musical_games-0.5.2/docs/make.bat
--rw-rw-r--   0 robbert   (1000) robbert   (1000)       76 2018-08-01 14:00:31.000000 musical_games-0.5.2/docs/modules.rst
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      962 2018-08-01 14:00:31.000000 musical_games-0.5.2/docs/musical_games.converters.rst
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1387 2018-08-01 14:00:31.000000 musical_games-0.5.2/docs/musical_games.dice_games.lilypond.rst
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1276 2018-08-01 14:00:31.000000 musical_games-0.5.2/docs/musical_games.dice_games.rst
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      749 2018-08-01 14:00:31.000000 musical_games-0.5.2/docs/musical_games.rst
--rw-rw-r--   0 robbert   (1000) robbert   (1000)       27 2018-08-01 14:00:31.000000 musical_games-0.5.2/docs/readme.rst
--rw-rw-r--   0 robbert   (1000) robbert   (1000)       87 2018-08-01 14:00:31.000000 musical_games-0.5.2/docs/usage.rst
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.618608 musical_games-0.5.2/musical_games/
--rwxrwxr-x   0 robbert   (1000) robbert   (1000)      216 2021-11-27 09:11:05.000000 musical_games-0.5.2/musical_games/__init__.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      362 2022-02-15 13:40:22.000000 musical_games-0.5.2/musical_games/__version__.py
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.618608 musical_games-0.5.2/musical_games/data/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      140 2021-03-09 13:25:57.000000 musical_games-0.5.2/musical_games/data/__init__.py
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.618608 musical_games-0.5.2/musical_games/data/dice_games/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      140 2021-11-21 15:05:23.000000 musical_games-0.5.2/musical_games/data/dice_games/__init__.py
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.618608 musical_games-0.5.2/musical_games/data/dice_games/cpe_bach_counterpoint/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      140 2021-03-09 13:25:57.000000 musical_games-0.5.2/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     5833 2022-01-05 17:00:12.000000 musical_games-0.5.2/musical_games/data/dice_games/cpe_bach_counterpoint/config.yaml
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.618608 musical_games-0.5.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1410 2022-01-05 17:18:42.000000 musical_games-0.5.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1773 2022-01-08 12:37:19.000000 musical_games-0.5.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     2819 2022-01-08 12:39:01.000000 musical_games-0.5.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      750 2022-01-05 17:08:44.000000 musical_games-0.5.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.618608 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      140 2021-03-09 13:25:57.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)    25330 2022-01-08 12:41:21.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/config.yaml
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.618608 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     2443 2022-01-08 12:41:45.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     6621 2022-01-08 12:48:36.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     4259 2022-01-08 12:45:27.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1192 2022-01-08 12:42:30.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.618608 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.610608 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.622608 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     3901 2016-07-03 13:55:58.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     2059 2016-07-03 13:55:58.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      154 2021-03-10 10:23:16.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.610608 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.622608 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     9117 2016-07-03 13:55:58.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     2453 2016-07-03 13:55:58.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.622608 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_polonaise/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      140 2021-03-10 10:43:40.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)    47125 2022-02-12 14:39:12.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_polonaise/config.yaml
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.622608 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     2835 2022-01-08 12:52:46.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     4472 2022-01-08 13:05:24.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     3631 2022-01-08 13:21:18.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1651 2022-01-08 12:53:31.000000 musical_games-0.5.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.622608 musical_games-0.5.2/musical_games/data/dice_games/mozart_waltz/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      140 2021-03-12 08:34:24.000000 musical_games-0.5.2/musical_games/data/dice_games/mozart_waltz/__init__.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)    20487 2022-02-15 13:39:35.000000 musical_games-0.5.2/musical_games/data/dice_games/mozart_waltz/config.yaml
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.622608 musical_games-0.5.2/musical_games/data/dice_games/mozart_waltz/lilypond/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1702 2022-01-08 13:15:40.000000 musical_games-0.5.2/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     2869 2022-01-08 13:28:11.000000 musical_games-0.5.2/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     3905 2022-01-08 13:23:54.000000 musical_games-0.5.2/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1268 2022-01-08 13:16:33.000000 musical_games-0.5.2/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.622608 musical_games-0.5.2/musical_games/data/dice_games/stadler_menuet_trio/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      140 2021-11-21 15:05:19.000000 musical_games-0.5.2/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)    33572 2022-01-08 13:46:05.000000 musical_games-0.5.2/musical_games/data/dice_games/stadler_menuet_trio/config.yaml
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.622608 musical_games-0.5.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     2462 2022-01-08 13:32:08.000000 musical_games-0.5.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     6621 2022-01-08 13:42:37.000000 musical_games-0.5.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     4361 2022-01-08 13:37:58.000000 musical_games-0.5.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1192 2022-01-08 13:33:19.000000 musical_games-0.5.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.626608 musical_games-0.5.2/musical_games/dice_games/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      140 2022-01-03 14:06:10.000000 musical_games-0.5.2/musical_games/dice_games/__init__.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     6212 2022-01-16 15:55:02.000000 musical_games-0.5.2/musical_games/dice_games/dice_games.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     8481 2022-01-15 12:46:25.000000 musical_games-0.5.2/musical_games/dice_games/game_mechanics.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     8658 2022-01-15 12:28:05.000000 musical_games-0.5.2/musical_games/dice_games/typesetting.py
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.626608 musical_games-0.5.2/musical_games/lib/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      138 2018-08-01 14:02:02.000000 musical_games-0.5.2/musical_games/lib/__init__.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     5138 2022-02-12 14:43:54.000000 musical_games-0.5.2/musical_games/lib/audio.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1920 2022-01-08 13:45:26.000000 musical_games-0.5.2/musical_games/lib/images.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     3033 2022-02-14 09:08:45.000000 musical_games-0.5.2/musical_games/lib/lilypond.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1878 2022-02-12 14:14:21.000000 musical_games-0.5.2/musical_games/lib/utils.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     4353 2022-01-08 13:45:26.000000 musical_games-0.5.2/musical_games/utils.py
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.618608 musical_games-0.5.2/musical_games.egg-info/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1138 2022-02-15 13:40:26.000000 musical_games-0.5.2/musical_games.egg-info/PKG-INFO
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     3946 2022-02-15 13:40:26.000000 musical_games-0.5.2/musical_games.egg-info/SOURCES.txt
--rw-rw-r--   0 robbert   (1000) robbert   (1000)        1 2022-02-15 13:40:26.000000 musical_games-0.5.2/musical_games.egg-info/dependency_links.txt
--rw-rw-r--   0 robbert   (1000) robbert   (1000)        1 2022-02-15 13:40:26.000000 musical_games-0.5.2/musical_games.egg-info/not-zip-safe
--rw-rw-r--   0 robbert   (1000) robbert   (1000)       41 2022-02-15 13:40:26.000000 musical_games-0.5.2/musical_games.egg-info/requires.txt
--rw-rw-r--   0 robbert   (1000) robbert   (1000)       28 2022-02-15 13:40:26.000000 musical_games-0.5.2/musical_games.egg-info/top_level.txt
--rw-rw-r--   0 robbert   (1000) robbert   (1000)       41 2021-11-21 14:27:49.000000 musical_games-0.5.2/requirements.txt
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.626608 musical_games-0.5.2/scripts/
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      138 2018-08-01 14:02:02.000000 musical_games-0.5.2/scripts/__init__.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)      764 2021-03-30 08:44:45.000000 musical_games-0.5.2/scripts/change_layout.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1627 2022-01-05 17:23:25.000000 musical_games-0.5.2/scripts/cpe_bach_test.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1636 2022-01-08 12:49:13.000000 musical_games-0.5.2/scripts/kirnberger_meneut_trio.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1533 2022-01-08 13:13:45.000000 musical_games-0.5.2/scripts/kirnberger_polonaise.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1506 2022-01-08 13:29:21.000000 musical_games-0.5.2/scripts/mozart_waltz.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1679 2022-01-08 13:45:26.000000 musical_games-0.5.2/scripts/stadler_meneut_trio.py
--rw-rw-r--   0 robbert   (1000) robbert   (1000)       38 2022-02-15 13:40:26.626608 musical_games-0.5.2/setup.cfg
--rw-rw-r--   0 robbert   (1000) robbert   (1000)     1689 2021-11-27 08:46:13.000000 musical_games-0.5.2/setup.py
-drwxrwxr-x   0 robbert   (1000) robbert   (1000)        0 2022-02-15 13:40:26.626608 musical_games-0.5.2/tests/
--rwxrwxr-x   0 robbert   (1000) robbert   (1000)       24 2018-08-01 14:02:02.000000 musical_games-0.5.2/tests/__init__.py
--rwxrwxr-x   0 robbert   (1000) robbert   (1000)      368 2018-08-01 14:02:02.000000 musical_games-0.5.2/tests/test_dice_games.py
+-rw-r--r--   0        0        0      511 2024-04-07 08:37:11.575406 musical_games-0.6.1/.coveragerc
+-rw-r--r--   0        0        0      292 2016-07-03 13:55:58.881844 musical_games-0.6.1/.editorconfig
+-rw-r--r--   0        0        0    10359 2024-04-07 08:37:38.227407 musical_games-0.6.1/.gitchangelog.rc
+-rw-r--r--   0        0        0      271 2018-09-16 09:02:35.270504 musical_games-0.6.1/.gitchangelog.tpl
+-rw-r--r--   0        0        0     1166 2024-04-07 08:37:55.851407 musical_games-0.6.1/.gitignore
+-rw-r--r--   0        0        0      419 2024-04-07 08:38:05.135407 musical_games-0.6.1/.travis.yml
+-rw-r--r--   0        0        0      804 2024-04-13 15:07:12.503552 musical_games-0.6.1/CHANGELOG.rst
+-rw-r--r--   0        0        0     7707 2016-07-03 13:55:58.881844 musical_games-0.6.1/LICENSE
+-rw-r--r--   0        0        0     4770 2024-04-13 15:08:13.743551 musical_games-0.6.1/Makefile
+-rw-r--r--   0        0        0     3103 2024-04-13 13:04:50.799749 musical_games-0.6.1/README.rst
+-rw-r--r--   0        0        0     6790 2016-07-03 13:55:58.881844 musical_games-0.6.1/docs/Makefile
+-rw-r--r--   0        0        0      154 2018-08-01 14:00:31.251630 musical_games-0.6.1/docs/authors.rst
+-rwxr-xr-x   0        0        0     7987 2024-04-09 10:08:14.002483 musical_games-0.6.1/docs/conf.py
+-rw-r--r--   0        0        0     3219 2018-08-01 14:00:31.247630 musical_games-0.6.1/docs/contributing.rst
+-rw-r--r--   0        0        0      119 2018-08-01 14:00:31.251630 musical_games-0.6.1/docs/history.rst
+-rw-r--r--   0        0        0      516 2018-08-01 14:00:31.247630 musical_games-0.6.1/docs/index.rst
+-rw-r--r--   0        0        0      209 2018-08-01 14:00:31.247630 musical_games-0.6.1/docs/installation.rst
+-rw-r--r--   0        0        0     6473 2016-07-03 13:55:58.881844 musical_games-0.6.1/docs/make.bat
+-rw-r--r--   0        0        0       76 2018-08-01 14:00:31.247630 musical_games-0.6.1/docs/modules.rst
+-rw-r--r--   0        0        0      962 2018-08-01 14:00:31.251630 musical_games-0.6.1/docs/musical_games.converters.rst
+-rw-r--r--   0        0        0     1387 2018-08-01 14:00:31.247630 musical_games-0.6.1/docs/musical_games.dice_games.lilypond.rst
+-rw-r--r--   0        0        0     1276 2018-08-01 14:00:31.247630 musical_games-0.6.1/docs/musical_games.dice_games.rst
+-rw-r--r--   0        0        0      749 2018-08-01 14:00:31.247630 musical_games-0.6.1/docs/musical_games.rst
+-rw-r--r--   0        0        0       27 2018-08-01 14:00:31.247630 musical_games-0.6.1/docs/readme.rst
+-rw-r--r--   0        0        0       87 2018-08-01 14:00:31.247630 musical_games-0.6.1/docs/usage.rst
+-rwxr-xr-x   0        0        0      191 2024-04-09 10:08:14.006483 musical_games-0.6.1/musical_games/__init__.py
+-rw-r--r--   0        0        0      518 2024-04-09 10:08:14.002483 musical_games-0.6.1/musical_games/__version__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.6.1/musical_games/data/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 14:44:21.674751 musical_games-0.6.1/musical_games/data/dice_games/__init__.py
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.6.1/musical_games/data/dice_games/cpe_bach_counterpoint/__init__.py
+-rw-r--r--   0        0        0     2435 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars.csv
+-rw-r--r--   0        0        0      882 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_bass.csv
+-rw-r--r--   0        0        0     1407 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/cpe_bach_counterpoint/bars_treble.csv
+-rw-r--r--   0        0        0     1427 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     1774 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     2747 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0      525 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/single_bar.ly
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2516 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6431 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4063 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1184 2024-04-13 12:50:48.939772 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     5346 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     3901 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt
+-rw-r--r--   0        0        0     2059 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt
+-rw-r--r--   0        0        0      154 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/readme
+-rw-r--r--   0        0        0     9117 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt
+-rw-r--r--   0        0        0     2453 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt
+-rw-r--r--   0        0        0    10956 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_polonaise/__init__.py
+-rw-r--r--   0        0        0     2868 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     4351 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3533 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1635 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly
+-rw-r--r--   0        0        0    32523 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/kirnberger_polonaise/polonaise_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/mozart_waltz/__init__.py
+-rw-r--r--   0        0        0     1800 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     2714 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     3713 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1258 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/mozart_waltz/lilypond/single_bar.ly
+-rw-r--r--   0        0        0     9516 2024-04-13 12:41:41.563787 musical_games-0.6.1/musical_games/data/dice_games/mozart_waltz/waltz_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-09 10:08:14.006483 musical_games-0.6.1/musical_games/data/dice_games/stadler_menuet_trio/__init__.py
+-rw-r--r--   0        0        0     2535 2024-04-13 12:49:58.583773 musical_games-0.6.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly
+-rw-r--r--   0        0        0     6431 2024-04-13 12:57:29.887761 musical_games-0.6.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly
+-rw-r--r--   0        0        0     4166 2024-04-13 12:54:59.155765 musical_games-0.6.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly
+-rw-r--r--   0        0        0     1184 2024-04-13 12:51:21.251771 musical_games-0.6.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly
+-rw-r--r--   0        0        0    13676 2024-04-13 12:47:13.523778 musical_games-0.6.1/musical_games/data/dice_games/stadler_menuet_trio/menuet_bars.csv
+-rw-r--r--   0        0        0     7653 2024-04-13 12:47:50.671777 musical_games-0.6.1/musical_games/data/dice_games/stadler_menuet_trio/trio_bars.csv
+-rw-r--r--   0        0        0      140 2024-04-09 12:20:58.102612 musical_games-0.6.1/musical_games/dice_games/__init__.py
+-rw-r--r--   0        0        0    34408 2024-04-13 14:28:04.919615 musical_games-0.6.1/musical_games/dice_games/base.py
+-rw-r--r--   0        0        0     2614 2024-04-13 13:00:55.979755 musical_games-0.6.1/musical_games/dice_games/data_csv.py
+-rw-r--r--   0        0        0    13161 2024-04-13 13:40:32.743692 musical_games-0.6.1/musical_games/dice_games/dice_games.py
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.006483 musical_games-0.6.1/musical_games/external/__init__.py
+-rw-r--r--   0        0        0     2969 2024-04-09 10:08:14.006483 musical_games-0.6.1/musical_games/external/base.py
+-rw-r--r--   0        0        0      411 2024-04-09 10:08:14.006483 musical_games-0.6.1/musical_games/external/exceptions.py
+-rw-r--r--   0        0        0      972 2024-04-09 10:08:14.006483 musical_games-0.6.1/musical_games/external/images.py
+-rw-r--r--   0        0        0     3459 2024-04-10 16:29:16.694716 musical_games-0.6.1/musical_games/external/lilypond.py
+-rw-r--r--   0        0        0     4729 2024-04-09 10:11:56.454487 musical_games-0.6.1/musical_games/external/midi_converters.py
+-rw-r--r--   0        0        0     1142 2024-04-09 10:08:14.006483 musical_games-0.6.1/musical_games/external/utils.py
+-rw-r--r--   0        0        0     2954 2024-04-09 10:11:56.486487 musical_games-0.6.1/musical_games/external/wav_converters.py
+-rw-r--r--   0        0        0     4695 2024-04-09 10:54:53.546529 musical_games-0.6.1/musical_games/utils.py
+-rw-r--r--   0        0        0     1114 2024-04-13 15:07:12.403552 musical_games-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      116 2024-04-09 10:08:14.002483 musical_games-0.6.1/scripts/__init__.py
+-rw-r--r--   0        0        0     1649 2024-04-13 13:01:09.427755 musical_games-0.6.1/scripts/demo_cpe_bach.py
+-rw-r--r--   0        0        0     1652 2024-04-13 13:54:11.547670 musical_games-0.6.1/scripts/demo_kirnberger_meneut_trio.py
+-rw-r--r--   0        0        0     1761 2024-04-13 14:21:32.579626 musical_games-0.6.1/scripts/demo_kirnberger_polonaise.py
+-rw-r--r--   0        0        0     1519 2024-04-13 14:35:38.727603 musical_games-0.6.1/scripts/demo_mozart_waltz.py
+-rw-r--r--   0        0        0     1664 2024-04-13 13:01:48.155754 musical_games-0.6.1/scripts/demo_stadler_meneut_trio.py
+-rwxr-xr-x   0        0        0       24 2024-04-09 10:08:14.002483 musical_games-0.6.1/tests/__init__.py
+-rw-r--r--   0        0        0     1061 2024-04-07 08:43:49.135413 musical_games-0.6.1/tox.ini
+-rw-r--r--   0        0        0     4182 1970-01-01 00:00:00.000000 musical_games-0.6.1/PKG-INFO
```

### Comparing `musical_games-0.5.2/LICENSE` & `musical_games-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `musical_games-0.5.2/docs/Makefile` & `musical_games-0.6.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `musical_games-0.5.2/docs/conf.py` & `musical_games-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `musical_games-0.5.2/docs/contributing.rst` & `musical_games-0.6.1/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.5.2/docs/index.rst` & `musical_games-0.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.5.2/docs/make.bat` & `musical_games-0.6.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `musical_games-0.5.2/docs/musical_games.converters.rst` & `musical_games-0.6.1/docs/musical_games.converters.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.5.2/docs/musical_games.dice_games.lilypond.rst` & `musical_games-0.6.1/docs/musical_games.dice_games.lilypond.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.5.2/docs/musical_games.dice_games.rst` & `musical_games-0.6.1/docs/musical_games.dice_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.5.2/docs/musical_games.rst` & `musical_games-0.6.1/docs/musical_games.rst`

 * *Files identical despite different names*

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly` & `musical_games-0.6.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/bar_overview.ly`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 \version "2.19.81"
 \paper {
     print-all-headers = ##t
-    \BLOCK{ if render_settings['large_page'] }
+    \BLOCK{ if render_settings['single_page'] }
         system-system-spacing = #'((basic-distance . 15))
         paper-height = 420\mm  %% default is 297 for a4
     \BLOCK{ endif }
 }
 \header{
     title = "Counterpoint"
     composer = "C.P.E. Bach."
@@ -24,31 +24,31 @@
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c\major
                 \time 4/4
             }
             {
                 \clef treble
-                \BLOCK{ for bar_index, bar in game_mechanics.bars['treble']['piano_right_hand'].items() }
-                    \VAR{bar}
+                \BLOCK{ for bar in bar_collections['treble'].get_bars('piano_right_hand').values() }
+                    \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c\major
                 \time 4/4
             }
             {
                 \clef bass
-                \BLOCK{ for bar_index, bar in game_mechanics.bars['bass']['piano_left_hand'].items() }
-                    \VAR{bar}
+                \BLOCK{ for bar in bar_collections['bass'].get_bars('piano_left_hand').values() }
+                    \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
     \layout {
         indent = #0
```

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly` & `musical_games-0.6.1/musical_games/data/dice_games/cpe_bach_counterpoint/lilypond/composition_pdf.ly`

 * *Files 9% similar despite different names*

```diff
@@ -58,32 +58,32 @@
                 \key c\major
                 \time 4/4
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
-                \BLOCK{ for bar_index in range(6) }
-                    \VAR{game_mechanics.get_bar('treble', 'piano_right_hand',  bar_nmrs['treble']['piano_right_hand'][bar_index])}
+                \BLOCK{ for synchronous_bar in composition_bars['treble'] }
+                    \VAR{synchronous_bar.get_bars()[0].lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
                 \key c\major
                 \time 4/4
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
-                \BLOCK{ for bar_index in range(6) }
-                    \VAR{game_mechanics.get_bar('bass', 'piano_left_hand',  bar_nmrs['bass']['piano_left_hand'][bar_index])}
+                \BLOCK{ for synchronous_bar in composition_bars['bass'] }
+                    \VAR{synchronous_bar.get_bars()[0].lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
     >>
     \layout {
         indent = 0\mm
```

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/bar_overview.ly`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 \version "2.19.81"
 \paper {
     print-all-headers = ##t
-    \BLOCK{ if render_settings['large_page'] }
+    \BLOCK{ if render_settings['single_page'] }
         system-system-spacing = #'((basic-distance . 15))
         paper-height = 1400\mm  %% default is 297 for a4
     \BLOCK{ endif }
 }
 \header{
     title = "Menuet and Trio"
     composer = "Kirnberger"
@@ -24,31 +24,31 @@
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key d\major
                 \time 3/4
             }
             {
                 \clef treble
-                \BLOCK{ for bar in game_mechanics.bars['menuet']['piano_right_hand'].values() }
-                    \VAR{bar}
+                \BLOCK{ for bar in bar_collections['menuet'].get_bars('piano_right_hand').values() }
+                    \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key d\major
                 \time 3/4
             }
             {
                 \clef bass
-                \BLOCK{ for bar in game_mechanics.bars['menuet']['piano_left_hand'].values() }
-                    \VAR{bar}
+                \BLOCK{ for bar in bar_collections['menuet'].get_bars('piano_left_hand').values() }
+                    \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
     \layout {
         indent = #0
@@ -66,31 +66,31 @@
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key d\minor
                 \time 3/4
             }
             {
                 \clef treble
-                \BLOCK{ for bar in game_mechanics.bars['trio']['piano_right_hand'].values() }
-                    \VAR{bar}
+                \BLOCK{ for bar in bar_collections['trio'].get_bars('piano_right_hand').values() }
+                    \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key d\minor
                 \time 3/4
             }
             {
                 \clef bass
-                \BLOCK{ for bar in game_mechanics.bars['trio']['piano_left_hand'].values() }
-                    \VAR{bar}
+                \BLOCK{ for bar in bar_collections['trio'].get_bars('piano_left_hand').values() }
+                    \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
     \layout {
         indent = 0\mm
```

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.6.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly`

 * *Files 20% similar despite different names*

```diff
@@ -5,63 +5,63 @@
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
     <<
         \new Staff
             \with {
-                midiMinimumVolume = #\VAR{render_settings['menuet_treble_midi_settings'].min_volume}
-                midiMaximumVolume = #\VAR{render_settings['menuet_treble_midi_settings'].max_volume}
-                midiInstrument = #"\VAR{render_settings['menuet_treble_midi_settings'].instrument}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('menuet', 'piano_right_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('menuet', 'piano_right_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('menuet', 'piano_right_hand')}"
             }
         <<
             {
                 \key d\major
                 \time 3/4
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8) }
-                        \VAR{game_mechanics.get_bar('menuet', 'piano_right_hand',  bar_nmrs['menuet']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
-                        \VAR{game_mechanics.get_bar('menuet', 'piano_right_hand',  bar_nmrs['menuet']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
         >>
         \new Staff
 
             \with {
-                midiMinimumVolume = #\VAR{render_settings['menuet_bass_midi_settings'].min_volume}
-                midiMaximumVolume = #\VAR{render_settings['menuet_bass_midi_settings'].max_volume}
-                midiInstrument = #"\VAR{render_settings['menuet_bass_midi_settings'].instrument}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('menuet', 'piano_left_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('menuet', 'piano_left_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('menuet', 'piano_left_hand')}"
             }
         <<
             {
                 \key d\major
                 \time 3/4
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
-    		            \VAR{game_mechanics.get_bar('menuet', 'piano_left_hand',  bar_nmrs['menuet']['piano_left_hand'][bar_index])}
+		                \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
-    		            \VAR{game_mechanics.get_bar('menuet', 'piano_left_hand',  bar_nmrs['menuet']['piano_left_hand'][bar_index])}
+    		            \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
             }
         >>
     >>
     \midi { }
 }
@@ -70,63 +70,63 @@
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
     <<
         \new Staff
             \with {
-                midiMinimumVolume = #\VAR{render_settings['trio_treble_midi_settings'].min_volume}
-                midiMaximumVolume = #\VAR{render_settings['trio_treble_midi_settings'].max_volume}
-                midiInstrument = #"\VAR{render_settings['trio_treble_midi_settings'].instrument}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('trio', 'piano_right_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('trio', 'piano_right_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('trio', 'piano_right_hand')}"
             }
         <<
             {
-                \key d\minor
+                \key g\major
                 \time 3/4
                 \tempo 4 = 80
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8) }
-                        \VAR{game_mechanics.get_bar('trio', 'piano_right_hand',  bar_nmrs['trio']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['trio'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
-                        \VAR{game_mechanics.get_bar('trio', 'piano_right_hand',  bar_nmrs['trio']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['trio'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
         >>
         \new Staff
 
             \with {
-                midiMinimumVolume = #\VAR{render_settings['trio_bass_midi_settings'].min_volume}
-                midiMaximumVolume = #\VAR{render_settings['trio_bass_midi_settings'].max_volume}
-                midiInstrument = #"\VAR{render_settings['trio_bass_midi_settings'].instrument}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('trio', 'piano_left_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('trio', 'piano_left_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('trio', 'piano_left_hand')}"
             }
         <<
             {
-                \key d\minor
+                \key g\major
                 \time 3/4
                 \tempo 4 = 80
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
-		                \VAR{game_mechanics.get_bar('trio', 'piano_left_hand',  bar_nmrs['trio']['piano_left_hand'][bar_index])}
+		                \VAR{composition_bars['trio'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
-    		            \VAR{game_mechanics.get_bar('trio', 'piano_left_hand',  bar_nmrs['trio']['piano_left_hand'][bar_index])}
+    		            \VAR{composition_bars['trio'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
             }
         >>
     >>
     \midi { }
 }
@@ -135,51 +135,51 @@
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
     <<
         \new Staff
             \with {
-                midiMinimumVolume = #\VAR{render_settings['menuet_treble_midi_settings'].min_volume}
-                midiMaximumVolume = #\VAR{render_settings['menuet_treble_midi_settings'].max_volume}
-                midiInstrument = #"\VAR{render_settings['menuet_treble_midi_settings'].instrument}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('menuet', 'piano_right_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('menuet', 'piano_right_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('menuet', 'piano_right_hand')}"
             }
         <<
             {
                 \key d\major
                 \time 3/4
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \BLOCK{ for bar_index in range(16) }
-                    \VAR{game_mechanics.get_bar('menuet', 'piano_right_hand',  bar_nmrs['menuet']['piano_right_hand'][bar_index])}
+                    \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
 
             \with {
-                midiMinimumVolume = #\VAR{render_settings['menuet_bass_midi_settings'].min_volume}
-                midiMaximumVolume = #\VAR{render_settings['menuet_bass_midi_settings'].max_volume}
-                midiInstrument = #"\VAR{render_settings['menuet_bass_midi_settings'].instrument}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('menuet', 'piano_left_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('menuet', 'piano_left_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('menuet', 'piano_left_hand')}"
             }
         <<
             {
                 \key d\major
                 \time 3/4
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
                 \BLOCK{ for bar_index in range(16) }
-                    \VAR{game_mechanics.get_bar('menuet', 'piano_left_hand',  bar_nmrs['menuet']['piano_left_hand'][bar_index])}
+                    \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
     >>
     \midi { }
 }
```

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_pdf.ly`

 * *Files 15% similar despite different names*

```diff
@@ -26,20 +26,20 @@
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8) }
-                        \VAR{game_mechanics.get_bar('menuet', 'piano_right_hand',  bar_nmrs['menuet']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
-                        \VAR{game_mechanics.get_bar('menuet', 'piano_right_hand',  bar_nmrs['menuet']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
         >>
         \new Staff
         <<
             {
@@ -48,20 +48,20 @@
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
-		                \VAR{game_mechanics.get_bar('menuet', 'piano_left_hand',  bar_nmrs['menuet']['piano_left_hand'][bar_index])}
+		                \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
-    		            \VAR{game_mechanics.get_bar('menuet', 'piano_left_hand',  bar_nmrs['menuet']['piano_left_hand'][bar_index])}
+    		            \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \once \override Score.RehearsalMark #'self-alignment-X = #right \mark \markup {\fontsize #-1 \italic "Fine"}
             }
         >>
     >>
     \layout {
@@ -85,20 +85,20 @@
                 \tempo 4 = 80
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8) }
-                        \VAR{game_mechanics.get_bar('trio', 'piano_right_hand',  bar_nmrs['trio']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['trio'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
-                        \VAR{game_mechanics.get_bar('trio', 'piano_right_hand',  bar_nmrs['trio']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['trio'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
         >>
         \new Staff
         <<
             {
@@ -107,20 +107,20 @@
                 \tempo 4 = 80
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
-    		            \VAR{game_mechanics.get_bar('trio', 'piano_left_hand',  bar_nmrs['trio']['piano_left_hand'][bar_index])}
+		                \VAR{composition_bars['trio'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
-    		            \VAR{game_mechanics.get_bar('trio', 'piano_left_hand',  bar_nmrs['trio']['piano_left_hand'][bar_index])}
+    		            \VAR{composition_bars['trio'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \once \override Score.RehearsalMark #'self-alignment-X = #right \mark \markup {\fontsize #-1 \italic "D.C. al Fine"}
             }
         >>
     >>
     \layout {
```

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.6.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly`

 * *Files 24% similar despite different names*

```diff
@@ -14,38 +14,38 @@
         \new Staff
         <<
             {
                 \BLOCK{ if table_name == 'menuet' }
                     \key d\major
                     \time 3/4
                 \BLOCK{ else }
-                    \key d\minor
+                    \key g\major
                     \time 3/4
                 \BLOCK{ endif }
             }
             {
                 \clef treble
-                \VAR{ game_mechanics.bars[table_name]['piano_right_hand'][bar_nmr] }
+                \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
                 \BLOCK{ if table_name == 'menuet' }
                     \key d\major
                     \time 3/4
                 \BLOCK{ else }
-                    \key d\minor
+                    \key g\major
                     \time 3/4
                 \BLOCK{ endif }
             }
             {
                 \clef bass
-                \VAR{ game_mechanics.bars[table_name]['piano_left_hand'][bar_nmr] }
+                \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
                 \bar "|."
             }
         >>
     >>
     \layout {
         indent = 0\mm
     }
```

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt` & `musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt` & `musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/menuet/chamber_music/bars_menuet_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt` & `musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_lh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt` & `musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/optional_instruments/trio/chamber_music/bars_trio_rh.txt`

 * *Files identical despite different names*

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly` & `musical_games-0.6.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/bar_overview.ly`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 \version "2.19.81"
 \paper {
     print-all-headers = ##t
 
-    \BLOCK{ if render_settings['large_page'] }
+    \BLOCK{ if render_settings['single_page'] }
         system-system-spacing = #'((basic-distance . 15))
         paper-height = 3400\mm  %% default is 297 for a4
     \BLOCK{ endif }
 }
 \header{
     title = "Polonaise"
     composer = "Kirnberger"
@@ -26,16 +26,16 @@
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key d\major
                 \time 3/4
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
-                \BLOCK{ for bar_index, bar in game_mechanics.bars['polonaise']['violin_1'].items() }
-                    \VAR{bar}
+                \BLOCK{ for bar in bar_collections['polonaise'].get_bars('violin_1').values() }
+                    \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             \set Staff.instrumentName = #"Violin #2 "
@@ -43,16 +43,16 @@
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key d\major
                 \time 3/4
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
-                \BLOCK{ for bar_index, bar in game_mechanics.bars['polonaise']['violin_2'].items() }
-                    \VAR{bar}
+                \BLOCK{ for bar in bar_collections['polonaise'].get_bars('violin_2').values() }
+                    \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new PianoStaff
         <<
             \set PianoStaff.instrumentName = #"Piano"
@@ -62,32 +62,32 @@
                     \override Score.BarNumber.break-visibility = ##(#t #t #t)
                     \key d\major
                     \time 3/4
                     \override Score.RehearsalMark.direction = #down
                 }
                 {
                     \clef treble
-                    \BLOCK{ for bar_index, bar in game_mechanics.bars['polonaise']['piano_right_hand'].items() }
-                        \VAR{bar}
+                    \BLOCK{ for bar in bar_collections['polonaise'].get_bars('piano_right_hand').values() }
+                        \VAR{bar.lilypond_str}
                     \BLOCK{ endfor }
                     \bar "|"
                 }
             >>
             \new Staff
             <<
                 {
                     \override Score.BarNumber.break-visibility = ##(#t #t #t)
                     \key d\major
                     \time 3/4
                     \override Score.RehearsalMark.direction = #down
                 }
                 {
                     \clef bass
-                    \BLOCK{ for bar_index, bar in game_mechanics.bars['polonaise']['piano_left_hand'].items() }
-                        \VAR{bar}
+                    \BLOCK{ for bar in bar_collections['polonaise'].get_bars('piano_left_hand').values() }
+                        \VAR{bar.lilypond_str}
                     \BLOCK{ endfor }
                     \bar "|"
                 }
             >>
         >>
     >>
 }
```

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly` & `musical_games-0.6.1/musical_games/data/dice_games/kirnberger_polonaise/lilypond/single_bar.ly`

 * *Files 20% similar despite different names*

```diff
@@ -16,54 +16,54 @@
             \set Staff.instrumentName = #"Violin #1 "
             {
                 \key d\major
                 \time 3/4
             }
             {
                 \clef treble
-                \VAR{ game_mechanics.bars[table_name]['violin_1'][bar_nmr] }
+                \VAR{ synchronous_bar.get_bar('violin_1').lilypond_str }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             \set Staff.instrumentName = #"Violin #2 "
             {
                 \key d\major
                 \time 3/4
             }
             {
                 \clef treble
-                \VAR{ game_mechanics.bars[table_name]['violin_2'][bar_nmr] }
+                \VAR{ synchronous_bar.get_bar('violin_2').lilypond_str }
                 \bar "|."
             }
         >>
         \new PianoStaff
         <<
             \set PianoStaff.instrumentName = #"Piano"
             \new Staff
             <<
                 {
                     \key d\major
                     \time 3/4
                 }
                 {
                     \clef treble
-                    \VAR{ game_mechanics.bars[table_name]['piano_right_hand'][bar_nmr] }
+                    \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
                     \bar "|."
                 }
             >>
             \new Staff
             <<
                 {
                     \key d\major
                     \time 3/4
                 }
                 {
                     \clef bass
-                    \VAR{ game_mechanics.bars[table_name]['piano_left_hand'][bar_nmr] }
+                    \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
                     \bar "|."
                 }
             >>
         >>
     >>
 }
```

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly` & `musical_games-0.6.1/musical_games/data/dice_games/mozart_waltz/lilypond/bar_overview.ly`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 \version "2.19.81"
 \paper {
     print-all-headers = ##t
 
-    \BLOCK{ if render_settings['large_page'] }
+    \BLOCK{ if render_settings['single_page'] }
         system-system-spacing = #'((basic-distance . 15))
         paper-height = 1200\mm  %% default is 297 for a4
     \BLOCK{ endif }
 }
 \header{
     title = "Waltz"
     composer = "Mozart"
@@ -25,34 +25,34 @@
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c\major
                 \time 3/8
             }
             {
                 \clef treble
-                \BLOCK{ for bar in game_mechanics.bars['waltz']['piano_right_hand'].values() }
-                    \VAR{bar}
+                \BLOCK{ for bar in bar_collections['waltz'].get_bars('piano_right_hand').values() }
+                    \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key c\major
                 \time 3/8
             }
             {
                 \clef bass
-                \BLOCK{ for ind, bar in game_mechanics.bars['waltz']['piano_left_hand'].items() }
-                    \BLOCK{ if game_mechanics.bars['waltz']['piano_left_hand_alternative'][ind] }
-                        << {\voiceOne \VAR{bar} } \new Voice { \voiceTwo \VAR{game_mechanics.bars['waltz']['piano_left_hand_alternative'][ind]}} >>
+                \BLOCK{ for bar_ind, bar in bar_collections['waltz'].get_bars('piano_left_hand').items() }
+                    \BLOCK{ if bar_collections['waltz'].get_bar('piano_left_hand_alternative', bar_ind).lilypond_str != '' }
+                        <<{\voiceOne \VAR{bar.lilypond_str}} \new Voice {\voiceTwo \VAR{bar_collections['waltz'].get_bar('piano_left_hand_alternative', bar_ind).lilypond_str}}>>
                     \BLOCK{ else }
-                        \VAR{bar}
+                        \VAR{bar.lilypond_str}
                     \BLOCK{ endif }
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
     \layout {
```

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly` & `musical_games-0.6.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_midi.ly`

 * *Files 26% similar despite different names*

```diff
@@ -3,69 +3,69 @@
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
     <<
         \new Staff
             \with {
-                midiMinimumVolume = #\VAR{render_settings['piano_rh_midi_settings'].min_volume}
-                midiMaximumVolume = #\VAR{render_settings['piano_rh_midi_settings'].max_volume}
-                midiInstrument = #"\VAR{render_settings['piano_rh_midi_settings'].instrument}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('waltz', 'piano_right_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('waltz', 'piano_right_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('waltz', 'piano_right_hand')}"
             }
         <<
             {
                 \key c\major
                 \time 3/8
                 \tempo 8 = 110
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(7) }
-                        \VAR{game_mechanics.get_bar('waltz', 'piano_right_hand',  bar_nmrs['waltz']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['waltz'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
 
-                \alternative { {\VAR{game_mechanics.get_bar('waltz', 'piano_right_hand', bar_nmrs['waltz']['piano_right_hand'][7])}} {\VAR{game_mechanics.get_bar('waltz', 'piano_right_hand', bar_nmrs['waltz']['piano_right_hand'][7])}} }
+                \alternative { {\VAR{composition_bars['waltz'][7].get_bar('piano_right_hand').lilypond_str}} {\VAR{composition_bars['waltz'][7].get_bar('piano_right_hand').lilypond_str}} }
 
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
-                        \VAR{game_mechanics.get_bar('waltz', 'piano_right_hand',  bar_nmrs['waltz']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['waltz'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
         >>
         \new Staff
 
             \with {
-                midiMinimumVolume = #\VAR{render_settings['piano_lh_midi_settings'].min_volume}
-                midiMaximumVolume = #\VAR{render_settings['piano_lh_midi_settings'].max_volume}
-                midiInstrument = #"\VAR{render_settings['piano_lh_midi_settings'].instrument}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('waltz', 'piano_left_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('waltz', 'piano_left_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('waltz', 'piano_left_hand')}"
             }
         <<
             {
                 \key c\major
                 \time 3/8
                 \tempo 8 = 110
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(7) }
-		                \VAR{game_mechanics.get_bar('waltz', 'piano_left_hand',  bar_nmrs['waltz']['piano_left_hand'][bar_index])}
+		                \VAR{composition_bars['waltz'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 
-                \alternative { {\VAR{game_mechanics.get_bar('waltz', 'piano_left_hand', bar_nmrs['waltz']['piano_left_hand'][7])}} {\VAR{game_mechanics.get_bar('waltz', 'piano_left_hand_alternative', bar_nmrs['waltz']['piano_left_hand'][7])}} }
+                \alternative { {\VAR{composition_bars['waltz'][7].get_bar('piano_left_hand').lilypond_str}} {\VAR{composition_bars['waltz'][7].get_bar('piano_left_hand_alternative').lilypond_str}} }
 
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
-    		            \VAR{game_mechanics.get_bar('waltz', 'piano_left_hand',  bar_nmrs['waltz']['piano_left_hand'][bar_index])}
+    		            \VAR{composition_bars['waltz'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
             }
         >>
     >>
     \midi { }
 }
```

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly` & `musical_games-0.6.1/musical_games/data/dice_games/mozart_waltz/lilypond/composition_pdf.ly`

 * *Files 21% similar despite different names*

```diff
@@ -60,23 +60,23 @@
                 \tempo 8 = 110
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(7) }
-                        \VAR{game_mechanics.get_bar('waltz', 'piano_right_hand',  bar_nmrs['waltz']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['waltz'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
 
-                \alternative { {\VAR{game_mechanics.get_bar('waltz', 'piano_right_hand', bar_nmrs['waltz']['piano_right_hand'][7])}} {\VAR{game_mechanics.get_bar('waltz', 'piano_right_hand', bar_nmrs['waltz']['piano_right_hand'][7])}} }
+                \alternative { {\VAR{composition_bars['waltz'][7].get_bar('piano_right_hand').lilypond_str}} {\VAR{composition_bars['waltz'][7].get_bar('piano_right_hand').lilypond_str}} }
 
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
-                        \VAR{game_mechanics.get_bar('waltz', 'piano_right_hand',  bar_nmrs['waltz']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['waltz'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
         >>
         \new Staff
         <<
             {
@@ -85,23 +85,23 @@
                 \tempo 8 = 110
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(7) }
-		                \VAR{game_mechanics.get_bar('waltz', 'piano_left_hand',  bar_nmrs['waltz']['piano_left_hand'][bar_index])}
+		                \VAR{composition_bars['waltz'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 
-                \alternative { {\VAR{game_mechanics.get_bar('waltz', 'piano_left_hand', bar_nmrs['waltz']['piano_left_hand'][7])}} {\VAR{game_mechanics.get_bar('waltz', 'piano_left_hand_alternative', bar_nmrs['waltz']['piano_left_hand'][7])}} }
+                \alternative { {\VAR{composition_bars['waltz'][7].get_bar('piano_left_hand').lilypond_str}} {\VAR{composition_bars['waltz'][7].get_bar('piano_left_hand_alternative').lilypond_str}} }
 
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
-    		            \VAR{game_mechanics.get_bar('waltz', 'piano_left_hand',  bar_nmrs['waltz']['piano_left_hand'][bar_index])}
+    		            \VAR{composition_bars['waltz'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
             }
         >>
     >>
     \layout {
         indent = 0\mm
```

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly` & `musical_games-0.6.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/bar_overview.ly`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 \version "2.19.81"
 \paper {
     print-all-headers = ##t
-    \BLOCK{ if render_settings['large_page'] }
+    \BLOCK{ if render_settings['single_page'] }
         system-system-spacing = #'((basic-distance . 15))
         paper-height = 2800\mm  %% default is 297 for a4
     \BLOCK{ endif }
 }
 \header{
     title = "Menuet and Trio"
     composer = "Stadler"
@@ -24,31 +24,31 @@
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key d\major
                 \time 3/4
             }
             {
                 \clef treble
-                \BLOCK{ for bar in game_mechanics.bars['menuet']['piano_right_hand'].values() }
-                    \VAR{bar}
+                \BLOCK{ for bar in bar_collections['menuet'].get_bars('piano_right_hand').values() }
+                    \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key d\major
                 \time 3/4
             }
             {
                 \clef bass
-                \BLOCK{ for bar in game_mechanics.bars['menuet']['piano_left_hand'].values() }
-                    \VAR{bar}
+                \BLOCK{ for bar in bar_collections['menuet'].get_bars('piano_left_hand').values() }
+                    \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
     \layout {
         indent = #0
@@ -67,31 +67,31 @@
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key g\major
                 \time 3/4
             }
             {
                 \clef treble
-                \BLOCK{ for bar in game_mechanics.bars['trio']['piano_right_hand'].values() }
-                    \VAR{bar}
+                \BLOCK{ for bar in bar_collections['trio'].get_bars('piano_right_hand').values() }
+                    \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
         \new Staff
         <<
             {
                 \override Score.BarNumber.break-visibility = ##(#t #t #t)
                 \key g\major
                 \time 3/4
             }
             {
                 \clef bass
-                \BLOCK{ for bar in game_mechanics.bars['trio']['piano_left_hand'].values() }
-                    \VAR{bar}
+                \BLOCK{ for bar in bar_collections['trio'].get_bars('piano_left_hand').values() }
+                    \VAR{bar.lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|"
             }
         >>
     >>
     \layout {
         indent = 0\mm
```

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_midi.ly` & `musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/composition_midi.ly`

 * *Files 22% similar despite different names*

```diff
@@ -5,63 +5,63 @@
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
     <<
         \new Staff
             \with {
-                midiMinimumVolume = #\VAR{render_settings['menuet_treble_midi_settings'].min_volume}
-                midiMaximumVolume = #\VAR{render_settings['menuet_treble_midi_settings'].max_volume}
-                midiInstrument = #"\VAR{render_settings['menuet_treble_midi_settings'].instrument}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('menuet', 'piano_right_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('menuet', 'piano_right_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('menuet', 'piano_right_hand')}"
             }
         <<
             {
                 \key d\major
                 \time 3/4
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8) }
-                        \VAR{game_mechanics.get_bar('menuet', 'piano_right_hand',  bar_nmrs['menuet']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
-                        \VAR{game_mechanics.get_bar('menuet', 'piano_right_hand',  bar_nmrs['menuet']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
         >>
         \new Staff
 
             \with {
-                midiMinimumVolume = #\VAR{render_settings['menuet_bass_midi_settings'].min_volume}
-                midiMaximumVolume = #\VAR{render_settings['menuet_bass_midi_settings'].max_volume}
-                midiInstrument = #"\VAR{render_settings['menuet_bass_midi_settings'].instrument}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('menuet', 'piano_left_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('menuet', 'piano_left_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('menuet', 'piano_left_hand')}"
             }
         <<
             {
                 \key d\major
                 \time 3/4
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
-		                \VAR{game_mechanics.get_bar('menuet', 'piano_left_hand',  bar_nmrs['menuet']['piano_left_hand'][bar_index])}
+		                \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
-    		            \VAR{game_mechanics.get_bar('menuet', 'piano_left_hand',  bar_nmrs['menuet']['piano_left_hand'][bar_index])}
+    		            \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
             }
         >>
     >>
     \midi { }
 }
@@ -70,63 +70,63 @@
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
     <<
         \new Staff
             \with {
-                midiMinimumVolume = #\VAR{render_settings['trio_treble_midi_settings'].min_volume}
-                midiMaximumVolume = #\VAR{render_settings['trio_treble_midi_settings'].max_volume}
-                midiInstrument = #"\VAR{render_settings['trio_treble_midi_settings'].instrument}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('trio', 'piano_right_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('trio', 'piano_right_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('trio', 'piano_right_hand')}"
             }
         <<
             {
-                \key g\major
+                \key d\minor
                 \time 3/4
                 \tempo 4 = 80
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8) }
-                        \VAR{game_mechanics.get_bar('trio', 'piano_right_hand',  bar_nmrs['trio']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['trio'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
-                        \VAR{game_mechanics.get_bar('trio', 'piano_right_hand',  bar_nmrs['trio']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['trio'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
         >>
         \new Staff
 
             \with {
-                midiMinimumVolume = #\VAR{render_settings['trio_bass_midi_settings'].min_volume}
-                midiMaximumVolume = #\VAR{render_settings['trio_bass_midi_settings'].max_volume}
-                midiInstrument = #"\VAR{render_settings['trio_bass_midi_settings'].instrument}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('trio', 'piano_left_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('trio', 'piano_left_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('trio', 'piano_left_hand')}"
             }
         <<
             {
-                \key g\major
+                \key d\minor
                 \time 3/4
                 \tempo 4 = 80
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
-		                \VAR{game_mechanics.get_bar('trio', 'piano_left_hand',  bar_nmrs['trio']['piano_left_hand'][bar_index])}
+		                \VAR{composition_bars['trio'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
-    		            \VAR{game_mechanics.get_bar('trio', 'piano_left_hand',  bar_nmrs['trio']['piano_left_hand'][bar_index])}
+    		            \VAR{composition_bars['trio'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
             }
         >>
     >>
     \midi { }
 }
@@ -135,51 +135,51 @@
 \score {
     \unfoldRepeats
     \articulate
     \new GrandStaff
     <<
         \new Staff
             \with {
-                midiMinimumVolume = #\VAR{render_settings['menuet_treble_midi_settings'].min_volume}
-                midiMaximumVolume = #\VAR{render_settings['menuet_treble_midi_settings'].max_volume}
-                midiInstrument = #"\VAR{render_settings['menuet_treble_midi_settings'].instrument}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('menuet', 'piano_right_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('menuet', 'piano_right_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('menuet', 'piano_right_hand')}"
             }
         <<
             {
                 \key d\major
                 \time 3/4
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \BLOCK{ for bar_index in range(16) }
-                    \VAR{game_mechanics.get_bar('menuet', 'piano_right_hand',  bar_nmrs['menuet']['piano_right_hand'][bar_index])}
+                    \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
         \new Staff
 
             \with {
-                midiMinimumVolume = #\VAR{render_settings['menuet_bass_midi_settings'].min_volume}
-                midiMaximumVolume = #\VAR{render_settings['menuet_bass_midi_settings'].max_volume}
-                midiInstrument = #"\VAR{render_settings['menuet_bass_midi_settings'].instrument}"
+                midiMinimumVolume = #\VAR{midi_settings.get_min_volume('menuet', 'piano_left_hand')}
+                midiMaximumVolume = #\VAR{midi_settings.get_max_volume('menuet', 'piano_left_hand')}
+                midiInstrument = #"\VAR{midi_settings.get_midi_instrument('menuet', 'piano_left_hand')}"
             }
         <<
             {
                 \key d\major
                 \time 3/4
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
                 \BLOCK{ for bar_index in range(16) }
-                    \VAR{game_mechanics.get_bar('menuet', 'piano_left_hand',  bar_nmrs['menuet']['piano_left_hand'][bar_index])}
+                    \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
                 \BLOCK{ endfor }
                 \bar "|."
             }
         >>
     >>
     \midi { }
 }
```

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly` & `musical_games-0.6.1/musical_games/data/dice_games/stadler_menuet_trio/lilypond/composition_pdf.ly`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 \version "2.19.81"
 \paper {
 	print-all-headers = ##t
     score-markup-spacing = #'((basic-distance . 10))
     markup-system-spacing = #'((minimum-distance = 0))
 
-    \BLOCK{ if render_settings['large_page'] }
+    \BLOCK{ if render_settings['single_page'] }
         paper-height = 360\mm  %% default is 297 for a4
     \BLOCK{ endif }
 }
 \header{
     title = "Menuet and Trio"
     composer = "Stadler"
     tagline = ##f
@@ -29,20 +29,20 @@
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8) }
-                        \VAR{game_mechanics.get_bar('menuet', 'piano_right_hand',  bar_nmrs['menuet']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
-                        \VAR{game_mechanics.get_bar('menuet', 'piano_right_hand',  bar_nmrs['menuet']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['menuet'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
         >>
         \new Staff
         <<
             {
@@ -51,20 +51,20 @@
                 \tempo 4 = 100
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
-		                \VAR{game_mechanics.get_bar('menuet', 'piano_left_hand',  bar_nmrs['menuet']['piano_left_hand'][bar_index])}
+		                \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
-    		            \VAR{game_mechanics.get_bar('menuet', 'piano_left_hand',  bar_nmrs['menuet']['piano_left_hand'][bar_index])}
+    		            \VAR{composition_bars['menuet'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \once \override Score.RehearsalMark #'self-alignment-X = #right \mark \markup {\fontsize #-1 \italic "Fine"}
             }
         >>
     >>
     \layout {
@@ -88,20 +88,20 @@
                 \tempo 4 = 80
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef treble
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8) }
-                        \VAR{game_mechanics.get_bar('trio', 'piano_right_hand',  bar_nmrs['trio']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['trio'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
                 \repeat volta 2{
                     \BLOCK{ for bar_index in range(8, 16) }
-                        \VAR{game_mechanics.get_bar('trio', 'piano_right_hand',  bar_nmrs['trio']['piano_right_hand'][bar_index])}
+                        \VAR{composition_bars['trio'][bar_index].get_bar('piano_right_hand').lilypond_str}
                     \BLOCK{ endfor }
                 }
             }
         >>
         \new Staff
         <<
             {
@@ -110,20 +110,20 @@
                 \tempo 4 = 80
                 \override Score.RehearsalMark.direction = #down
             }
             {
                 \clef bass
 		        \repeat volta 2{
 		            \BLOCK{ for bar_index in range(8) }
-		                \VAR{game_mechanics.get_bar('trio', 'piano_left_hand',  bar_nmrs['trio']['piano_left_hand'][bar_index])}
+		                \VAR{composition_bars['trio'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \repeat volta 2{
     		        \BLOCK{ for bar_index in range(8, 16) }
-    		            \VAR{game_mechanics.get_bar('trio', 'piano_left_hand',  bar_nmrs['trio']['piano_left_hand'][bar_index])}
+    		            \VAR{composition_bars['trio'][bar_index].get_bar('piano_left_hand').lilypond_str}
     		        \BLOCK{ endfor }
 	        	}
 		        \once \override Score.RehearsalMark #'self-alignment-X = #right \mark \markup {\fontsize #-1 \italic "D.C. al Fine"}
             }
         >>
     >>
     \layout {
```

### Comparing `musical_games-0.5.2/musical_games/data/dice_games/stadler_menuet_trio/lilypond/single_bar.ly` & `musical_games-0.6.1/musical_games/data/dice_games/kirnberger_menuet_trio/lilypond/single_bar.ly`

 * *Files 26% similar despite different names*

```diff
@@ -14,38 +14,38 @@
         \new Staff
         <<
             {
                 \BLOCK{ if table_name == 'menuet' }
                     \key d\major
                     \time 3/4
                 \BLOCK{ else }
-                    \key g\major
+                    \key d\minor
                     \time 3/4
                 \BLOCK{ endif }
             }
             {
                 \clef treble
-                \VAR{ game_mechanics.bars[table_name]['piano_right_hand'][bar_nmr] }
+                \VAR{ synchronous_bar.get_bar('piano_right_hand').lilypond_str }
                 \bar "|."
             }
         >>
         \new Staff
         <<
             {
                 \BLOCK{ if table_name == 'menuet' }
                     \key d\major
                     \time 3/4
                 \BLOCK{ else }
-                    \key g\major
+                    \key d\minor
                     \time 3/4
                 \BLOCK{ endif }
             }
             {
                 \clef bass
-                \VAR{ game_mechanics.bars[table_name]['piano_left_hand'][bar_nmr] }
+                \VAR{ synchronous_bar.get_bar('piano_left_hand').lilypond_str }
                 \bar "|."
             }
         >>
     >>
     \layout {
         indent = 0\mm
     }
```

### Comparing `musical_games-0.5.2/musical_games/lib/lilypond.py` & `musical_games-0.6.1/musical_games/external/lilypond.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,97 +1,111 @@
-import os
-import subprocess
-
 __author__ = 'Robbert Harms'
 __date__ = "2015-09-22"
 __maintainer__ = "Robbert Harms"
-__email__ = "robbert.harms@maastrichtuniversity.nl"
+__email__ = "robbert@xkls.nl"
+
+from dataclasses import dataclass
+from pathlib import Path
+import os
+
+from musical_games.external.images import trim_image
+from musical_games.external.utils import run_command
 
 
-def lilypond(lilypond_fname, output, pdf=True, png=True, ps=False):
-    """Typeset music and/or produce midi from file.
+def typeset_lilypond(lilypond_in: Path, output_basename: Path, pdf: bool = True, png: bool = True, ps: bool = False):
+    """Typeset a lilypond file and produce midi and/or a composition from the input file.
 
     This runs the shell command lilypond to on the inputs. Note that Midi output needs to be defined in the lilypond
     file and can not be set on the command line.
 
     Args:
-        lilypond_fname (Path or str): the location of the lilypond file to convert.
-        output (str): the location for the output files, suffixes will be added.
-        pdf (bool): if we want pdf output
-        png (boolean): if we want png output
-        ps (boolean): if we want postscript output
+        lilypond_in: the location of the lilypond file to convert.
+        output_basename: the location for the output files, suffixes will be added.
+        pdf: if we want pdf output
+        png: if we want png output
+        ps: if we want postscript output
 
     Raises:
         RuntimeError: if the compilation of the lilypond file failed somehow.
 
     Returns:
-        TypesetResults: the result set with the location of the output files.
+        LilypondTypesetResults: the result set with the location of the output files.
     """
-    if not os.path.isdir(os.path.dirname(output)):
-        os.makedirs(os.path.dirname(output))
+    output_basename.parent.mkdir(parents=True, exist_ok=True)
 
     command = ['lilypond']
     if pdf:
         command.append('--pdf')
     if png:
         command.append('--png')
     if ps:
         command.append('--ps')
-    command.extend(['-o', output, lilypond_fname])
+    command.extend(['-o', output_basename, lilypond_in])
 
-    process = subprocess.Popen(command, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-    std_err = process.communicate()[1]
-    rc = process.returncode
+    run_command(command)
 
-    if rc == 1:
-        raise RuntimeError('Error converting lilypond file. Error message: ' + str(std_err))
+    pdf_list = [output_basename.with_suffix('.pdf')] if pdf else []
+    png_list = _get_png_list(output_basename) if png else []
+    ps_list = [output_basename.with_suffix('.ps')] if ps else []
+    midi_list = _get_midi_list(output_basename)
 
-    pdf_list = [output + '.pdf'] if pdf else []
-    png_list = _get_png_list(output, png)
-    ps_list = [output + '.ps'] if ps else []
-    midi_list = _get_midi_list(output)
+    for png in png_list:
+        trim_image(png)
 
-    return TypesetResults(pdf_list, png_list, ps_list, midi_list)
+    return LilypondTypesetResults(pdf_list, png_list, ps_list, midi_list)
+
+
+@dataclass(frozen=True, slots=True)
+class LilypondTypesetResults:
+    """Result set for the output of the lilypond function.
+
+    Args:
+        pdf_list: the locations of the output pdf files
+        png_list: the locations of the png files
+        ps_list: the locations of the ps files
+        midi_list: the locations of the midi files
+    """
+    pdf_list: list[Path]
+    png_list: list[Path]
+    ps_list: list[Path]
+    midi_list: list[Path]
 
 
-class TypesetResults(object):
+def _get_png_list(output_basename: Path) -> list[Path]:
+    """Get the list of PNG images created by the lilypond typesetter.
 
-    def __init__(self, pdf_list, png_list, ps_list, midi_list):
-        """Result set for the output of the lilypond function.
+    Args:
+        output_basename: the basename of the output
 
-        Args:
-            pdf_list (list of str): the locations of the output pdf files
-            png_list (list of str): the locations of the png files
-            ps_list (list of str): the locations of the ps files
-            midi_list (list of str): the locations of the midi files
-        """
-        self.pdf_list = pdf_list
-        self.png_list = png_list
-        self.ps_list = ps_list
-        self.midi_list = midi_list
+    Returns:
+        A list of paths to the generated output files.
+    """
+    png_list = []
+    if output_basename.with_suffix('.png').exists():
+        png_list.append(output_basename.with_suffix('.png'))
 
+    i = 1
+    while os.path.isfile(str(output_basename) + '-page{}.png'.format(i)):
+        png_list.append(Path(str(output_basename) + '-page{}.png'.format(i)))
+        i += 1
+    return png_list
 
-def _get_png_list(output, png_enabled):
-    if png_enabled:
-        png_list = []
-        if os.path.isfile(output + '.png'):
-            png_list.append(output + '.png')
 
-        i = 1
-        while os.path.isfile(output + '-page{}.png'.format(i)):
-            png_list.append(output + '-page{}.png'.format(i))
-            i += 1
-        return png_list
-    return []
+def _get_midi_list(output_basename: Path) -> list[Path]:
+    """Get the list of midi images created by the lilypond typesetter.
 
+    Args:
+        output_basename: the basename of the output
 
-def _get_midi_list(output):
+    Returns:
+        A list of paths to the generated midi files.
+    """
     midi_list = []
-    if os.path.isfile(output + '.midi'):
-        midi_list.append(output + '.midi')
+    if output_basename.with_suffix('.midi').exists():
+        midi_list.append(output_basename.with_suffix('.midi'))
 
     i = 1
-    while os.path.isfile(output + '-{}.midi'.format(i)):
-        midi_list.append(output + '-{}.midi'.format(i))
+    while os.path.isfile(str(output_basename) + '-{}.midi'.format(i)):
+        midi_list.append(Path(str(output_basename) + '-{}.midi'.format(i)))
         i += 1
 
     return midi_list
```

### Comparing `musical_games-0.5.2/musical_games/utils.py` & `musical_games-0.6.1/musical_games/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,110 +1,115 @@
-import os
-import multiprocessing
-from musical_games.lib.audio import midi_to_wav, wav_to_mp3, wav_to_ogg
-from musical_games.lib.lilypond import lilypond, TypesetResults
+from __future__ import annotations
 
 __author__ = 'Robbert Harms'
 __date__ = "2015-09-23"
 __maintainer__ = "Robbert Harms"
-__email__ = "robbert.harms@maastrichtuniversity.nl"
+__email__ = "robbert@xkls.nl"
 
+from concurrent.futures.thread import ThreadPoolExecutor
+from dataclasses import dataclass
+from pathlib import Path
 
-def auto_convert_lilypond_file(lilypond_filename, sound_font=None, output_prefix=None, pdf=True,
-                               png=True, ps=False, mp3=True, ogg=True, midi_gain=None):
+from musical_games.external.wav_converters import wav_to_mp3, wav_to_ogg
+from musical_games.external.midi_converters import midi_to_wav
+from musical_games.external.lilypond import typeset_lilypond, LilypondTypesetResults
+
+
+def auto_convert_lilypond_file(lilypond_in: Path, soundfont: Path | None = None, output_basename: Path | None = None,
+                               pdf: bool = True, png: bool = True, ps: bool = False, mp3: bool = True,
+                               ogg: bool = True, midi_gain: float | None = None) -> AutoConvertLilypondResults:
     """Converts a lilypond file to pdf, png, midi, wav, mp3 and ogg.
 
-    The idea is that given a lilypond file you want to have some standard output. This wrapper function
-    will give you the common output files.
+    Given a lilypond file we create some common output files you are typically interested in.
 
     Args:
-        lilypond_filename (str): the lilypond file name
-        sound_font (str): the path to the soundfont to use. If not given we will not convert to wav, mp3 and ogg.
-        output_prefix (str): path + file prefix. If None we use the dir and basename of the lilypond file.
-        pdf (boolean): if we want pdf output
-        png (boolean): if we want png output
-        ps (boolean): if we want postscript output
-        mp3 (boolean): if we want mp3 output, only applicable if the lilypond has midi output defined
-        ogg (boolean): if we want ogg output, only applicable if the lilypond has midi output defined
-        png_concatenation (PNGConcatenation): the concatenation routine to use for concatenating the PNGs
-        midi_gain (float): the gain for use during the midi to wav conversion
+        lilypond_in: the lilypond file name
+        soundfont: the path to the soundfont to use. If not given we will not convert to wav, mp3 and ogg.
+        output_basename: path + file prefix. If None we use the dir and basename of the lilypond file.
+        pdf: if we want pdf output
+        png: if we want png output
+        ps: if we want postscript output
+        mp3: if we want mp3 output, only applicable if the lilypond has midi output defined
+        ogg: if we want ogg output, only applicable if the lilypond has midi output defined
+        midi_gain: the gain for use during the midi to wav conversion
 
     Returns:
-        LilypondConvertOutput: information about the file names that were outputted
+        Information about the file names that were outputted
     """
-    output_prefix = output_prefix or os.path.splitext(lilypond_filename)[0]
-    if output_prefix[-1:] == '/':
-        output_prefix += 'lilypond'
+    if not output_basename:
+        output_basename = lilypond_in.parent / lilypond_in.stem
 
-    typeset_results = lilypond(lilypond_filename, output_prefix, pdf=pdf, png=png, ps=ps)
+    typeset_results = typeset_lilypond(lilypond_in, output_basename, pdf=pdf, png=png, ps=ps)
 
     wav_list = []
     mp3_list = []
     ogg_list = []
 
-    if sound_font:
-        pool = multiprocessing.Pool(processes=6)
-        results = pool.map(_convert_midi, [{'midi_file': midi_file,
-                                            'sound_font': sound_font,
-                                            'midi_gain': midi_gain,
-                                            'mp3': mp3,
-                                            'ogg': ogg} for midi_file in typeset_results.midi_list])
-
-        for result in results:
-            wav_list.append(result['wav'])
-            if mp3:
-                mp3_list.append(result['mp3'])
-
-            if ogg:
-                ogg_list.append(result['ogg'])
-
-    return ConvertLilypondResults(typeset_results, wav_list, mp3_list, ogg_list)
-
-
-def _convert_midi(info):
-    """Small utility for use in multiprocessing. This converts midi to wav, mp3 and ogg."""
-    midi_file = info['midi_file']
-    sound_font = info['sound_font']
-    midi_gain = info['midi_gain']
+    with ThreadPoolExecutor() as executor:
+        for midi_conversion_result in executor.map(lambda midi_file: _convert_midi(midi_file, soundfont=soundfont,
+                                                                                   midi_gain=midi_gain,
+                                                                                   output_mp3=mp3, output_ogg=ogg),
+                                                   typeset_results.midi_list):
+            wav_list.append(midi_conversion_result['wav'])
+            if 'mp3' in midi_conversion_result:
+                mp3_list.append(midi_conversion_result['mp3'])
+            if 'ogg' in midi_conversion_result:
+                ogg_list.append(midi_conversion_result['ogg'])
+
+    return AutoConvertLilypondResults(typeset_results, wav_list, mp3_list, ogg_list)
+
+
+def _convert_midi(midi_in: Path, soundfont: Path | None = None,
+                  midi_gain: float | None = None, output_mp3: bool = True,
+                  output_ogg: bool = True) -> dict[str, Path]:
+    """Small utility for use in multiprocessing, converting midi to wav, mp3 and ogg.
 
-    results = {}
+    Args:
+        midi_in: the input midi file to convert
+        soundfont: the optional soundfont to use
+        midi_gain: the midi gain for midi conversion
+        output_mp3: if we want to output mp3
+        output_ogg: if we want to output ogg
 
-    wav_file = os.path.splitext(midi_file)[0] + '.wav'
-    midi_to_wav(midi_file, wav_file, sound_font, gain=midi_gain)
+    Returns:
+        A dictionary with at least the key "wav" and optionally the keys "mp3" and "ogg".
+    """
+    results = {}
 
+    wav_file = midi_in.with_suffix('.wav')
+    midi_to_wav(midi_in, wav_file, soundfont, gain=midi_gain)
     results['wav'] = wav_file
 
-    if info['mp3']:
-        mp3_file = os.path.splitext(midi_file)[0] + '.mp3'
+    if output_mp3:
+        mp3_file = wav_file.with_suffix('.mp3')
         wav_to_mp3(wav_file, mp3_file)
         results['mp3'] = mp3_file
 
-    if info['ogg']:
-        ogg_file = os.path.splitext(midi_file)[0] + '.ogg'
+    if output_ogg:
+        ogg_file = wav_file.with_suffix('.ogg')
         wav_to_ogg(wav_file, ogg_file)
         results['ogg'] = ogg_file
 
     return results
 
 
-class ConvertLilypondResults(object):
-
-    def __init__(self, typeset_results, wav_list, mp3_list, ogg_list):
-        """The output object from converting a lilypond file to the most common outputs.
+@dataclass(frozen=True, slots=True)
+class AutoConvertLilypondResults:
+    """Results from converting the lilypond input to common output files.
 
-        Args:
-            typeset_results (TypesetResults): the original typeset results
-            wav_list (list of str): the location of the wav files
-            mp3_list (list of str): the location of the mp3 files
-            ogg_list (list of str): the location of the ogg files
-        """
-        self.typeset_results = typeset_results
-        self.wav_list = wav_list
-        self.mp3_list = mp3_list
-        self.ogg_list = ogg_list
+    Args:
+        typeset_results: the typeset musical scores output
+        wav_list: list of generated wav files
+        mp3_list: list of generated mp3 files
+        ogg_list: list of generated ogg files
+    """
+    typeset_results: LilypondTypesetResults
+    wav_list: list[Path]
+    mp3_list: list[Path]
+    ogg_list: list[Path]
 
     @property
     def pdf_list(self):
         return self.typeset_results.pdf_list
 
     @property
     def png_list(self):
```

### Comparing `musical_games-0.5.2/scripts/kirnberger_meneut_trio.py` & `musical_games-0.6.1/scripts/demo_cpe_bach.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 __author__ = 'Robbert Harms'
 __date__ = '2021-03-09'
 __maintainer__ = 'Robbert Harms'
 __email__ = 'robbert@xkls.nl'
 __licence__ = 'LGPL v3'
 
-from musical_games.dice_games.dice_games import KirnbergerMenuetTrio
-from musical_games.dice_games.typesetting import MidiSettings
+from pathlib import Path
+from musical_games.dice_games.dice_games import CPEBachCounterpoint
 from musical_games.utils import auto_convert_lilypond_file
 
-dice_game = KirnbergerMenuetTrio()
+out_dir = Path('/tmp/test2')
 
-dice_game.typeset_bars_overview({'large_page': True}, '/tmp/test/overview.ly')
-auto_convert_lilypond_file('/tmp/test/overview.ly')
+dice_game = CPEBachCounterpoint()
 
-dice_game.typeset_single_bar('menuet', 1, out_file='/tmp/test/bar_menuet_1.ly')
-auto_convert_lilypond_file('/tmp/test/bar_menuet_1.ly')
-dice_game.typeset_single_bar('trio', 1, out_file='/tmp/test/bar_trio_1.ly')
-auto_convert_lilypond_file('/tmp/test/bar_trio_1.ly')
-
-print(dice_game.game_mechanics.get_all_duplicate_bars('menuet'))
-print(dice_game.game_mechanics.count_unique_compositions(count_duplicates=True))
-print(dice_game.game_mechanics.count_unique_compositions(count_duplicates=False))
-
-dice_game.typeset_composition_pdf(
-    dice_game.game_mechanics.get_random_bar_nmrs(seed=0),
-    render_settings={'comment': 'Test'},
-    out_file='/tmp/test/composition_pdf.ly')
-
-auto_convert_lilypond_file('/tmp/test/composition_pdf.ly')
-
-dice_game.typeset_composition_midi(
-    dice_game.game_mechanics.get_random_bar_nmrs(seed=0),
-    render_settings={'menuet_bass_midi_settings': MidiSettings('flute', 0, 1)},
-    out_file='/tmp/test/composition_midi.ly')
+dice_game.compile_bars_overview(single_page=True).to_file(out_dir / 'overview.ly')
+auto_convert_lilypond_file(out_dir / 'overview.ly')
+
+dice_game.compile_single_bar('treble', 1).to_file(out_dir / 'bar_treble_1.ly')
+auto_convert_lilypond_file(out_dir / 'bar_treble_1.ly')
+dice_game.compile_single_bar('bass', 1).to_file(out_dir / 'bar_bass_1.ly')
+auto_convert_lilypond_file(out_dir / 'bar_bass_1.ly')
+
+print(dice_game.get_all_duplicate_bars())
+print(dice_game.count_unique_compositions(count_duplicates=True))
+print(dice_game.count_unique_compositions(count_duplicates=False))
+
+dice_game.compile_composition_score(dice_game.get_random_bar_selection(seed=0),
+                                    comment='Test').to_file(out_dir / 'composition_pdf.ly')
+auto_convert_lilypond_file(out_dir / 'composition_pdf.ly')
+
+midi_settings = dice_game.get_default_midi_settings()
+my_midi_settings = midi_settings.with_updated_instrument('flute', 'treble', 'piano_right_hand')
+
+dice_game.compile_composition_audio(
+    dice_game.get_random_bar_selection(seed=0),
+    midi_settings=my_midi_settings).to_file(out_dir / 'composition_midi.ly')
+
+auto_convert_lilypond_file(
+    out_dir / 'composition_midi.ly',
+    soundfont=Path('/home/robbert/programming/python/opus_infinity.org/soundfonts/Musyng_Kite.sf2'))
 
-auto_convert_lilypond_file('/tmp/test/composition_midi.ly',
-                           sound_font='/home/robbert/programming/python/opus_infinity.org/soundfonts/Musyng_Kite.sf2')
```

### Comparing `musical_games-0.5.2/scripts/mozart_waltz.py` & `musical_games-0.6.1/scripts/demo_mozart_waltz.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,40 @@
 __author__ = 'Robbert Harms'
 __date__ = '2021-03-09'
 __maintainer__ = 'Robbert Harms'
 __email__ = 'robbert@xkls.nl'
 __licence__ = 'LGPL v3'
 
+from pathlib import Path
+
 from musical_games.dice_games.dice_games import MozartWaltz
-from musical_games.dice_games.typesetting import MidiSettings
 from musical_games.utils import auto_convert_lilypond_file
 
+out_dir = Path('/tmp/test2')
+
 dice_game = MozartWaltz()
 
-dice_game.typeset_bars_overview(render_settings={'large_page': True}, out_file='/tmp/test/overview.ly')
-auto_convert_lilypond_file('/tmp/test/overview.ly')
+dice_game.compile_bars_overview(single_page=True).to_file(out_dir / 'overview.ly')
+auto_convert_lilypond_file(out_dir / 'overview.ly')
 
-dice_game.typeset_single_bar('waltz', 5, out_file='/tmp/test/bar_waltz_1.ly')
-auto_convert_lilypond_file('/tmp/test/bar_waltz_1.ly')
+dice_game.compile_single_bar('waltz', 5).to_file(out_dir / 'bar_waltz_1.ly')
+auto_convert_lilypond_file(out_dir / 'bar_waltz_1.ly')
 
-print(dice_game.game_mechanics.get_all_duplicate_bars('waltz'))
-print(dice_game.game_mechanics.count_unique_compositions(count_duplicates=True))
-print(dice_game.game_mechanics.count_unique_compositions(count_duplicates=False))
-
-dice_game.typeset_composition_pdf(
-    dice_game.game_mechanics.get_random_bar_nmrs(seed=0),
-    render_settings={'comment': 'Test'},
-    out_file='/tmp/test/composition_pdf.ly')
-auto_convert_lilypond_file('/tmp/test/composition_pdf.ly')
-
-dice_game.typeset_composition_midi(
-    dice_game.game_mechanics.get_random_bar_nmrs(seed=0),
-    render_settings={'piano_rh_midi_settings': MidiSettings('violin', 0, 1)},
-    out_file='/tmp/test/composition_midi.ly')
+print(dice_game.get_all_duplicate_bars())
+print(dice_game.count_unique_compositions(count_duplicates=True))
+print(dice_game.count_unique_compositions(count_duplicates=False))
+
+dice_game.compile_composition_score(dice_game.get_random_bar_selection(seed=0),
+                                    comment='Test', single_page=True).to_file(out_dir / 'composition_pdf.ly')
+auto_convert_lilypond_file(out_dir / 'composition_pdf.ly')
+
+midi_settings = dice_game.get_default_midi_settings()
+my_midi_settings = midi_settings.with_updated_instrument('flute', 'waltz', 'piano_right_hand')
+
+dice_game.compile_composition_audio(
+    dice_game.get_random_bar_selection(seed=0),
+    midi_settings=my_midi_settings).to_file(out_dir / 'composition_midi.ly')
+
+auto_convert_lilypond_file(
+    out_dir / 'composition_midi.ly',
+    soundfont=Path('/home/robbert/programming/python/opus_infinity.org/soundfonts/Musyng_Kite.sf2'))
 
-auto_convert_lilypond_file('/tmp/test/composition_midi.ly',
-                           sound_font='/home/robbert/programming/python/opus_infinity.org/soundfonts/Musyng_Kite.sf2')
```

### Comparing `musical_games-0.5.2/scripts/stadler_meneut_trio.py` & `musical_games-0.6.1/scripts/demo_stadler_meneut_trio.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 __author__ = 'Robbert Harms'
 __date__ = '2021-03-09'
 __maintainer__ = 'Robbert Harms'
 __email__ = 'robbert@xkls.nl'
 __licence__ = 'LGPL v3'
 
+from pathlib import Path
 
 from musical_games.dice_games.dice_games import StadlerMenuetTrio
-from musical_games.dice_games.typesetting import MidiSettings
 from musical_games.utils import auto_convert_lilypond_file
 
-dice_game = StadlerMenuetTrio()
+out_dir = Path('/tmp/test2')
 
-dice_game.typeset_bars_overview(render_settings={'large_page': True}, out_file='/tmp/test/overview.ly')
-auto_convert_lilypond_file('/tmp/test/overview.ly')
+dice_game = StadlerMenuetTrio()
 
-dice_game.typeset_single_bar('menuet', 1, out_file='/tmp/test/bar_menuet_1.ly')
-auto_convert_lilypond_file('/tmp/test/bar_menuet_1.ly')
-dice_game.typeset_single_bar('trio', 1, out_file='/tmp/test/bar_trio_1.ly')
-auto_convert_lilypond_file('/tmp/test/bar_trio_1.ly')
-
-print(dice_game.game_mechanics.get_all_duplicate_bars('menuet'))
-print(dice_game.game_mechanics.count_unique_compositions(count_duplicates=True))
-print(dice_game.game_mechanics.count_unique_compositions(count_duplicates=False))
-
-dice_game.typeset_composition_pdf(
-    dice_game.game_mechanics.get_random_bar_nmrs(seed=0),
-    render_settings={'large_page': True, 'comment': 'Test'},
-    out_file='/tmp/test/composition_pdf.ly')
-auto_convert_lilypond_file('/tmp/test/composition_pdf.ly')
-
-dice_game.typeset_composition_midi(
-    dice_game.game_mechanics.get_random_bar_nmrs(seed=0),
-    render_settings={'menuet_treble_midi_settings': MidiSettings('violin', 0, 1)},
-    out_file='/tmp/test/composition_midi.ly')
+dice_game.compile_bars_overview(single_page=True).to_file(out_dir / 'overview.ly')
+auto_convert_lilypond_file(out_dir / 'overview.ly')
 
-auto_convert_lilypond_file('/tmp/test/composition_midi.ly',
-                           sound_font='/home/robbert/programming/python/opus_infinity.org/soundfonts/Musyng_Kite.sf2')
+dice_game.compile_single_bar('menuet', 1).to_file(out_dir / 'bar_menuet_1.ly')
+auto_convert_lilypond_file(out_dir / 'bar_menuet_1.ly')
+dice_game.compile_single_bar('trio', 1).to_file(out_dir / 'bar_trio_1.ly')
+auto_convert_lilypond_file(out_dir / 'bar_trio_1.ly')
+
+print(dice_game.get_all_duplicate_bars())
+print(dice_game.count_unique_compositions(count_duplicates=True))
+print(dice_game.count_unique_compositions(count_duplicates=False))
+
+dice_game.compile_composition_score(dice_game.get_random_bar_selection(seed=0),
+                                    comment='Test', single_page=True).to_file(out_dir / 'composition_pdf.ly')
+auto_convert_lilypond_file(out_dir / 'composition_pdf.ly')
+
+midi_settings = dice_game.get_default_midi_settings()
+my_midi_settings = midi_settings.with_updated_instrument('flute', 'menuet', 'piano_right_hand')
+
+dice_game.compile_composition_audio(
+    dice_game.get_random_bar_selection(seed=0),
+    midi_settings=my_midi_settings).to_file(out_dir / 'composition_midi.ly')
+
+auto_convert_lilypond_file(
+    out_dir / 'composition_midi.ly',
+    soundfont=Path('/home/robbert/programming/python/opus_infinity.org/soundfonts/Musyng_Kite.sf2'))
```

