# Comparing `tmp/xklb-2.6.3.tar.gz` & `tmp/xklb-2.6.5.tar.gz`

## Comparing `xklb-2.6.3.tar` & `xklb-2.6.5.tar`

### file list

```diff
@@ -1,123 +1,123 @@
--rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.6.3/.gitattributes
--rw-r--r--   0        0        0   196596 2020-02-02 00:00:00.000000 xklb-2.6.3/pdm.lock
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.6.3/.github/FUNDING.yml
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.6.3/.github/LICENSE
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 xklb-2.6.3/.github/Windows.md
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.6.3/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.6.3/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.6.3/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.6.3/.github/examples/extract.svg
--rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.6.3/.github/examples/tubeadd.svg
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.6.3/.github/workflows/green.yaml
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 xklb-2.6.3/.github/workflows/push.yaml
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/__init__.py
--rw-r--r--   0        0        0    18761 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/db_media.py
--rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/db_playlists.py
--rw-r--r--   0        0        0    12781 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/dl_extract.py
--rw-r--r--   0        0        0    15660 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/fs_extract.py
--rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/gdl_backend.py
--rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/gdl_extract.py
--rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/history.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/hn_extract.py
--rw-r--r--   0        0        0    13522 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/lb.py
--rw-r--r--   0        0        0    18970 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/play_actions.py
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/post_actions.py
--rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/readme.py
--rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/reddit_extract.py
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/rss_extract.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/search.py
--rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/site_extract.py
--rw-r--r--   0        0        0     5977 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/tabs_actions.py
--rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/tabs_extract.py
--rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/tube_backend.py
--rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/tube_extract.py
--rw-r--r--   0        0        0   115867 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/usage.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/data/__init__.py
--rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/data/imagemagick_errors.py
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/data/wordbank.py
--rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/data/yt_dlp_errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/media/__init__.py
--rw-r--r--   0        0        0     9128 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/media/av.py
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/media/books.py
--rw-r--r--   0        0        0    20846 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/media/dedupe.py
--rw-r--r--   0        0        0     6760 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/media/media_check.py
--rw-r--r--   0        0        0    23467 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/media/media_player.py
--rw-r--r--   0        0        0     9756 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/media/media_printer.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/media/subtitle.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scratch/__init__.py
--rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scratch/javguru.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scratch/javtiful.py
--rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scratch/mam_search.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scratch/mam_slots.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/__init__.py
--rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/add_row.py
--rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/big_dirs.py
--rw-r--r--   0        0        0    11643 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/block.py
--rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/christen.py
--rw-r--r--   0        0        0    13461 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/cluster_sort.py
--rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/copy_play_counts.py
--rw-r--r--   0        0        0    13762 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/dedupe_czkawka.py
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/dedupe_db.py
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/disk_usage.py
--rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/download_status.py
--rw-r--r--   0        0        0     7441 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/eda.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/export_text.py
--rw-r--r--   0        0        0     6810 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/history.py
--rw-r--r--   0        0        0     4380 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/incremental_diff.py
--rw-r--r--   0        0        0    10660 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/links_db.py
--rw-r--r--   0        0        0     8184 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/mcda.py
--rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/merge_dbs.py
--rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/merge_folders.py
--rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/merge_online_local.py
--rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/move_list.py
--rw-r--r--   0        0        0     6751 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/open_links.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/optimize_db.py
--rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/places_import.py
--rw-r--r--   0        0        0     9944 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/playback_control.py
--rw-r--r--   0        0        0     5812 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/playlists.py
--rw-r--r--   0        0        0     7326 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/process_ffmpeg.py
--rw-r--r--   0        0        0     2797 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/process_image.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/redownload.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/rel_mv.py
--rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/sample_compare.py
--rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/sample_hash.py
--rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/scatter.py
--rw-r--r--   0        0        0     2581 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/search_db.py
--rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/streaming_tab_loader.py
--rw-r--r--   0        0        0     9759 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/web_add.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/mining/__init__.py
--rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/mining/extract_links.py
--rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/mining/extract_text.py
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/mining/markdown_links.py
--rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/mining/mpv_watchlater.py
--rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/mining/nouns.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/mining/pushshift.py
--rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/mining/reddit_selftext.py
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/mining/substack.py
--rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/scripts/mining/tildes.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/__init__.py
--rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/arg_utils.py
--rw-r--r--   0        0        0    17266 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/arggroups.py
--rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/argparse_utils.py
--rw-r--r--   0        0        0    10523 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/consts.py
--rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/db_utils.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/devices.py
--rw-r--r--   0        0        0    15122 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/file_utils.py
--rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/gui.py
--rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/iterables.py
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/log_utils.py
--rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/mpv_utils.py
--rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/nums.py
--rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/objects.py
--rw-r--r--   0        0        0     3355 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/path_utils.py
--rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/pd_utils.py
--rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/printing.py
--rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/processes.py
--rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/sql_utils.py
--rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/strings.py
--rw-r--r--   0        0        0    22041 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/utils/web.py
--rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.6.3/xklb/assets/kotobago.png
--rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.6.3/.gitignore
--rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 xklb-2.6.3/pyproject.toml
--rw-r--r--   0        0        0   155708 2020-02-02 00:00:00.000000 xklb-2.6.3/.github/README.md
--rw-r--r--   0        0        0   159469 2020-02-02 00:00:00.000000 xklb-2.6.3/PKG-INFO
+-rw-r--r--   0        0        0      137 2020-02-02 00:00:00.000000 xklb-2.6.5/.gitattributes
+-rw-r--r--   0        0        0   202498 2020-02-02 00:00:00.000000 xklb-2.6.5/pdm.lock
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/FUNDING.yml
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/LICENSE
+-rw-r--r--   0        0        0     1727 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/Windows.md
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0    17854 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/examples/extract.svg
+-rw-r--r--   0        0        0    13463 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/examples/tubeadd.svg
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/workflows/green.yaml
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/workflows/push.yaml
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/__init__.py
+-rw-r--r--   0        0        0    18761 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/db_media.py
+-rw-r--r--   0        0        0     8190 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/db_playlists.py
+-rw-r--r--   0        0        0    12781 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/dl_extract.py
+-rw-r--r--   0        0        0    15664 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/fs_extract.py
+-rw-r--r--   0        0        0     8076 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/gdl_backend.py
+-rw-r--r--   0        0        0     3230 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/gdl_extract.py
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/history.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/hn_extract.py
+-rw-r--r--   0        0        0    13522 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/lb.py
+-rw-r--r--   0        0        0    19486 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/play_actions.py
+-rw-r--r--   0        0        0     7206 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/post_actions.py
+-rw-r--r--   0        0        0    13785 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/readme.py
+-rw-r--r--   0        0        0    13125 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/reddit_extract.py
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/rss_extract.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/search.py
+-rw-r--r--   0        0        0     6463 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/site_extract.py
+-rw-r--r--   0        0        0     5890 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/tabs_actions.py
+-rw-r--r--   0        0        0     5722 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/tabs_extract.py
+-rw-r--r--   0        0        0    20308 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/tube_backend.py
+-rw-r--r--   0        0        0     4059 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/tube_extract.py
+-rw-r--r--   0        0        0   118259 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/usage.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/data/__init__.py
+-rw-r--r--   0        0        0      948 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/data/imagemagick_errors.py
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/data/wordbank.py
+-rw-r--r--   0        0        0     7204 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/data/yt_dlp_errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/__init__.py
+-rw-r--r--   0        0        0     9140 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/av.py
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/books.py
+-rw-r--r--   0        0        0    20852 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/dedupe.py
+-rw-r--r--   0        0        0     6806 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/media_check.py
+-rw-r--r--   0        0        0    23467 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/media_player.py
+-rw-r--r--   0        0        0    10390 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/media_printer.py
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/media/subtitle.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scratch/__init__.py
+-rw-r--r--   0        0        0     6159 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scratch/javguru.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scratch/javtiful.py
+-rw-r--r--   0        0        0     8327 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scratch/mam_search.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scratch/mam_slots.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/__init__.py
+-rw-r--r--   0        0        0     1282 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/add_row.py
+-rw-r--r--   0        0        0     7057 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/big_dirs.py
+-rw-r--r--   0        0        0    11608 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/block.py
+-rw-r--r--   0        0        0     2717 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/christen.py
+-rw-r--r--   0        0        0    13461 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/cluster_sort.py
+-rw-r--r--   0        0        0     1957 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/copy_play_counts.py
+-rw-r--r--   0        0        0    13814 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/dedupe_czkawka.py
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/dedupe_db.py
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/disk_usage.py
+-rw-r--r--   0        0        0     3627 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/download_status.py
+-rw-r--r--   0        0        0     7498 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/eda.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/export_text.py
+-rw-r--r--   0        0        0     6810 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/history.py
+-rw-r--r--   0        0        0     4437 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/incremental_diff.py
+-rw-r--r--   0        0        0    10660 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/links_db.py
+-rw-r--r--   0        0        0     8241 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mcda.py
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/merge_dbs.py
+-rw-r--r--   0        0        0     7811 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/merge_folders.py
+-rw-r--r--   0        0        0     3695 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/merge_online_local.py
+-rw-r--r--   0        0        0     7501 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/move_list.py
+-rw-r--r--   0        0        0     6658 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/open_links.py
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/optimize_db.py
+-rw-r--r--   0        0        0     1997 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/places_import.py
+-rw-r--r--   0        0        0     9778 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/playback_control.py
+-rw-r--r--   0        0        0     5638 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/playlists.py
+-rw-r--r--   0        0        0     7478 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/process_ffmpeg.py
+-rw-r--r--   0        0        0     2885 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/process_image.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/redownload.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/rel_mv.py
+-rw-r--r--   0        0        0     3634 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/sample_compare.py
+-rw-r--r--   0        0        0     2693 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/sample_hash.py
+-rw-r--r--   0        0        0    11711 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/scatter.py
+-rw-r--r--   0        0        0     2583 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/search_db.py
+-rw-r--r--   0        0        0     2378 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/streaming_tab_loader.py
+-rw-r--r--   0        0        0     9863 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/web_add.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/__init__.py
+-rw-r--r--   0        0        0     6606 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/extract_links.py
+-rw-r--r--   0        0        0     3486 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/extract_text.py
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/markdown_links.py
+-rw-r--r--   0        0        0     1848 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/mpv_watchlater.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/nouns.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/pushshift.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/reddit_selftext.py
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/substack.py
+-rw-r--r--   0        0        0     5733 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/scripts/mining/tildes.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/__init__.py
+-rw-r--r--   0        0        0     6202 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/arg_utils.py
+-rw-r--r--   0        0        0    17735 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/arggroups.py
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/argparse_utils.py
+-rw-r--r--   0        0        0    10529 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/consts.py
+-rw-r--r--   0        0        0    11248 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/db_utils.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/devices.py
+-rw-r--r--   0        0        0    15276 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/file_utils.py
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/gui.py
+-rw-r--r--   0        0        0     4574 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/iterables.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/log_utils.py
+-rw-r--r--   0        0        0     2237 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/mpv_utils.py
+-rw-r--r--   0        0        0     4023 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/nums.py
+-rw-r--r--   0        0        0     3714 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/objects.py
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/path_utils.py
+-rw-r--r--   0        0        0      787 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/pd_utils.py
+-rw-r--r--   0        0        0     7418 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/printing.py
+-rw-r--r--   0        0        0     7051 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/processes.py
+-rw-r--r--   0        0        0     8306 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/sql_utils.py
+-rw-r--r--   0        0        0     6170 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/strings.py
+-rw-r--r--   0        0        0    22041 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/utils/web.py
+-rw-r--r--   0        0        0     8385 2020-02-02 00:00:00.000000 xklb-2.6.5/xklb/assets/kotobago.png
+-rw-r--r--   0        0        0     1504 2020-02-02 00:00:00.000000 xklb-2.6.5/.gitignore
+-rw-r--r--   0        0        0     3111 2020-02-02 00:00:00.000000 xklb-2.6.5/pyproject.toml
+-rw-r--r--   0        0        0   158100 2020-02-02 00:00:00.000000 xklb-2.6.5/.github/README.md
+-rw-r--r--   0        0        0   161861 2020-02-02 00:00:00.000000 xklb-2.6.5/PKG-INFO
```

### Comparing `xklb-2.6.3/pdm.lock` & `xklb-2.6.5/pdm.lock`

 * *Files 1% similar despite different names*

```diff
@@ -5,72 +5,72 @@
 groups = ["default", "deluxe", "test"]
 strategy = ["cross_platform"]
 lock_version = "4.4.1"
 content_hash = "sha256:b2b7a02304f39d3e9958315a1f0c3230799c9e4cda0d0f411634c2057b9b871a"
 
 [[package]]
 name = "aiohttp"
-version = "3.9.3"
+version = "3.9.4"
 requires_python = ">=3.8"
 summary = "Async http client/server framework (asyncio)"
 dependencies = [
     "aiosignal>=1.1.2",
     "async-timeout<5.0,>=4.0; python_version < \"3.11\"",
     "attrs>=17.3.0",
     "frozenlist>=1.1.1",
     "multidict<7.0,>=4.5",
     "yarl<2.0,>=1.0",
 ]
 files = [
-    {file = "aiohttp-3.9.3-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:939677b61f9d72a4fa2a042a5eee2a99a24001a67c13da113b2e30396567db54"},
-    {file = "aiohttp-3.9.3-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:1f5cd333fcf7590a18334c90f8c9147c837a6ec8a178e88d90a9b96ea03194cc"},
-    {file = "aiohttp-3.9.3-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:82e6aa28dd46374f72093eda8bcd142f7771ee1eb9d1e223ff0fa7177a96b4a5"},
-    {file = "aiohttp-3.9.3-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:f56455b0c2c7cc3b0c584815264461d07b177f903a04481dfc33e08a89f0c26b"},
-    {file = "aiohttp-3.9.3-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:bca77a198bb6e69795ef2f09a5f4c12758487f83f33d63acde5f0d4919815768"},
-    {file = "aiohttp-3.9.3-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:e083c285857b78ee21a96ba1eb1b5339733c3563f72980728ca2b08b53826ca5"},
-    {file = "aiohttp-3.9.3-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ab40e6251c3873d86ea9b30a1ac6d7478c09277b32e14745d0d3c6e76e3c7e29"},
-    {file = "aiohttp-3.9.3-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:df822ee7feaaeffb99c1a9e5e608800bd8eda6e5f18f5cfb0dc7eeb2eaa6bbec"},
-    {file = "aiohttp-3.9.3-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:acef0899fea7492145d2bbaaaec7b345c87753168589cc7faf0afec9afe9b747"},
-    {file = "aiohttp-3.9.3-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:cd73265a9e5ea618014802ab01babf1940cecb90c9762d8b9e7d2cc1e1969ec6"},
-    {file = "aiohttp-3.9.3-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:a78ed8a53a1221393d9637c01870248a6f4ea5b214a59a92a36f18151739452c"},
-    {file = "aiohttp-3.9.3-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:6b0e029353361f1746bac2e4cc19b32f972ec03f0f943b390c4ab3371840aabf"},
-    {file = "aiohttp-3.9.3-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:7cf5c9458e1e90e3c390c2639f1017a0379a99a94fdfad3a1fd966a2874bba52"},
-    {file = "aiohttp-3.9.3-cp310-cp310-win32.whl", hash = "sha256:3e59c23c52765951b69ec45ddbbc9403a8761ee6f57253250c6e1536cacc758b"},
-    {file = "aiohttp-3.9.3-cp310-cp310-win_amd64.whl", hash = "sha256:055ce4f74b82551678291473f66dc9fb9048a50d8324278751926ff0ae7715e5"},
-    {file = "aiohttp-3.9.3-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:6b88f9386ff1ad91ace19d2a1c0225896e28815ee09fc6a8932fded8cda97c3d"},
-    {file = "aiohttp-3.9.3-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:c46956ed82961e31557b6857a5ca153c67e5476972e5f7190015018760938da2"},
-    {file = "aiohttp-3.9.3-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:07b837ef0d2f252f96009e9b8435ec1fef68ef8b1461933253d318748ec1acdc"},
-    {file = "aiohttp-3.9.3-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:dad46e6f620574b3b4801c68255492e0159d1712271cc99d8bdf35f2043ec266"},
-    {file = "aiohttp-3.9.3-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:5ed3e046ea7b14938112ccd53d91c1539af3e6679b222f9469981e3dac7ba1ce"},
-    {file = "aiohttp-3.9.3-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:039df344b45ae0b34ac885ab5b53940b174530d4dd8a14ed8b0e2155b9dddccb"},
-    {file = "aiohttp-3.9.3-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7943c414d3a8d9235f5f15c22ace69787c140c80b718dcd57caaade95f7cd93b"},
-    {file = "aiohttp-3.9.3-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:84871a243359bb42c12728f04d181a389718710129b36b6aad0fc4655a7647d4"},
-    {file = "aiohttp-3.9.3-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:5eafe2c065df5401ba06821b9a054d9cb2848867f3c59801b5d07a0be3a380ae"},
-    {file = "aiohttp-3.9.3-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:9d3c9b50f19704552f23b4eaea1fc082fdd82c63429a6506446cbd8737823da3"},
-    {file = "aiohttp-3.9.3-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:f033d80bc6283092613882dfe40419c6a6a1527e04fc69350e87a9df02bbc283"},
-    {file = "aiohttp-3.9.3-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:2c895a656dd7e061b2fd6bb77d971cc38f2afc277229ce7dd3552de8313a483e"},
-    {file = "aiohttp-3.9.3-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:1f5a71d25cd8106eab05f8704cd9167b6e5187bcdf8f090a66c6d88b634802b4"},
-    {file = "aiohttp-3.9.3-cp311-cp311-win32.whl", hash = "sha256:50fca156d718f8ced687a373f9e140c1bb765ca16e3d6f4fe116e3df7c05b2c5"},
-    {file = "aiohttp-3.9.3-cp311-cp311-win_amd64.whl", hash = "sha256:5fe9ce6c09668063b8447f85d43b8d1c4e5d3d7e92c63173e6180b2ac5d46dd8"},
-    {file = "aiohttp-3.9.3-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:38a19bc3b686ad55804ae931012f78f7a534cce165d089a2059f658f6c91fa60"},
-    {file = "aiohttp-3.9.3-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:770d015888c2a598b377bd2f663adfd947d78c0124cfe7b959e1ef39f5b13869"},
-    {file = "aiohttp-3.9.3-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:ee43080e75fc92bf36219926c8e6de497f9b247301bbf88c5c7593d931426679"},
-    {file = "aiohttp-3.9.3-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:52df73f14ed99cee84865b95a3d9e044f226320a87af208f068ecc33e0c35b96"},
-    {file = "aiohttp-3.9.3-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:dc9b311743a78043b26ffaeeb9715dc360335e5517832f5a8e339f8a43581e4d"},
-    {file = "aiohttp-3.9.3-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:b955ed993491f1a5da7f92e98d5dad3c1e14dc175f74517c4e610b1f2456fb11"},
-    {file = "aiohttp-3.9.3-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:504b6981675ace64c28bf4a05a508af5cde526e36492c98916127f5a02354d53"},
-    {file = "aiohttp-3.9.3-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a6fe5571784af92b6bc2fda8d1925cccdf24642d49546d3144948a6a1ed58ca5"},
-    {file = "aiohttp-3.9.3-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:ba39e9c8627edc56544c8628cc180d88605df3892beeb2b94c9bc857774848ca"},
-    {file = "aiohttp-3.9.3-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:e5e46b578c0e9db71d04c4b506a2121c0cb371dd89af17a0586ff6769d4c58c1"},
-    {file = "aiohttp-3.9.3-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:938a9653e1e0c592053f815f7028e41a3062e902095e5a7dc84617c87267ebd5"},
-    {file = "aiohttp-3.9.3-cp312-cp312-musllinux_1_1_s390x.whl", hash = "sha256:c3452ea726c76e92f3b9fae4b34a151981a9ec0a4847a627c43d71a15ac32aa6"},
-    {file = "aiohttp-3.9.3-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:ff30218887e62209942f91ac1be902cc80cddb86bf00fbc6783b7a43b2bea26f"},
-    {file = "aiohttp-3.9.3-cp312-cp312-win32.whl", hash = "sha256:38f307b41e0bea3294a9a2a87833191e4bcf89bb0365e83a8be3a58b31fb7f38"},
-    {file = "aiohttp-3.9.3-cp312-cp312-win_amd64.whl", hash = "sha256:b791a3143681a520c0a17e26ae7465f1b6f99461a28019d1a2f425236e6eedb5"},
-    {file = "aiohttp-3.9.3.tar.gz", hash = "sha256:90842933e5d1ff760fae6caca4b2b3edba53ba8f4b71e95dacf2818a2aca06f7"},
+    {file = "aiohttp-3.9.4-cp310-cp310-macosx_10_9_universal2.whl", hash = "sha256:76d32588ef7e4a3f3adff1956a0ba96faabbdee58f2407c122dd45aa6e34f372"},
+    {file = "aiohttp-3.9.4-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:56181093c10dbc6ceb8a29dfeea1e815e1dfdc020169203d87fd8d37616f73f9"},
+    {file = "aiohttp-3.9.4-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:c7a5b676d3c65e88b3aca41816bf72831898fcd73f0cbb2680e9d88e819d1e4d"},
+    {file = "aiohttp-3.9.4-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d1df528a85fb404899d4207a8d9934cfd6be626e30e5d3a5544a83dbae6d8a7e"},
+    {file = "aiohttp-3.9.4-cp310-cp310-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:f595db1bceabd71c82e92df212dd9525a8a2c6947d39e3c994c4f27d2fe15b11"},
+    {file = "aiohttp-3.9.4-cp310-cp310-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:9c0b09d76e5a4caac3d27752027fbd43dc987b95f3748fad2b924a03fe8632ad"},
+    {file = "aiohttp-3.9.4-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:689eb4356649ec9535b3686200b231876fb4cab4aca54e3bece71d37f50c1d13"},
+    {file = "aiohttp-3.9.4-cp310-cp310-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:a3666cf4182efdb44d73602379a66f5fdfd5da0db5e4520f0ac0dcca644a3497"},
+    {file = "aiohttp-3.9.4-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:b65b0f8747b013570eea2f75726046fa54fa8e0c5db60f3b98dd5d161052004a"},
+    {file = "aiohttp-3.9.4-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:a1885d2470955f70dfdd33a02e1749613c5a9c5ab855f6db38e0b9389453dce7"},
+    {file = "aiohttp-3.9.4-cp310-cp310-musllinux_1_1_ppc64le.whl", hash = "sha256:0593822dcdb9483d41f12041ff7c90d4d1033ec0e880bcfaf102919b715f47f1"},
+    {file = "aiohttp-3.9.4-cp310-cp310-musllinux_1_1_s390x.whl", hash = "sha256:47f6eb74e1ecb5e19a78f4a4228aa24df7fbab3b62d4a625d3f41194a08bd54f"},
+    {file = "aiohttp-3.9.4-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:c8b04a3dbd54de6ccb7604242fe3ad67f2f3ca558f2d33fe19d4b08d90701a89"},
+    {file = "aiohttp-3.9.4-cp310-cp310-win32.whl", hash = "sha256:8a78dfb198a328bfb38e4308ca8167028920fb747ddcf086ce706fbdd23b2926"},
+    {file = "aiohttp-3.9.4-cp310-cp310-win_amd64.whl", hash = "sha256:e78da6b55275987cbc89141a1d8e75f5070e577c482dd48bd9123a76a96f0bbb"},
+    {file = "aiohttp-3.9.4-cp311-cp311-macosx_10_9_universal2.whl", hash = "sha256:c111b3c69060d2bafc446917534150fd049e7aedd6cbf21ba526a5a97b4402a5"},
+    {file = "aiohttp-3.9.4-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:efbdd51872cf170093998c87ccdf3cb5993add3559341a8e5708bcb311934c94"},
+    {file = "aiohttp-3.9.4-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:7bfdb41dc6e85d8535b00d73947548a748e9534e8e4fddd2638109ff3fb081df"},
+    {file = "aiohttp-3.9.4-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2bd9d334412961125e9f68d5b73c1d0ab9ea3f74a58a475e6b119f5293eee7ba"},
+    {file = "aiohttp-3.9.4-cp311-cp311-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:35d78076736f4a668d57ade00c65d30a8ce28719d8a42471b2a06ccd1a2e3063"},
+    {file = "aiohttp-3.9.4-cp311-cp311-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:824dff4f9f4d0f59d0fa3577932ee9a20e09edec8a2f813e1d6b9f89ced8293f"},
+    {file = "aiohttp-3.9.4-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:52b8b4e06fc15519019e128abedaeb56412b106ab88b3c452188ca47a25c4093"},
+    {file = "aiohttp-3.9.4-cp311-cp311-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:eae569fb1e7559d4f3919965617bb39f9e753967fae55ce13454bec2d1c54f09"},
+    {file = "aiohttp-3.9.4-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:69b97aa5792428f321f72aeb2f118e56893371f27e0b7d05750bcad06fc42ca1"},
+    {file = "aiohttp-3.9.4-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:4d79aad0ad4b980663316f26d9a492e8fab2af77c69c0f33780a56843ad2f89e"},
+    {file = "aiohttp-3.9.4-cp311-cp311-musllinux_1_1_ppc64le.whl", hash = "sha256:d6577140cd7db19e430661e4b2653680194ea8c22c994bc65b7a19d8ec834403"},
+    {file = "aiohttp-3.9.4-cp311-cp311-musllinux_1_1_s390x.whl", hash = "sha256:9860d455847cd98eb67897f5957b7cd69fbcb436dd3f06099230f16a66e66f79"},
+    {file = "aiohttp-3.9.4-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:69ff36d3f8f5652994e08bd22f093e11cfd0444cea310f92e01b45a4e46b624e"},
+    {file = "aiohttp-3.9.4-cp311-cp311-win32.whl", hash = "sha256:e27d3b5ed2c2013bce66ad67ee57cbf614288bda8cdf426c8d8fe548316f1b5f"},
+    {file = "aiohttp-3.9.4-cp311-cp311-win_amd64.whl", hash = "sha256:d6a67e26daa686a6fbdb600a9af8619c80a332556245fa8e86c747d226ab1a1e"},
+    {file = "aiohttp-3.9.4-cp312-cp312-macosx_10_9_universal2.whl", hash = "sha256:c5ff8ff44825736a4065d8544b43b43ee4c6dd1530f3a08e6c0578a813b0aa35"},
+    {file = "aiohttp-3.9.4-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:d12a244627eba4e9dc52cbf924edef905ddd6cafc6513849b4876076a6f38b0e"},
+    {file = "aiohttp-3.9.4-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:dcad56c8d8348e7e468899d2fb3b309b9bc59d94e6db08710555f7436156097f"},
+    {file = "aiohttp-3.9.4-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:4f7e69a7fd4b5ce419238388e55abd220336bd32212c673ceabc57ccf3d05b55"},
+    {file = "aiohttp-3.9.4-cp312-cp312-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:c4870cb049f10d7680c239b55428916d84158798eb8f353e74fa2c98980dcc0b"},
+    {file = "aiohttp-3.9.4-cp312-cp312-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:3b2feaf1b7031ede1bc0880cec4b0776fd347259a723d625357bb4b82f62687b"},
+    {file = "aiohttp-3.9.4-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:939393e8c3f0a5bcd33ef7ace67680c318dc2ae406f15e381c0054dd658397de"},
+    {file = "aiohttp-3.9.4-cp312-cp312-manylinux_2_5_i686.manylinux1_i686.manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:7d2334e387b2adcc944680bebcf412743f2caf4eeebd550f67249c1c3696be04"},
+    {file = "aiohttp-3.9.4-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:e0198ea897680e480845ec0ffc5a14e8b694e25b3f104f63676d55bf76a82f1a"},
+    {file = "aiohttp-3.9.4-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:e40d2cd22914d67c84824045861a5bb0fb46586b15dfe4f046c7495bf08306b2"},
+    {file = "aiohttp-3.9.4-cp312-cp312-musllinux_1_1_ppc64le.whl", hash = "sha256:aba80e77c227f4234aa34a5ff2b6ff30c5d6a827a91d22ff6b999de9175d71bd"},
+    {file = "aiohttp-3.9.4-cp312-cp312-musllinux_1_1_s390x.whl", hash = "sha256:fb68dc73bc8ac322d2e392a59a9e396c4f35cb6fdbdd749e139d1d6c985f2527"},
+    {file = "aiohttp-3.9.4-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:f3460a92638dce7e47062cf088d6e7663adb135e936cb117be88d5e6c48c9d53"},
+    {file = "aiohttp-3.9.4-cp312-cp312-win32.whl", hash = "sha256:32dc814ddbb254f6170bca198fe307920f6c1308a5492f049f7f63554b88ef36"},
+    {file = "aiohttp-3.9.4-cp312-cp312-win_amd64.whl", hash = "sha256:63f41a909d182d2b78fe3abef557fcc14da50c7852f70ae3be60e83ff64edba5"},
+    {file = "aiohttp-3.9.4.tar.gz", hash = "sha256:6ff71ede6d9a5a58cfb7b6fffc83ab5d4a63138276c771ac91ceaaddf5459644"},
 ]
 
 [[package]]
 name = "aiosignal"
 version = "1.3.1"
 requires_python = ">=3.7"
 summary = "aiosignal: a list of registered asynchronous callbacks"
@@ -1317,14 +1317,15 @@
     {file = "pandas-2.2.2-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:8e90497254aacacbc4ea6ae5e7a8cd75629d6ad2b30025a4a8b09aa4faf55151"},
     {file = "pandas-2.2.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:58b84b91b0b9f4bafac2a0ac55002280c094dfc6402402332c0913a59654ab2b"},
     {file = "pandas-2.2.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6d2123dc9ad6a814bcdea0f099885276b31b24f7edf40f6cdbc0912672e22eee"},
     {file = "pandas-2.2.2-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:2925720037f06e89af896c70bca73459d7e6a4be96f9de79e2d440bd499fe0db"},
     {file = "pandas-2.2.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:0cace394b6ea70c01ca1595f839cf193df35d1575986e484ad35c4aeae7266c1"},
     {file = "pandas-2.2.2-cp311-cp311-win_amd64.whl", hash = "sha256:873d13d177501a28b2756375d59816c365e42ed8417b41665f346289adc68d24"},
     {file = "pandas-2.2.2-cp312-cp312-macosx_10_9_x86_64.whl", hash = "sha256:9dfde2a0ddef507a631dc9dc4af6a9489d5e2e740e226ad426a05cabfbd7c8ef"},
+    {file = "pandas-2.2.2-cp312-cp312-macosx_11_0_arm64.whl", hash = "sha256:e9b79011ff7a0f4b1d6da6a61aa1aa604fb312d6647de5bad20013682d1429ce"},
     {file = "pandas-2.2.2-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1cb51fe389360f3b5a4d57dbd2848a5f033350336ca3b340d1c53a1fad33bcad"},
     {file = "pandas-2.2.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:eee3a87076c0756de40b05c5e9a6069c035ba43e8dd71c379e68cab2c20f16ad"},
     {file = "pandas-2.2.2-cp312-cp312-musllinux_1_1_aarch64.whl", hash = "sha256:3e374f59e440d4ab45ca2fffde54b81ac3834cf5ae2cdfa69c90bc03bde04d76"},
     {file = "pandas-2.2.2-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:43498c0bdb43d55cb162cdc8c06fac328ccb5d2eabe3cadeb3529ae6f0517c32"},
     {file = "pandas-2.2.2-cp312-cp312-win_amd64.whl", hash = "sha256:d187d355ecec3629624fccb01d104da7d7f391db0311145817525281e2804d23"},
     {file = "pandas-2.2.2.tar.gz", hash = "sha256:9e79019aba43cb4fda9e4d983f8e88ca0373adbb697ae9c6c43093218de28b54"},
 ]
@@ -1892,35 +1893,35 @@
 files = [
     {file = "rich-13.7.1-py3-none-any.whl", hash = "sha256:4edbae314f59eb482f54e9e30bf00d33350aaa94f4bfcd4e9e3110e64d0d7222"},
     {file = "rich-13.7.1.tar.gz", hash = "sha256:9be308cb1fe2f1f57d67ce99e95af38a1e2bc71ad9813b0e247cf7ffbcc3a432"},
 ]
 
 [[package]]
 name = "ruff"
-version = "0.3.6"
+version = "0.3.7"
 requires_python = ">=3.7"
 summary = "An extremely fast Python linter and code formatter, written in Rust."
 files = [
-    {file = "ruff-0.3.6-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:732ef99984275534f9466fbc01121523caf72aa8c2bdeb36fd2edf2bc294a992"},
-    {file = "ruff-0.3.6-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:93699d61116807edc5ca1cdf9d2d22cf8d93335d59e3ff0ca7aee62c1818a736"},
-    {file = "ruff-0.3.6-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:fc4006cbc6c11fefc25f122d2eb4731d7a3d815dc74d67c54991cc3f99c90177"},
-    {file = "ruff-0.3.6-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:878ef1a55ce931f3ca23b690b159cd0659f495a4c231a847b00ca55e4c688baf"},
-    {file = "ruff-0.3.6-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:ecb87788284af96725643eae9ab3ac746d8cc09aad140268523b019f7ac3cd98"},
-    {file = "ruff-0.3.6-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:b2e79f8e1b6bd5411d7ddad3f2abff3f9d371beda29daef86400d416dedb7e02"},
-    {file = "ruff-0.3.6-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:cf48ec2c4bfae7837dc325c431a2932dc23a1485e71c59591c1df471ba234e0e"},
-    {file = "ruff-0.3.6-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:c466a52c522e6a08df0af018f550902f154f5649ad09e7f0d43da766e7399ebc"},
-    {file = "ruff-0.3.6-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:28ccf3fb6d1162a73cd286c63a5e4d885f46a1f99f0b392924bc95ccbd18ea8f"},
-    {file = "ruff-0.3.6-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:b11e09439d9df6cc12d9f622065834654417c40216d271f639512d80e80e3e53"},
-    {file = "ruff-0.3.6-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:647f1fb5128a3e24ce68878b8050bb55044c45bb3f3ae4710d4da9ca96ede5cb"},
-    {file = "ruff-0.3.6-py3-none-musllinux_1_2_i686.whl", hash = "sha256:2b0c4c70578ef1871a9ac5c85ed7a8c33470e976c73ba9211a111d2771b5f787"},
-    {file = "ruff-0.3.6-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:e3da499ded004d0b956ab04248b2ae17e54a67ffc81353514ac583af5959a255"},
-    {file = "ruff-0.3.6-py3-none-win32.whl", hash = "sha256:4056480f5cf38ad278667c31b0ef334c29acdfcea617cb89c4ccbc7d96f1637f"},
-    {file = "ruff-0.3.6-py3-none-win_amd64.whl", hash = "sha256:f1aa621beed533f46e9c7d6fe00e7f6e4570155b61d8f020387b72ace2b42e04"},
-    {file = "ruff-0.3.6-py3-none-win_arm64.whl", hash = "sha256:7c8a2a0e0cab077a07465259ffe3b3c090e747ca8097c5dc4c36ca0fdaaac90d"},
-    {file = "ruff-0.3.6.tar.gz", hash = "sha256:26071fb530038602b984e3bbe1443ef82a38450c4dcb1344a9caf67234ff9756"},
+    {file = "ruff-0.3.7-py3-none-macosx_10_12_x86_64.macosx_11_0_arm64.macosx_10_12_universal2.whl", hash = "sha256:0e8377cccb2f07abd25e84fc5b2cbe48eeb0fea9f1719cad7caedb061d70e5ce"},
+    {file = "ruff-0.3.7-py3-none-macosx_10_12_x86_64.whl", hash = "sha256:15a4d1cc1e64e556fa0d67bfd388fed416b7f3b26d5d1c3e7d192c897e39ba4b"},
+    {file = "ruff-0.3.7-py3-none-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:d28bdf3d7dc71dd46929fafeec98ba89b7c3550c3f0978e36389b5631b793663"},
+    {file = "ruff-0.3.7-py3-none-manylinux_2_17_armv7l.manylinux2014_armv7l.whl", hash = "sha256:379b67d4f49774ba679593b232dcd90d9e10f04d96e3c8ce4a28037ae473f7bb"},
+    {file = "ruff-0.3.7-py3-none-manylinux_2_17_i686.manylinux2014_i686.whl", hash = "sha256:c060aea8ad5ef21cdfbbe05475ab5104ce7827b639a78dd55383a6e9895b7c51"},
+    {file = "ruff-0.3.7-py3-none-manylinux_2_17_ppc64.manylinux2014_ppc64.whl", hash = "sha256:ebf8f615dde968272d70502c083ebf963b6781aacd3079081e03b32adfe4d58a"},
+    {file = "ruff-0.3.7-py3-none-manylinux_2_17_ppc64le.manylinux2014_ppc64le.whl", hash = "sha256:d48098bd8f5c38897b03604f5428901b65e3c97d40b3952e38637b5404b739a2"},
+    {file = "ruff-0.3.7-py3-none-manylinux_2_17_s390x.manylinux2014_s390x.whl", hash = "sha256:da8a4fda219bf9024692b1bc68c9cff4b80507879ada8769dc7e985755d662ea"},
+    {file = "ruff-0.3.7-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:6c44e0149f1d8b48c4d5c33d88c677a4aa22fd09b1683d6a7ff55b816b5d074f"},
+    {file = "ruff-0.3.7-py3-none-musllinux_1_2_aarch64.whl", hash = "sha256:3050ec0af72b709a62ecc2aca941b9cd479a7bf2b36cc4562f0033d688e44fa1"},
+    {file = "ruff-0.3.7-py3-none-musllinux_1_2_armv7l.whl", hash = "sha256:a29cc38e4c1ab00da18a3f6777f8b50099d73326981bb7d182e54a9a21bb4ff7"},
+    {file = "ruff-0.3.7-py3-none-musllinux_1_2_i686.whl", hash = "sha256:5b15cc59c19edca917f51b1956637db47e200b0fc5e6e1878233d3a938384b0b"},
+    {file = "ruff-0.3.7-py3-none-musllinux_1_2_x86_64.whl", hash = "sha256:e491045781b1e38b72c91247cf4634f040f8d0cb3e6d3d64d38dcf43616650b4"},
+    {file = "ruff-0.3.7-py3-none-win32.whl", hash = "sha256:bc931de87593d64fad3a22e201e55ad76271f1d5bfc44e1a1887edd0903c7d9f"},
+    {file = "ruff-0.3.7-py3-none-win_amd64.whl", hash = "sha256:5ef0e501e1e39f35e03c2acb1d1238c595b8bb36cf7a170e7c1df1b73da00e74"},
+    {file = "ruff-0.3.7-py3-none-win_arm64.whl", hash = "sha256:789e144f6dc7019d1f92a812891c645274ed08af6037d11fc65fcbc183b7d59f"},
+    {file = "ruff-0.3.7.tar.gz", hash = "sha256:d5c1aebee5162c2226784800ae031f660c350e7a3402c4d1f8ea4e97e232e3ba"},
 ]
 
 [[package]]
 name = "scikit-learn"
 version = "1.4.2"
 requires_python = ">=3.9"
 summary = "A set of python modules for machine learning and data mining"
@@ -2503,24 +2504,59 @@
 files = [
     {file = "yt_dlp-2024.4.9-py3-none-any.whl", hash = "sha256:d6ff6798bd114cc48763564fcb2f296464ec1604f731e69b07a8814c89b170a2"},
     {file = "yt_dlp-2024.4.9.tar.gz", hash = "sha256:7ee90572b4d313b582b99c89e4eccf779b57ff54edc331873c6b3fba77faa8b0"},
 ]
 
 [[package]]
 name = "zeroconf"
-version = "0.132.0"
+version = "0.132.2"
 requires_python = "<4.0,>=3.8"
 summary = "A pure python implementation of multicast DNS service discovery"
 dependencies = [
     "async-timeout>=3.0.0; python_version < \"3.11\"",
     "ifaddr>=0.1.7",
 ]
 files = [
-    {file = "zeroconf-0.132.0-cp310-cp310-manylinux_2_31_x86_64.whl", hash = "sha256:fb0a91b58b10d3a31b8324b2a8548e59c547a5c37055344c12d929f86c063d4e"},
-    {file = "zeroconf-0.132.0.tar.gz", hash = "sha256:e2dddb9b8e6a9de3c43f943d8547300e6bd49b2043fd719ae830cfe0f2908a5c"},
+    {file = "zeroconf-0.132.2-cp310-cp310-macosx_11_0_x86_64.whl", hash = "sha256:31c8406f62251aa62f5b67d865007ffd1dd929eae9027166ffa6bccca69253bd"},
+    {file = "zeroconf-0.132.2-cp310-cp310-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:d4bc5e43d02e0848c3174914595dfcebed9b74e65cbdfb1011c5082db7916605"},
+    {file = "zeroconf-0.132.2-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:59953e8445e69e5fee53381c437d3494f7fac8d7b51f0169d59b69eba8f95063"},
+    {file = "zeroconf-0.132.2-cp310-cp310-manylinux_2_31_x86_64.whl", hash = "sha256:ddae9592604fe04ec065cc53a321844c3592c812988346136d8ee548127f3d12"},
+    {file = "zeroconf-0.132.2-cp310-cp310-musllinux_1_1_i686.whl", hash = "sha256:b20036ab22df2fb663f797b110fa82d4798084fcc56c8a264af50989581062be"},
+    {file = "zeroconf-0.132.2-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:82678a77e471dd3b0ad5ed47a4a42474af3150819718eff7e36dca32ae591949"},
+    {file = "zeroconf-0.132.2-cp310-cp310-win32.whl", hash = "sha256:390feb3e7fccdffbf66c9bcd895b1db92e501aa2789d6a8b44e6e027ab80ec14"},
+    {file = "zeroconf-0.132.2-cp310-cp310-win_amd64.whl", hash = "sha256:779d81aac693e57090343ce5b18f477fec993f969aa87660a33e7ce81880ccdf"},
+    {file = "zeroconf-0.132.2-cp311-cp311-macosx_11_0_x86_64.whl", hash = "sha256:76d12185c335c14b04b8706b4dd0badc16f4185caeb635419c84e575cef7c980"},
+    {file = "zeroconf-0.132.2-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:700bae69eb7c45037deef4a729586f32205d391de38802e2ab89151a7a87d1fc"},
+    {file = "zeroconf-0.132.2-cp311-cp311-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:9d364a929121df5b96af53ac62abdd61fa3a931e74c7a4c80204c961c01a8667"},
+    {file = "zeroconf-0.132.2-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:e7e2c398679c863e810a9af2c5d14542a32d438e3bf5ba0b9d8e119326c33303"},
+    {file = "zeroconf-0.132.2-cp311-cp311-musllinux_1_1_i686.whl", hash = "sha256:28b1721617ddc9bf3d2ba3e2b96234f7539e1dbdcacaf6e94ec31ff7b5ebe620"},
+    {file = "zeroconf-0.132.2-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:f2b26c23efeded0e7fcfd0fb4d638ec4a83d120e1d455267d353090e36479528"},
+    {file = "zeroconf-0.132.2-cp311-cp311-win32.whl", hash = "sha256:4754dfba1af63545dfd0ab26c834c907e1dd3f94c8ee190c3041a6444313aaed"},
+    {file = "zeroconf-0.132.2-cp311-cp311-win_amd64.whl", hash = "sha256:db8607a32347da1fd4519cfea441d8b36b44df0c53198ae0471c76fc932a86e0"},
+    {file = "zeroconf-0.132.2-cp312-cp312-macosx_11_0_x86_64.whl", hash = "sha256:5354c1cf83d36b2d03ee5774923d30fe838f9371963b42ca46ecba45d3507ff4"},
+    {file = "zeroconf-0.132.2-cp312-cp312-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:48275e3db89a8d90ff983c3f7b0c6eee2ede3c4e5e75eaf2aa571ea8cb956d95"},
+    {file = "zeroconf-0.132.2-cp312-cp312-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:3eb0e57654e139c3ef5b6421053236be4a0add9f0301b01545b11a0552c7c123"},
+    {file = "zeroconf-0.132.2-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b3dd7143dfc37a20f7d1ccf32f916ac78c11d3c8bae61438ee06376b1bc535fc"},
+    {file = "zeroconf-0.132.2-cp312-cp312-musllinux_1_1_i686.whl", hash = "sha256:f9a28b0416a36ec32273ee1ac80cc72ff9b06d1cb15a9481dcd5c92bd2bc8f03"},
+    {file = "zeroconf-0.132.2-cp312-cp312-musllinux_1_1_x86_64.whl", hash = "sha256:06203c23a82b69aca9e961da675600dff19026bb22b5d042f18f9e0ff1139ed3"},
+    {file = "zeroconf-0.132.2-cp312-cp312-win32.whl", hash = "sha256:5c8c2eeb838538fffaa421f9b3f9c671778886595b5aa0d4ef4d000531e721d2"},
+    {file = "zeroconf-0.132.2-cp312-cp312-win_amd64.whl", hash = "sha256:a37fe4f302edb8d931a4c386d0944f996e3f54717495636113880c4492ab479f"},
+    {file = "zeroconf-0.132.2-pp310-pypy310_pp73-macosx_11_0_x86_64.whl", hash = "sha256:1a95025f0949ed0e873e141d482fbbefa223ef90646443e4a1d6d47f50eb89d7"},
+    {file = "zeroconf-0.132.2-pp310-pypy310_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:1c932b15848ae6b8e4b2b50c65368e396d000fea95acd473611693dbe5a00096"},
+    {file = "zeroconf-0.132.2-pp310-pypy310_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:9c295b424a271ce5022da83a1274b4cd0f696c5b8e0c190e6a28efde8b36e82d"},
+    {file = "zeroconf-0.132.2-pp310-pypy310_pp73-win_amd64.whl", hash = "sha256:c50ee0df6b0b06f1dad6261670b5be53c909b9a2b1985bcf65ea5b0d766fd10e"},
+    {file = "zeroconf-0.132.2-pp38-pypy38_pp73-macosx_11_0_x86_64.whl", hash = "sha256:5b6cfc2b62e6282eabbcb6c7223b0a8c05ed3a326e7b467d06b85a3eeda1bfc8"},
+    {file = "zeroconf-0.132.2-pp38-pypy38_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:d6c05af8b49c442422ce49565ab41a094b23e0f5692abe1533428cbe35a78f8e"},
+    {file = "zeroconf-0.132.2-pp38-pypy38_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:0b0d2ffc4bafbcc4152067bfbc1a67074d23e6100e356424bd985ca8067a2bfd"},
+    {file = "zeroconf-0.132.2-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:b60b260c70bb77d7f3b666bdd2a2a74cead5e36814f8b4295778bcdd08f65c7e"},
+    {file = "zeroconf-0.132.2-pp39-pypy39_pp73-macosx_11_0_x86_64.whl", hash = "sha256:9228c512334905338f65825102e47778e5ce034bb4249c3deb22991826ed061f"},
+    {file = "zeroconf-0.132.2-pp39-pypy39_pp73-manylinux_2_17_i686.manylinux_2_5_i686.manylinux1_i686.manylinux2014_i686.whl", hash = "sha256:e36f50a963d149bb7152543db9bdbd73f7997e66b57b7956fc17751f55e59625"},
+    {file = "zeroconf-0.132.2-pp39-pypy39_pp73-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:3bd0cd9435dced8c31491b3ed7c15707acedd11f00451f7fbb57ba3868dd5724"},
+    {file = "zeroconf-0.132.2-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:d80bde641349198c8c17684692a8cc40a36a93c0cebd8f1d7c42db7ceeaa17be"},
+    {file = "zeroconf-0.132.2.tar.gz", hash = "sha256:9ad8bc6e3f168fe8c164634c762d3265c775643defff10e26273623a12d73ae1"},
 ]
 
 [[package]]
 name = "zstandard"
 version = "0.22.0"
 requires_python = ">=3.8"
 summary = "Zstandard bindings for Python"
```

### Comparing `xklb-2.6.3/.github/LICENSE` & `xklb-2.6.5/.github/LICENSE`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/.github/Windows.md` & `xklb-2.6.5/.github/Windows.md`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 ```
 
 Then install xklb and enjoy!
 
 ```fish
 pip install xklb
 lb
+```
+
+Then you will see:
+
+```
 xk media library
 
 local media subcommands:
   fsadd [extract, xr]                Create a local media database; Add folders
   listen [lt]                        Listen to local media
   watch [wt]                         Watch local media
 ```
```

### Comparing `xklb-2.6.3/.github/examples/extract.svg` & `xklb-2.6.5/.github/examples/extract.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/.github/examples/tubeadd.svg` & `xklb-2.6.5/.github/examples/tubeadd.svg`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/.github/workflows/push.yaml` & `xklb-2.6.5/.github/workflows/push.yaml`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/db_media.py` & `xklb-2.6.5/xklb/db_media.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/db_playlists.py` & `xklb-2.6.5/xklb/db_playlists.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/dl_extract.py` & `xklb-2.6.5/xklb/dl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/fs_extract.py` & `xklb-2.6.5/xklb/fs_extract.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from xklb.utils.consts import SC, DBType
 from xklb.utils.log_utils import log
 
 
 def parse_args(action, usage):
     parser = argparse.ArgumentParser(prog="library " + action, usage=usage)
     arggroups.db_profiles(parser)
+    arggroups.capability_simulate(parser)
 
     parser.add_argument(
         "--io-multiplier",
         type=float,
         default=1.0,
         help="Especially useful for text, image, filesystem db types",
     )
@@ -142,37 +143,34 @@
 
     if getattr(mp_args, "hash", False) and media["type"] != "directory" and media["size"] > 0:
         media["hash"] = sample_hash.sample_hash_file(path)
 
     if getattr(mp_args, "move", False) and not file_utils.is_file_open(path):
         dest_path = bytes(Path(mp_args.move) / Path(path).relative_to(mp_args.playlist_path))
         dest_path = path_utils.clean_path(dest_path)
-        file_utils.rename_move_file(path, dest_path)
+        file_utils.rename_move_file(path, dest_path, simulate=mp_args.simulate)
         path = media["path"] = dest_path
 
     if getattr(mp_args, "process", False):
         if objects.is_profile(mp_args, DBType.audio) and Path(path).suffix not in [".opus", ".mka"]:
             result = process_ffmpeg.process_path(
                 mp_args,
                 path,
-                split_longer_than=2160 if "audiobook" in path.lower() else None,
+                split_longer_than=2160 if mp_args.split_longer_than is None and "audiobook" in path.lower() else None,
             )
             if result is None:
                 return None
             path = media["path"] = str(result)
         elif objects.is_profile(mp_args, DBType.video) and Path(path).suffix not in [".av1.mkv"]:
             result = process_ffmpeg.process_path(mp_args, path)
             if result is None:
                 return None
             path = media["path"] = str(result)
         elif objects.is_profile(mp_args, DBType.image) and Path(path).suffix not in [".avif", ".avifs"]:
-            result = process_image.process_path(
-                path,
-                delete_unplayable=getattr(mp_args, "delete_unplayable", False),
-            )
+            result = process_image.process_path(mp_args, path)
             if result is None:
                 return None
             path = media["path"] = str(result)
 
     return media
 
 
@@ -402,15 +400,14 @@
 
 
 def fs_add(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
     args, _parser = parse_args(SC.fsadd, usage.fsadd)
-
     extractor(args, args.paths)
 
 
 def fs_update(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
```

### Comparing `xklb-2.6.3/xklb/gdl_backend.py` & `xklb-2.6.5/xklb/gdl_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/gdl_extract.py` & `xklb-2.6.5/xklb/gdl_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/history.py` & `xklb-2.6.5/xklb/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/hn_extract.py` & `xklb-2.6.5/xklb/hn_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/lb.py` & `xklb-2.6.5/xklb/lb.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/play_actions.py` & `xklb-2.6.5/xklb/play_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,16 @@
     parser.add_argument("--transcode", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--transcode-audio", action="store_true", help=argparse.SUPPRESS)
 
     for i in range(0, 255):
         parser.add_argument(f"--cmd{i}", help=argparse.SUPPRESS)
     parser.add_argument("--shallow-organize", default="/mnt/d/", help=argparse.SUPPRESS)
 
-    parser.add_argument("--safe", "-safe", action="store_true", help="Skip generic URLs")
+    parser.add_argument("--safe", action="store_true", help="Skip generic URLs")
+    parser.add_argument("--refresh", "--rescan", action="store_true")
 
     parser.add_argument("--fetch-siblings")
     parser.add_argument("--sibling", "--episode", "--episodes", "--episodic", action="store_true")
     parser.add_argument("--solo", action="store_true")
 
     parser.add_argument("--prefetch", type=int, default=3)
     parser.add_argument("--prefix", default="", help=argparse.SUPPRESS)
@@ -480,20 +481,34 @@
 
     if args.cluster_sort:
         from xklb.scripts.cluster_sort import cluster_dicts
 
         media = cluster_dicts(args, media)
         log.debug("cluster-sort: %s", t.elapsed())
 
+    if getattr(args, "refresh", False):
+        marked = db_media.mark_media_deleted(args, [d["path"] for d in media if not Path(d["path"]).exists()])
+        log.warning(f"Marked {marked} metadata records as deleted")
+        args.refresh = False
+        return process_playqueue(args)
+
     if args.folder:
         media = ({**m, "path": str(Path(m["path"]).parent)} for m in media)
     elif args.folder_glob:
         media = ({"path": s} for m in media for s in file_utils.fast_glob(Path(m["path"]).parent, args.folder_glob))
 
-    if args.print:
+    if any(
+        [
+            args.print,
+            args.delete_files,
+            args.delete_rows,
+            args.mark_deleted,
+            args.mark_watched,
+        ]
+    ):
         media_printer.media_printer(args, media)
     else:
         media_player.play_list(args, media)
 
 
 def watch() -> None:
     args = parse_args(SC.watch, default_chromecast="Living Room TV")
```

### Comparing `xklb-2.6.3/xklb/post_actions.py` & `xklb-2.6.5/xklb/post_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     for p in paths:
         if p.startswith("http"):
             continue
 
         if getattr(args, "prefix", False):
             Path(p).unlink(missing_ok=True)
         else:
-            file_utils.trash(p, detach=len(paths) < 30)
+            file_utils.trash(args, p, detach=len(paths) < 30)
 
     if hasattr(args, "db"):
         return db_media.mark_media_deleted(args, paths)
     else:
         return len(paths)
 
 
@@ -141,15 +141,15 @@
     cmd = getattr(args, player_exit_code_cmd, None)
     if cmd:
         log_action(player_exit_code_cmd.upper())
         if cmd in ["pass", "mark-watched"]:
             pass
         elif cmd in ["soft-delete", "mark-deleted"]:
             db_media.mark_media_deleted(args, media_file)
-        elif cmd in ["delete"]:
+        elif cmd in ["delete", "delete-files", "delete-file"]:
             if media_file.startswith("http"):
                 db_media.mark_media_deleted(args, media_file)
             else:
                 delete_media(args, media_file)
         elif "{}" in cmd:
             processes.cmd_detach(media_file if s == "{}" else s for s in shlex.split(cmd))
         else:
```

### Comparing `xklb-2.6.3/xklb/readme.py` & `xklb-2.6.5/xklb/readme.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/reddit_extract.py` & `xklb-2.6.5/xklb/reddit_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/rss_extract.py` & `xklb-2.6.5/xklb/rss_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/search.py` & `xklb-2.6.5/xklb/search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/site_extract.py` & `xklb-2.6.5/xklb/site_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/tabs_actions.py` & `xklb-2.6.5/xklb/tabs_actions.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     parser = argparse.ArgumentParser(
         prog="library tabs",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         usage=usage.tabs,
     )
 
     arggroups.sql_fs(parser)
-    arggroups.capability_delete(parser)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("search", nargs="*")
     args = parser.parse_intermixed_args()
     args.action = action
 
@@ -31,17 +30,14 @@
     if args.sort:
         args.sort = [arg_utils.override_sort(s) for s in args.sort]
         args.sort = " ".join(args.sort)
 
     if args.cols:
         args.cols = list(iterables.flatten([s.split(",") for s in args.cols]))
 
-    if args.delete:
-        args.print += "d"
-
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
 
     return args
 
 
 def tabs_include_sql(x) -> str:
```

### Comparing `xklb-2.6.3/xklb/tabs_extract.py` & `xklb-2.6.5/xklb/tabs_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/tube_backend.py` & `xklb-2.6.5/xklb/tube_backend.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/tube_extract.py` & `xklb-2.6.5/xklb/tube_extract.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/usage.py` & `xklb-2.6.5/xklb/usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -738,15 +738,15 @@
         ├────────────────────────────────────────────────────────────────────────────────────────────────────────────┼───────────────┼──────────────────┼────────────────┤
         │ Commodore 64 Longplay [062] The Transformers (EU) /mnt/d/71_Mealtime_Videos/Youtube/World_of_Longplays/Com │ 24.77 minutes │                2 │ yesterday      │
         │ modore_64_Longplay_062_The_Transformers_EU_[1RRX7Kykb38].webm                                              │               │                  │                │
         ...
 
 """
 
-playlists = """library playlists DATABASE [--delete ...]
+playlists = """library playlists DATABASE
 
     List of Playlists
 
         library playlists
         ╒══════════╤════════════════════╤══════════════════════════════════════════════════════════════════════════╕
         │ extractor_key   │ title              │ path                                                                     │
         ╞══════════╪════════════════════╪══════════════════════════════════════════════════════════════════════════╡
@@ -773,15 +773,15 @@
 
     Print only playlist urls:
         Useful for piping to other utilities like xargs or GNU Parallel.
         library playlists -p f
         https://www.youtube.com/playlist?list=PL7gXS9DcOm5-O0Fc1z79M72BsrHByda3n
 
     Remove a playlist/channel and all linked videos:
-        library playlists --remove https://vimeo.com/canal180
+        library playlists --delete-rows https://vimeo.com/canal180
 
 """
 
 download_status = """library download-status DATABASE
 
     Print download queue groups
 
@@ -855,29 +855,29 @@
         │ path      │   count │
         ╞═══════════╪═════════╡
         │ Aggregate │     134 │
         ╘═══════════╧═════════╛
 
     Delete URLs
 
-        library tb -p -s cyber
+        library tabs -p -s cyber
         ╒═══════════════════════════════════════╤═════════════╤══════════════╕
         │ path                                  │ frequency   │ time_valid   │
         ╞═══════════════════════════════════════╪═════════════╪══════════════╡
         │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
         │ p/?sort=top&t=year                    │             │              │
         ├───────────────────────────────────────┼─────────────┼──────────────┤
         │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
         │ p/?sort=top&t=year                    │             │              │
         ├───────────────────────────────────────┼─────────────┼──────────────┤
         │ https://www.reddit.com/r/cyberDeck/   │ yearly      │ Sep 05 2023  │
         ╘═══════════════════════════════════════╧═════════════╧══════════════╛
-        library tb -p -w "path='https://www.reddit.com/r/cyberDeck/'" --delete
+        library tabs -p -w "path='https://www.reddit.com/r/cyberDeck/'" --delete-rows
         Removed 1 metadata records
-        library tb -p -s cyber
+        library tabs -p -s cyber
         ╒═══════════════════════════════════════╤═════════════╤══════════════╕
         │ path                                  │ frequency   │ time_valid   │
         ╞═══════════════════════════════════════╪═════════════╪══════════════╡
         │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
         │ p/?sort=top&t=year                    │             │              │
         ├───────────────────────────────────────┼─────────────┼──────────────┤
         │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
@@ -1117,15 +1117,15 @@
         library dedupe-db ./video.db media --bk path
 
     By default all non-primary and non-business key columns will be upserted unless --only-columns is provided
     If --primary-keys is not provided table metadata primary keys will be used
     If your duplicate rows contain exactly the same data in all the columns you can run with --skip-upsert to save a lot of time
 """
 
-search_db = """library search-db DATABASE TABLE SEARCH ... [--delete]
+search_db = """library search-db DATABASE TABLE SEARCH ... [--delete-rows]
 
     Search all columns in a SQLITE table. If the table does not exist, uses the table which startswith (if only one match)
 """
 
 merge_dbs = """library merge-dbs DEST_DB SOURCE_DB ... [--only-target-columns] [--only-new-rows] [--upsert] [--pk PK ...] [--table TABLE ...]
 
     Merge-DBs will insert new rows from source dbs to target db, table by table. If primary key(s) are provided,
@@ -1500,14 +1500,42 @@
         - price
 
         |    |   price |   size |   warranty |   TOPSIS |      MABAC |   SPOTIS |   BORDA |
         |----|---------|--------|------------|----------|------------|----------|---------|
         |  0 |     359 |     36 |          5 | 0.769153 |  0.348907  | 0.230847 | 7.65109 |
         |  1 |     453 |     40 |          2 | 0.419921 |  0.0124531 | 0.567301 | 8.00032 |
         |  2 |     519 |     44 |          2 | 0.230847 | -0.189399  | 0.769153 | 8.1894  |
+
+    It also works with HTTP/GCS/S3 URLs:
+
+    $ library mcda https://en.wikipedia.org/wiki/List_of_Academy_Award-winning_films --clean --minimize Year
+
+        ### Goals
+
+        #### Maximize
+
+        - Nominations
+        - Awards
+
+        #### Minimize
+
+        - Year
+
+        |      | Film                                                                    |   Year |   Awards |   Nominations |      TOPSIS |    MABAC |      SPOTIS |   BORDA |
+        |------|-------------------------------------------------------------------------|--------|----------|---------------|-------------|----------|-------------|---------|
+        |  378 | Titanic                                                                 |   1997 |       11 |            14 | 0.999993    | 1.38014  | 4.85378e-06 | 4116.62 |
+        |  868 | Ben-Hur                                                                 |   1959 |       11 |            12 | 0.902148    | 1.30871  | 0.0714303   | 4116.72 |
+        |  296 | The Lord of the Rings: The Return of the King                           |   2003 |       11 |            11 | 0.8558      | 1.27299  | 0.107147    | 4116.76 |
+        | 1341 | West Side Story                                                         |   1961 |       10 |            11 | 0.837716    | 1.22754  | 0.152599    | 4116.78 |
+        |  389 | The English Patient                                                     |   1996 |        9 |            12 | 0.836725    | 1.2178   | 0.162341    | 4116.78 |
+        | 1007 | Gone with the Wind                                                      |   1939 |        8 |            13 | 0.807086    | 1.20806  | 0.172078    | 4116.81 |
+        |  990 | From Here to Eternity                                                   |   1953 |        8 |            13 | 0.807086    | 1.20806  | 0.172079    | 4116.81 |
+        | 1167 | On the Waterfront                                                       |   1954 |        8 |            12 | 0.785       | 1.17235  | 0.207793    | 4116.83 |
+        | 1145 | My Fair Lady                                                            |   1964 |        8 |            12 | 0.785       | 1.17235  | 0.207793    | 4116.83 |
+        |  591 | Gandhi                                                                  |   1982 |        8 |            11 | 0.755312    | 1.13663  | 0.243509    | 4116.86 |
 """
 
 incremental_diff = """library incremental-diff PATH1 PATH2 [--join-keys JOIN_KEYS] [--table1 TABLE1] [--table2 TABLE2] [--table1-index TABLE1_INDEX] [--table2-index TABLE2_INDEX] [--start-row START_ROW] [--batch-size BATCH_SIZE]
 
     See data differences in an incremental way to quickly see how two different files differ.
 
     Data (PATH1, PATH2) can be two different files of different file formats (CSV, Excel) or it could even be the same file with different tables.
```

### Comparing `xklb-2.6.3/xklb/data/imagemagick_errors.py` & `xklb-2.6.5/xklb/data/imagemagick_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/data/wordbank.py` & `xklb-2.6.5/xklb/data/wordbank.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/data/yt_dlp_errors.py` & `xklb-2.6.5/xklb/data/yt_dlp_errors.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/media/av.py` & `xklb-2.6.5/xklb/media/av.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         if e.errno == 23:  # Too many open files
             raise e
         raise e
     except processes.UnplayableFile as e:
         log.error(f"Failed reading header. {path}")
         log.debug(e)
         if getattr(args, "delete_unplayable", False) and not file_utils.is_file_open(path):
-            file_utils.trash(path, detach=False)
+            file_utils.trash(args, path, detach=False)
             media["time_deleted"] = consts.APPLICATION_START
         media["error"] = "Metadata check failed"
         return media
 
     if not probe.format:
         log.error(f"Failed reading format. {path}")
         log.warning(probe)
@@ -161,15 +161,15 @@
         ) and not file_utils.is_file_open(path):
             threshold_str = (
                 strings.safe_percent(args.delete_corrupt)
                 if 0 < args.delete_corrupt < 1
                 else (args.delete_corrupt + "s")
             )
             log.warning("Deleting %s corruption %.1f%% exceeded threshold %s", path, corruption * 100, threshold_str)
-            file_utils.trash(path, detach=False)
+            file_utils.trash(args, path, detach=False)
             media["time_deleted"] = consts.APPLICATION_START
             media["error"] = "Media check failed"
 
     tags = format_.pop("tags", None)
     if tags:
         upload_date = tags.get("DATE")
         if upload_date:
```

### Comparing `xklb-2.6.3/xklb/media/books.py` & `xklb-2.6.5/xklb/media/books.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/media/dedupe.py` & `xklb-2.6.5/xklb/media/dedupe.py`

 * *Files 0% similar despite different names*

```diff
@@ -593,13 +593,13 @@
             path = d["duplicate_path"]
             if not path.startswith("http") and not args.no_delete:
                 if args.dedupe_cmd:
                     processes.cmd(
                         *shlex.split(args.dedupe_cmd), d["duplicate_path"], d["keep_path"]
                     )  # follows rmlint interface
                 else:
-                    file_utils.trash(path, detach=False)
+                    file_utils.trash(args, path, detach=False)
             db_media.mark_media_deleted(args, path)
 
 
 if __name__ == "__main__":
     dedupe_media()
```

### Comparing `xklb-2.6.3/xklb/media/media_check.py` & `xklb-2.6.5/xklb/media/media_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from xklb import usage
 from xklb.utils import arggroups, consts, file_utils, nums, objects, printing, processes, strings
 from xklb.utils.log_utils import log
 
 
 def parse_args():
     parser = argparse.ArgumentParser(prog="library media-check", usage=usage.media_check)
+    arggroups.capability_delete(parser)
     arggroups.media_check(parser)
     arggroups.debug(parser)
     parser.add_argument("paths", nargs="+")
     args = parser.parse_args()
 
     args.gap = nums.float_from_percent(args.gap)
     if args.delete_corrupt:
@@ -187,8 +188,8 @@
                         strings.safe_percent(args.delete_corrupt)
                         if 0 < args.delete_corrupt < 1
                         else (args.delete_corrupt + "s")
                     )
                     log.warning(
                         "Deleting %s corruption %.1f%% exceeded threshold %s", path, corruption * 100, threshold_str
                     )
-                    file_utils.trash(path)
+                    file_utils.trash(args, path)
```

### Comparing `xklb-2.6.3/xklb/media/media_player.py` & `xklb-2.6.5/xklb/media/media_player.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/media/media_printer.py` & `xklb-2.6.5/xklb/media/media_printer.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from copy import deepcopy
 from io import StringIO
 from numbers import Number
 from pathlib import Path
 
 from tabulate import tabulate
 
-from xklb import db_media, history
+from xklb import db_media, history, post_actions
 from xklb.utils import consts, db_utils, iterables, printing, processes, sql_utils, strings
 from xklb.utils.consts import SC
 from xklb.utils.log_utils import log
 
 
 def filter_deleted(media):
     http_list = []
@@ -139,22 +139,31 @@
             for c in cols:
                 if isinstance(media[0][c], Number):
                     D[f"sum_{c}"] = sum((d[c] or 0) for d in media)
                     D[f"avg_{c}"] = sum((d[c] or 0) for d in media) / len(media)
         media = [D]
 
     else:
+        # NOTE: when changing/moving this code be sure to preserve the behavior that -pa does not run the code
+        if getattr(args, "delete_files", False):
+            marked = post_actions.delete_media(args, [d["path"] for d in media])
+            log.warning(f"Deleted {marked} files")
+
+        if getattr(args, "delete_rows", False) or "d" in print_args:
+            args.db["media"].delete_where("path = ?", [d["path"] for d in media])
+            log.warning(f"Deleted {len(media)} rows")
+
         if "r" in print_args:
             marked = db_media.mark_media_deleted(args, [d["path"] for d in media if not Path(d["path"]).exists()])
             log.warning(f"Marked {marked} metadata records as deleted")
-        elif "d" in print_args:
+        elif getattr(args, "mark_deleted", False) or "d" in print_args:
             marked = db_media.mark_media_deleted(args, [d["path"] for d in media])
             log.warning(f"Marked {marked} metadata records as deleted")
 
-        if "w" in print_args:
+        if getattr(args, "mark_watched", False) or "w" in print_args:
             marked = history.add(args, [d["path"] for d in media])
             log.warning(f"Marked {marked} metadata records as watched")
 
     if (
         "a" not in print_args
         and "history" in tables
         and action == SC.download_status
@@ -217,14 +226,16 @@
             for line in virtual_csv.readlines():
                 printing.pipe_print(line.strip())
 
     elif "j" in print_args or consts.MOBILE_TERMINAL:
         print(json.dumps(media, indent=3))
     elif "c" in print_args:
         printing.write_csv_to_stdout(media)
+    elif "n" in print_args:
+        pass
     else:
         tbl = deepcopy(media)
         tbl = [{k: f"{v:.4f}" if isinstance(v, float) else v for k, v in d.items()} for d in tbl]
         max_col_widths = printing.calculate_max_col_widths(tbl)
         adjusted_widths = printing.distribute_excess_width(max_col_widths)
         for k, v in adjusted_widths.items():
             printing.col_resize(tbl, k, v)
```

### Comparing `xklb-2.6.3/xklb/media/subtitle.py` & `xklb-2.6.5/xklb/media/subtitle.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scratch/javguru.py` & `xklb-2.6.5/xklb/scratch/javguru.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scratch/javtiful.py` & `xklb-2.6.5/xklb/scratch/javtiful.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scratch/mam_search.py` & `xklb-2.6.5/xklb/scratch/mam_search.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scratch/mam_slots.py` & `xklb-2.6.5/xklb/scratch/mam_slots.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/add_row.py` & `xklb-2.6.5/xklb/scripts/add_row.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/big_dirs.py` & `xklb-2.6.5/xklb/scripts/big_dirs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/block.py` & `xklb-2.6.5/xklb/scripts/block.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
     parser.add_argument("--match-column", "-c", default="path", help="Column to block media if text matches")
 
     parser.add_argument("--cluster", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--min-tried", default=0, type=int, help=argparse.SUPPRESS)
     parser.add_argument("--no-confirm", "--yes", "-y", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--force", "-f", action="store_true", help=argparse.SUPPRESS)
-    arggroups.capability_delete(parser)
     parser.add_argument("--offline", "--no-tube", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--ignore-errors", "--ignoreerrors", "-i", action="store_true", help=argparse.SUPPRESS)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("playlists", nargs="*")
     args = parser.parse_intermixed_args()
@@ -191,15 +190,15 @@
                 post_actions.delete_media(args, paths_to_delete)
         return
 
     unmatched_playlists = []
     for p in args.playlists:
         p = [p]
         if consts.PYTEST_RUNNING or args.force:
-            if args.delete:
+            if args.delete_rows:
                 remove_from_blocklist(args, p)
             else:
                 add_to_blocklist(args, p)
             continue
 
         matching_media = list(
             args.db.query(
```

### Comparing `xklb-2.6.3/xklb/scripts/christen.py` & `xklb-2.6.5/xklb/scripts/christen.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/cluster_sort.py` & `xklb-2.6.5/xklb/scripts/cluster_sort.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/copy_play_counts.py` & `xklb-2.6.5/xklb/scripts/copy_play_counts.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/dedupe_czkawka.py` & `xklb-2.6.5/xklb/scripts/dedupe_czkawka.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 right_mpv_socket = str(Path(consts.TEMP_SCRIPT_DIR) / f"mpv_socket_{consts.random_string()}")
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Choose which duplicate to keep by opening both side-by-side in mpv")
     arggroups.playback(parser)
     arggroups.capability_clobber(parser)
+    arggroups.capability_delete(parser)
     arggroups.post_actions(parser)
     parser.set_defaults(start="15%", volume="70")
 
     parser.add_argument(
         "--auto-select-min-ratio",
         type=float,
         default=1.0,
@@ -240,15 +241,15 @@
         if src_size > dst_size:
             print("Source is larger than destination", diff_size)
         elif src_size < dst_size:
             print("Source is smaller than destination", diff_size)
         else:
             print("Source and destination are the same size", humanize.naturalsize(src_size, binary=True))
         if devices.confirm("Replace destination file?"):
-            file_utils.trash(new_path, detach=False)
+            file_utils.trash(args, new_path, detach=False)
             new_path = shutil.move(media_file, keep_path)
 
     log.info(f"{new_path}: new location")
 
 
 def group_and_delete(args, groups):
     is_interactive = not any([args.all_keep, args.all_left, args.all_right, args.all_delete])
@@ -258,15 +259,15 @@
             continue
 
         group = extract_group_data(group_content)
         if group is None:
             continue
 
         def delete_dupe(d, detach=is_interactive):
-            file_utils.trash(d["path"], detach=detach)
+            file_utils.trash(args, d["path"], detach=detach)
             log.info(f"{d['path']}: Deleted")
 
         group.sort(key=lambda x: x["size"], reverse=True)
         left = group[0]
 
         dups = group[1:]
         kept_dups = []
```

### Comparing `xklb-2.6.3/xklb/scripts/dedupe_db.py` & `xklb-2.6.5/xklb/scripts/dedupe_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/disk_usage.py` & `xklb-2.6.5/xklb/scripts/disk_usage.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/download_status.py` & `xklb-2.6.5/xklb/scripts/download_status.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/eda.py` & `xklb-2.6.5/xklb/scripts/eda.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 
 from xklb import usage
-from xklb.utils import arggroups, file_utils, nums
+from xklb.utils import arggroups, file_utils, nums, web
 from xklb.utils.consts import DEFAULT_FILE_ROWS_READ_LIMIT
 from xklb.utils.log_utils import log
 from xklb.utils.printing import print_df, print_series
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Perform EDA on one or more files", usage=usage.eda)
@@ -201,13 +201,14 @@
     for df in dfs:
         print(f"## {path}:{df.name}")
         print_info(args, df)
 
 
 def eda():
     args = parse_args()
+    web.requests_session(args)  # configure session
     for path in args.paths:
         file_eda(args, path)
 
 
 if __name__ == "__main__":
     eda()
```

### Comparing `xklb-2.6.3/xklb/scripts/export_text.py` & `xklb-2.6.5/xklb/scripts/export_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/history.py` & `xklb-2.6.5/xklb/scripts/history.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/incremental_diff.py` & `xklb-2.6.5/xklb/scripts/incremental_diff.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import argparse
 
 from xklb import usage
-from xklb.utils import arggroups, consts, file_utils
+from xklb.utils import arggroups, consts, file_utils, web
 from xklb.utils.argparse_utils import ArgparseList
 from xklb.utils.log_utils import log
 from xklb.utils.printing import print_df
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Diff two table-like files", usage=usage.incremental_diff)
@@ -114,12 +114,13 @@
             continue
         else:
             break
 
 
 def incremental_diff():
     args = parse_args()
+    web.requests_session(args)  # configure session
     process_chunks(args)
 
 
 if __name__ == "__main__":
     incremental_diff()
```

### Comparing `xklb-2.6.3/xklb/scripts/links_db.py` & `xklb-2.6.5/xklb/scripts/links_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/mcda.py` & `xklb-2.6.5/xklb/scripts/mcda.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import argparse
 from pathlib import Path
 
 from xklb import usage
-from xklb.utils import arggroups, argparse_utils, file_utils, iterables, objects, pd_utils, sql_utils
+from xklb.utils import arggroups, argparse_utils, file_utils, iterables, objects, pd_utils, sql_utils, web
 from xklb.utils.consts import DEFAULT_FILE_ROWS_READ_LIMIT
 from xklb.utils.log_utils import log
 from xklb.utils.printing import print_df, print_series
 
 
 def parse_args():
     parser = argparse.ArgumentParser(description="Perform MCDA on one or more files", usage=usage.mcda)
@@ -255,13 +255,14 @@
         print(f"## {path}:{df.name}")
         df = pd_utils.convert_dtypes(df, clean=args.clean)
         print_info(args, df)
 
 
 def mcda():
     args = parse_args()
+    web.requests_session(args)  # configure session
     for path in args.paths:
         file_mcda(args, path)
 
 
 if __name__ == "__main__":
     mcda()
```

### Comparing `xklb-2.6.3/xklb/scripts/merge_dbs.py` & `xklb-2.6.5/xklb/scripts/merge_dbs.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/merge_folders.py` & `xklb-2.6.5/xklb/scripts/merge_folders.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/merge_online_local.py` & `xklb-2.6.5/xklb/scripts/merge_online_local.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/move_list.py` & `xklb-2.6.5/xklb/scripts/move_list.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/open_links.py` & `xklb-2.6.5/xklb/scripts/open_links.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,22 +13,21 @@
         prog="library open-links",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         usage=usage.open_links,
     )
     arggroups.sql_fs(parser)
 
     parser.add_argument("--path", action="store_true")
-    parser.add_argument("--title", "-S", action="store_true")
+    parser.add_argument("--title", action="store_true")
     parser.add_argument("--title-prefix", "--prefix", nargs="+", action="extend")
 
     parser.add_argument("--online-media-only", "--online", action="store_true", help=argparse.SUPPRESS)
     parser.add_argument("--local-media-only", "--local", action="store_true", help=argparse.SUPPRESS)
 
     parser.add_argument("--category", "-c")
-    arggroups.capability_delete(parser)
 
     arggroups.operation_cluster(parser)
     arggroups.operation_related(parser)
 
     parser.add_argument("--browser")
     arggroups.debug(parser)
 
@@ -54,17 +53,14 @@
     if args.sort:
         args.sort = [arg_utils.override_sort(s) for s in args.sort]
         args.sort = " ".join(args.sort)
 
     if args.cols:
         args.cols = list(iterables.flatten([s.split(",") for s in args.cols]))
 
-    if args.delete:
-        args.print += "d"
-
     args.db = db_utils.connect(args)
     log.info(objects.dict_filter_bool(args.__dict__))
 
     return args
 
 
 def links_include_sql(x) -> str:
```

### Comparing `xklb-2.6.3/xklb/scripts/optimize_db.py` & `xklb-2.6.5/xklb/scripts/optimize_db.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/places_import.py` & `xklb-2.6.5/xklb/scripts/places_import.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/playback_control.py` & `xklb-2.6.5/xklb/scripts/playback_control.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,27 +7,20 @@
 
 
 def parse_args(action) -> argparse.Namespace:
     parser = argparse.ArgumentParser(
         prog=f"library {action}",
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
+    if action == "next":
+        arggroups.capability_delete(parser)
+
     parser.add_argument("--mpv-socket", default=consts.DEFAULT_MPV_LISTEN_SOCKET)
     parser.add_argument("--chromecast-device", "--cast-to", "-t")
 
-    if action == "next":
-        parser.add_argument(
-            "--delete",
-            "--remove",
-            "--erase",
-            "--rm",
-            action="store_true",
-            help="Delete currently playing media from the filesystem",
-        )
-
     arggroups.debug(parser)
     args = parser.parse_args()
 
     args.mpv = mpv_utils.connect_mpv(args.mpv_socket)
 
     log.info(objects.dict_filter_bool(args.__dict__))
 
@@ -314,15 +307,15 @@
     playing = _now_playing(args)
 
     # TODO: figure out if catt or mpv is stale
     # [kill_process(s) for s in ("python.*xklb", "bin/lb", "bin/library", "mpv")]
     if playing["catt"] or not any(playing.values()):
         Path(consts.CAST_NOW_PLAYING).unlink(missing_ok=True)
         catt_stop(args)
-        if args.delete:
-            file_utils.trash(playing["catt"])
+        if args.delete_files:
+            file_utils.trash(args, playing["catt"])
 
     if playing["mpv"]:
         args.mpv.command("playlist_next", "force")
         args.mpv.terminate()
-        if args.delete:
-            file_utils.trash(playing["mpv"])
+        if args.delete_files:
+            file_utils.trash(args, playing["mpv"])
```

### Comparing `xklb-2.6.3/xklb/scripts/playlists.py` & `xklb-2.6.5/xklb/scripts/playlists.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,23 +11,14 @@
         "library playlists",
         usage.playlists,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
     )
 
     arggroups.sql_fs(parser)
     arggroups.sql_media(parser)
-
-    parser.add_argument(
-        "--delete",
-        "--remove",
-        "--rm",
-        action="store_true",
-        help="Delete matching playlists and playlist media",
-    )
-
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("search", nargs="*")
     args = parser.parse_intermixed_args()
 
     args.include += args.search
@@ -161,9 +152,9 @@
             {', sum(count) media_count' if 'count' in query else ''}
         from ({query})
         """
 
     playlists = list(args.db.query(query, bindings))
     media_printer.media_printer(args, playlists, units="playlists")
 
-    if args.delete:
+    if args.delete_rows:
         delete_playlists(args, [d["path"] for d in playlists])
```

### Comparing `xklb-2.6.3/xklb/scripts/process_ffmpeg.py` & `xklb-2.6.5/xklb/scripts/process_ffmpeg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import argparse, json, shlex, subprocess
+import argparse, json, os, shlex, subprocess
 from pathlib import Path
 
 from xklb import usage
 from xklb.utils import arggroups, nums, objects, path_utils, processes, web
 from xklb.utils.arg_utils import kwargs_overwrite
 from xklb.utils.log_utils import log
 
@@ -27,14 +27,15 @@
 def process_path(args, path, **kwargs):
     args = kwargs_overwrite(args, kwargs)
 
     output_path = Path(web.url_to_local_path(path) if path.startswith("http") else path)
     output_path = Path(path_utils.clean_path(bytes(output_path), max_name_len=251))
 
     path = Path(path)
+    original_stats = path.stat()
 
     ffprobe_cmd = ["ffprobe", "-v", "error", "-print_format", "json", "-show_format", "-show_streams", path]
     result = subprocess.run(ffprobe_cmd, capture_output=True)
     info = json.loads(result.stdout)
 
     if "streams" not in info:
         log.error("No media streams found: %s", path)
@@ -131,15 +132,15 @@
                         "s16le",
                         "-y",
                         "/dev/null",
                     ]
                 )
             except subprocess.CalledProcessError:
                 log.exception("Splits could not be identified. Likely broken file: %s", path)
-                if args.delete_broken:
+                if args.delete_unplayable:
                     path.unlink()
                     return None
                 raise
 
             splits = result.decode().split("\n")
             splits = [line.split("=")[1] for line in splits if "lavfi.silence_start" in line]
 
@@ -158,20 +159,21 @@
                 ff_opts.extend(["-f segment", f"-segment_times {final_splits}"])
             else:
                 is_split = False
 
     cmd = f'ffmpeg -nostdin -hide_banner -loglevel warning -y -i {shlex.quote(str(path))} {" ".join(ff_opts)} {shlex.quote(str(output_path))}'
     if args.simulate:
         print(cmd)
+        return path
     else:
         try:
             processes.cmd(cmd, shell=True)
         except subprocess.CalledProcessError:
             log.exception("Could not transcode: %s", path)
-            if args.delete_broken:
+            if args.delete_unplayable:
                 path.unlink()
                 return None
             else:
                 raise
 
         if video_stream and (not args.audio_only or (args.audio_only and args.no_preserve_video)):
             path.unlink()  # Remove original
@@ -179,14 +181,16 @@
             path.unlink()  # Remove original
             return path.with_suffix(".000" + output_suffix)  # TODO: return multiple paths...
         elif output_path.stat().st_size > path.stat().st_size:
             output_path.unlink()  # Remove transcode
             return path
         else:
             path.unlink()  # Remove original
+            os.utime(output_path, (original_stats.st_atime, original_stats.st_mtime))
+
     return output_path
 
 
 def process_ffmpeg():
     args = parse_args()
 
     for path in args.paths:
```

### Comparing `xklb-2.6.3/xklb/scripts/process_image.py` & `xklb-2.6.5/xklb/scripts/process_image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,54 @@
-import argparse, subprocess
+import argparse, os, shlex, subprocess
 from pathlib import Path
 
 from xklb import usage
 from xklb.data import imagemagick_errors
 from xklb.utils import arggroups, objects, path_utils, processes, web
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library process-image", usage=usage.process_image)
+    arggroups.capability_simulate(parser)
     parser.add_argument("--delete-unplayable", action="store_true")
     arggroups.debug(parser)
 
     parser.add_argument("paths", nargs="+")
     args = parser.parse_args()
 
     log.info(objects.dict_filter_bool(args.__dict__))
     return args
 
 
-def process_path(path, delete_unplayable=False):
+def process_path(args, path):
     if path.startswith("http"):
         output_path = Path(web.url_to_local_path(path))
     else:
         output_path = Path(path)
     output_path = Path(path_utils.clean_path(bytes(output_path.with_suffix(".avif"))))
 
     path = Path(path)
     if path == output_path:
         output_path = Path(path).with_suffix(".r.avif")
         if path == output_path:
             log.error("Input and output files must have different names %s", path)
             return path
 
+    command = ["magick", "convert", "-resize", "2400>", str(path), str(output_path)]
+
+    if args.simulate:
+        print(shlex.join(command))
+        return path
+
+    original_stats = path.stat()
+
     try:
         processes.cmd(
-            "magick",
-            "mogrify",
-            "-define",
-            "preserve-timestamp=true",
-            "-resize",
-            "2400>",
-            "-format",
-            "avif",
-            str(path),
+            *command,
             ignore_regexps=[
                 imagemagick_errors.ignore_error,
                 imagemagick_errors.unsupported_error,
                 imagemagick_errors.image_error,
             ],
         )
     except subprocess.CalledProcessError as e:
@@ -55,38 +56,39 @@
         is_unsupported = any(imagemagick_errors.unsupported_error.match(l) for l in error_log)
         is_image_error = any(imagemagick_errors.image_error.match(l) for l in error_log)
         is_env_error = any(imagemagick_errors.environment_error.match(l) for l in error_log)
 
         if is_unsupported:
             output_path.unlink(missing_ok=True)  # Remove transcode attempt, if any
             return path
-        elif delete_unplayable and not is_env_error and is_image_error:
+        elif args.delete_unplayable and not is_env_error and is_image_error:
             path.unlink()
             return None
         else:
             raise
 
     if output_path.stat().st_size > path.stat().st_size:
         output_path.unlink()  # Remove transcode
         return path
     else:
         path.unlink()  # Remove original
+        os.utime(output_path, (original_stats.st_atime, original_stats.st_mtime))
 
     return output_path
 
 
 def process_image():
     args = parse_args()
 
     for path in args.paths:
         if not path.startswith("http"):
             path = str(Path(path).resolve())
 
         try:
-            process_path(path, delete_unplayable=args.delete_unplayable)
+            process_path(args, path)
         except Exception:
             print(path)
             raise
 
 
 if __name__ == "__main__":
     process_image()
```

### Comparing `xklb-2.6.3/xklb/scripts/redownload.py` & `xklb-2.6.5/xklb/scripts/redownload.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/rel_mv.py` & `xklb-2.6.5/xklb/scripts/rel_mv.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/sample_compare.py` & `xklb-2.6.5/xklb/scripts/sample_compare.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/sample_hash.py` & `xklb-2.6.5/xklb/scripts/sample_hash.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/scatter.py` & `xklb-2.6.5/xklb/scripts/scatter.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/search_db.py` & `xklb-2.6.5/xklb/scripts/search_db.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from xklb.utils import arggroups, consts, db_utils, objects
 from xklb.utils.log_utils import log
 
 
 def parse_args() -> argparse.Namespace:
     parser = argparse.ArgumentParser(prog="library search-db", usage=usage.search_db)
     arggroups.sql_fs(parser)
-    arggroups.capability_delete(parser)
     arggroups.debug(parser)
 
     arggroups.database(parser)
     parser.add_argument("table")
     parser.add_argument("search", nargs="+")
     args = parser.parse_intermixed_args()
 
@@ -55,15 +54,15 @@
 
     args.filter_sql = []
     args.filter_bindings = {}
 
     columns = args.db[args.table].columns_dict
     db_utils.construct_search_bindings(args, columns)
 
-    if args.delete:
+    if args.delete_rows:  # TODO: replace with media_printer?
         deleted_count = 0
         with args.db.conn:
             cursor = args.db.conn.execute(
                 f"DELETE FROM {args.table} WHERE 1=1 " + " ".join(args.filter_sql),
                 args.filter_bindings,
             )
             deleted_count += cursor.rowcount
```

### Comparing `xklb-2.6.3/xklb/scripts/streaming_tab_loader.py` & `xklb-2.6.5/xklb/scripts/streaming_tab_loader.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/web_add.py` & `xklb-2.6.5/xklb/scripts/web_add.py`

 * *Files 2% similar despite different names*

```diff
@@ -193,14 +193,15 @@
 
 
 def web_add(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
     args, _parser = parse_args(prog=f"library {SC.webadd}", usage=usage.webadd)
+    web.requests_session(args)  # configure session
 
     if args.no_extract:
         media_new = set()
         media_known = set()
         for p in arg_utils.gen_paths(args):
             if db_media.exists(args, p):
                 media_known.add(p)
@@ -226,14 +227,15 @@
 
 
 def web_update(args=None) -> None:
     if args:
         sys.argv = ["lb", *args]
 
     args, parser = parse_args(prog=f"library {SC.webupdate}", usage=usage.webupdate)
+    web.requests_session(args)  # configure session
 
     web_playlists = db_playlists.get_all(
         args,
         sql_filters="extractor_key = 'WebFolder'",
         order_by="""length(path)-length(REPLACE(path, '/', '')) desc
         , random()
         """,
```

### Comparing `xklb-2.6.3/xklb/scripts/mining/extract_links.py` & `xklb-2.6.5/xklb/scripts/mining/extract_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/mining/extract_text.py` & `xklb-2.6.5/xklb/scripts/mining/extract_text.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/mining/markdown_links.py` & `xklb-2.6.5/xklb/scripts/mining/markdown_links.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/mining/mpv_watchlater.py` & `xklb-2.6.5/xklb/scripts/mining/mpv_watchlater.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/mining/nouns.py` & `xklb-2.6.5/xklb/scripts/mining/nouns.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/mining/pushshift.py` & `xklb-2.6.5/xklb/scripts/mining/pushshift.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/mining/reddit_selftext.py` & `xklb-2.6.5/xklb/scripts/mining/reddit_selftext.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/mining/substack.py` & `xklb-2.6.5/xklb/scripts/mining/substack.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/scripts/mining/tildes.py` & `xklb-2.6.5/xklb/scripts/mining/tildes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/arg_utils.py` & `xklb-2.6.5/xklb/utils/arg_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/arggroups.py` & `xklb-2.6.5/xklb/utils/arggroups.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,37 @@
 from xklb.utils.consts import DEFAULT_FILE_ROWS_READ_LIMIT, DBType
 
 
 def debug(parser):
     parser.add_argument("--verbose", "-v", action="count", default=0)
 
 
+def capability_soft_delete(parser):
+    parser.add_argument("--mark-deleted", "--soft-delete", action="store_true", help="Mark matching rows as deleted")
+    parser.add_argument("--mark-watched", action="store_true", help="Mark matching rows as watched")
+    parser.add_argument("--delete-rows", action="store_true", help="Delete matching rows")
+
+
+def capability_delete(parser):
+    parser.add_argument(
+        "--override-trash", "--override-rm", "--trash-cmd", default="trash", help="Custom trash command"
+    )
+    parser.add_argument(
+        "--delete-files",
+        "--delete-file",
+        "--trash",
+        "--rm",
+        action="store_true",
+        help="Delete files from filesystem",
+    )
+
+
 def database(parser):
+    capability_soft_delete(parser)
+    capability_delete(parser)
     parser.add_argument("--db", "-db", dest="database", help="Positional argument override")
     parser.add_argument("database")
 
 
 def paths_or_stdin(parser):
     parser.add_argument("--file", "-f", help="File with one URL per line")
     parser.add_argument(
@@ -180,25 +202,14 @@
     parser.add_argument("--exclude-unique", "--no-unique", action="store_true", help="Exclude 'unique' lines")
 
 
 def operation_related(parser):
     parser.add_argument("--related", "-R", action="count", default=0, help=argparse.SUPPRESS)
 
 
-def capability_delete(parser):
-    parser.add_argument("--mark-deleted", "--soft-delete", action="store_true", help="Mark matching rows as deleted")
-    parser.add_argument(
-        "--delete",
-        "--remove",
-        "--rm",
-        action="store_true",
-        help="Delete matching rows",
-    )
-
-
 def capability_clobber(parser):
     parser.add_argument("--replace", "--clobber", action="store_true")
     parser.add_argument("--no-replace", "--no-clobber", action="store_true")
 
 
 def capability_simulate(parser):
     parser.add_argument("--simulate", "--dry-run", action="store_true")
```

### Comparing `xklb-2.6.3/xklb/utils/argparse_utils.py` & `xklb-2.6.5/xklb/utils/argparse_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/consts.py` & `xklb-2.6.5/xklb/utils/consts.py`

 * *Files 1% similar despite different names*

```diff
@@ -135,15 +135,15 @@
 OCR_EXTENSIONS = set("gif|jpg|jpeg|png|tif|tff|tiff".split("|"))
 AUDIO_ONLY_EXTENSIONS = set("mka|opus|oga|ogg|mp3|mpga|m2a|m4a|m4b|flac|wav|wma|aac|aa3|ac3|ape|mid|midi".split("|"))
 VIDEO_EXTENSIONS = set(
     (
         "str|aa|aax|acm|adf|adp|dtk|ads|ss2|adx|aea|afc|aix|al|apl|avifs|gif|gifv"
         "|mac|aptx|aptxhd|aqt|ast|obu|avi|avr|avs|avs2|avs3|bfstm|bcstm|binka"
         "|bit|bmv|brstm|cdg|cdxl|xl|c2|302|daud|str|adp|dav|dss|dts|dtshd|dv"
-        "|dif|divx|cdata|eac3|paf|fap|flm|flv|fsb|fwse|g722|722|tco|rco"
+        "|dif|divx|cdata|eac3|paf|fap|flm|flv|fsb|fwse|g722|722|tco|rco|heics"
         "|g723_1|g729|genh|gsm|h261|h26l|h264|264|avc|mts|m2ts|hca|hevc|h265|265|idf"
         "|ifv|cgi|ipu|sf|ircam|ivr|kux|669|abc|amf|ams|dbm|dmf|dsm|far|it|mdl"
         "|med|mod|mt2|mtm|okt|psm|ptm|s3m|stm|ult|umx|xm|itgz|itr|itz|iso|img"
         "|mdgz|mdr|mdz|s3gz|s3r|s3z|xmgz|xmr|xmz|669|amf|ams|dbm|digi|dmf"
         "|dsm|dtm|far|gdm|ice|imf|it|j2b|m15|mdl|med|mmcmp|mms|mo3|mod|mptm"
         "|mt2|mtm|nst|okt|ogm|ogv|plm|ppm|psm|pt36|ptm|s3m|sfx|sfx2|st26|stk|stm"
         "|stp|ult|umx|wow|xm|xpk|flv|dat|lvf|m4v|mkv|ts|tp|mk3d|webm|mca|mcc"
```

### Comparing `xklb-2.6.3/xklb/utils/db_utils.py` & `xklb-2.6.5/xklb/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/devices.py` & `xklb-2.6.5/xklb/utils/devices.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/file_utils.py` & `xklb-2.6.5/xklb/utils/file_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,17 +61,17 @@
         shutil.copyfileobj(fo_src, fo_dest)
     fo_dest.seek(0)
     fname = fo_dest.name
     fo_dest.close()
     return fname
 
 
-def trash(path: Path | str, detach=True) -> None:
+def trash(args, path: Path | str, detach=True) -> None:
     if Path(path).exists():
-        trash_put = which("trash-put") or which("trash")
+        trash_put = which(args.override_trash)
         if trash_put is not None:
             if not detach:
                 processes.cmd(trash_put, path, strict=False)
                 return
             try:
                 processes.cmd_detach(trash_put, path)
             except Exception:
@@ -145,31 +145,34 @@
             if entry.is_file():
                 files.append(entry.path)
                 if len(files) == limit:
                     break
     return sorted(files)
 
 
-def rename_move_file(source_file, destination_file):
-    try:
-        os.rename(source_file, destination_file)  # performance
-    except OSError as e:
-        if e.errno == errno.ENOENT:
-            try:
-                os.makedirs(os.path.dirname(destination_file), exist_ok=True)
-                os.rename(source_file, destination_file)  # try again
-            except OSError as e:
-                if e.errno == errno.EXDEV:  # Cross-device
-                    shutil.move(source_file, destination_file)  # Fallback to shutil.move
-                else:
-                    raise
-        elif e.errno == errno.EXDEV:  # Cross-device
-            shutil.move(source_file, destination_file)  # Fallback to shutil.move
-        else:
-            raise
+def rename_move_file(source_file, destination_file, simulate=False):
+    if simulate:
+        print("mv", source_file, destination_file)
+    else:
+        try:
+            os.rename(source_file, destination_file)  # performance
+        except OSError as e:
+            if e.errno == errno.ENOENT:
+                try:
+                    os.makedirs(os.path.dirname(destination_file), exist_ok=True)
+                    os.rename(source_file, destination_file)  # try again
+                except OSError as e:
+                    if e.errno == errno.EXDEV:  # Cross-device
+                        shutil.move(source_file, destination_file)  # Fallback to shutil.move
+                    else:
+                        raise
+            elif e.errno == errno.EXDEV:  # Cross-device
+                shutil.move(source_file, destination_file)  # Fallback to shutil.move
+            else:
+                raise
 
 
 def move_files(file_list):
     for existing_path, new_path in file_list:
         try:
             os.rename(existing_path, new_path)
         except Exception:
```

### Comparing `xklb-2.6.3/xklb/utils/gui.py` & `xklb-2.6.5/xklb/utils/gui.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/iterables.py` & `xklb-2.6.5/xklb/utils/iterables.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/log_utils.py` & `xklb-2.6.5/xklb/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/mpv_utils.py` & `xklb-2.6.5/xklb/utils/mpv_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/nums.py` & `xklb-2.6.5/xklb/utils/nums.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/objects.py` & `xklb-2.6.5/xklb/utils/objects.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/path_utils.py` & `xklb-2.6.5/xklb/utils/path_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from collections import OrderedDict
 from pathlib import Path
 
 from xklb.utils import consts, iterables, strings
-from xklb.utils.log_utils import log
 
 
 def random_filename(path) -> str:
     ext = Path(path).suffix
     path = str(Path(path).with_suffix(""))
     return f"{path}.{consts.random_string()}{ext}"
 
@@ -41,24 +40,24 @@
     pre = ""
     if path.drive and path.drive.endswith(":"):
         pre = path.drive
         path = Path(str(path)[len(path.drive) :])
 
     parent = [strings.clean_string(part) for part in path.parent.parts]
     stem = strings.clean_string(path.stem)
-    log.debug("cleaned %s %s", parent, stem)
+    # log.debug("cleaned %s %s", parent, stem)
 
     parent = [strings.remove_prefixes(part, [" ", "-"]) for part in parent]
-    log.debug("parent_prefixes %s %s", parent, stem)
+    # log.debug("parent_prefixes %s %s", parent, stem)
     parent = [strings.remove_suffixes(part, [" ", "-", "_", "."]) for part in parent]
-    log.debug("parent_suffixes %s %s", parent, stem)
+    # log.debug("parent_suffixes %s %s", parent, stem)
 
     stem = strings.remove_prefixes(stem, [" ", "-"])
     stem = strings.remove_suffixes(stem, [" ", "-", "."])
-    log.debug("stem %s %s", parent, stem)
+    # log.debug("stem %s %s", parent, stem)
 
     parent = ["_" if part == "" else part for part in parent]
     if lowercase_folders:
         parent = [p.lower() for p in parent]
     elif case_insensitive:
 
         def case_insensitive_r(p):
```

### Comparing `xklb-2.6.3/xklb/utils/pd_utils.py` & `xklb-2.6.5/xklb/utils/pd_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/printing.py` & `xklb-2.6.5/xklb/utils/printing.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/processes.py` & `xklb-2.6.5/xklb/utils/processes.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/sql_utils.py` & `xklb-2.6.5/xklb/utils/sql_utils.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/strings.py` & `xklb-2.6.5/xklb/utils/strings.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/utils/web.py` & `xklb-2.6.5/xklb/utils/web.py`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/xklb/assets/kotobago.png` & `xklb-2.6.5/xklb/assets/kotobago.png`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/.gitignore` & `xklb-2.6.5/.gitignore`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/pyproject.toml` & `xklb-2.6.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `xklb-2.6.3/.github/README.md` & `xklb-2.6.5/.github/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.6.003)
+    xk media library subcommands (v2.6.005)
 
     Create database subcommands:
     ╭───────────────┬────────────────────────────────────────────────────╮
     │ fsadd         │ Add local media                                    │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ tubeadd       │ Add online video media (yt-dlp)                    │
     ├───────────────┼────────────────────────────────────────────────────┤
@@ -1538,29 +1538,29 @@
         │ path      │   count │
         ╞═══════════╪═════════╡
         │ Aggregate │     134 │
         ╘═══════════╧═════════╛
 
     Delete URLs
 
-        library tb -p -s cyber
+        library tabs -p -s cyber
         ╒═══════════════════════════════════════╤═════════════╤══════════════╕
         │ path                                  │ frequency   │ time_valid   │
         ╞═══════════════════════════════════════╪═════════════╪══════════════╡
         │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
         │ p/?sort=top&t=year                    │             │              │
         ├───────────────────────────────────────┼─────────────┼──────────────┤
         │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
         │ p/?sort=top&t=year                    │             │              │
         ├───────────────────────────────────────┼─────────────┼──────────────┤
         │ https://www.reddit.com/r/cyberDeck/   │ yearly      │ Sep 05 2023  │
         ╘═══════════════════════════════════════╧═════════════╧══════════════╛
-        library tb -p -w "path='https://www.reddit.com/r/cyberDeck/'" --delete
+        library tabs -p -w "path='https://www.reddit.com/r/cyberDeck/'" --delete-rows
         Removed 1 metadata records
-        library tb -p -s cyber
+        library tabs -p -s cyber
         ╒═══════════════════════════════════════╤═════════════╤══════════════╕
         │ path                                  │ frequency   │ time_valid   │
         ╞═══════════════════════════════════════╪═════════════╪══════════════╡
         │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
         │ p/?sort=top&t=year                    │             │              │
         ├───────────────────────────────────────┼─────────────┼──────────────┤
         │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
@@ -1622,15 +1622,15 @@
 </details>
 
 ###### playlists
 
 <details><summary>List stored playlists</summary>
 
     $ library playlists -h
-    usage: library playlists DATABASE [--delete ...]
+    usage: library playlists DATABASE
 
     List of Playlists
 
         library playlists
         ╒══════════╤════════════════════╤══════════════════════════════════════════════════════════════════════════╕
         │ extractor_key   │ title              │ path                                                                     │
         ╞══════════╪════════════════════╪══════════════════════════════════════════════════════════════════════════╡
@@ -1657,15 +1657,15 @@
 
     Print only playlist urls:
         Useful for piping to other utilities like xargs or GNU Parallel.
         library playlists -p f
         https://www.youtube.com/playlist?list=PL7gXS9DcOm5-O0Fc1z79M72BsrHByda3n
 
     Remove a playlist/channel and all linked videos:
-        library playlists --remove https://vimeo.com/canal180
+        library playlists --delete-rows https://vimeo.com/canal180
 
 
 
 </details>
 
 ###### download
 
@@ -2124,14 +2124,42 @@
 
         |    |   price |   size |   warranty |   TOPSIS |      MABAC |   SPOTIS |   BORDA |
         |----|---------|--------|------------|----------|------------|----------|---------|
         |  0 |     359 |     36 |          5 | 0.769153 |  0.348907  | 0.230847 | 7.65109 |
         |  1 |     453 |     40 |          2 | 0.419921 |  0.0124531 | 0.567301 | 8.00032 |
         |  2 |     519 |     44 |          2 | 0.230847 | -0.189399  | 0.769153 | 8.1894  |
 
+    It also works with HTTP/GCS/S3 URLs:
+
+    $ library mcda https://en.wikipedia.org/wiki/List_of_Academy_Award-winning_films --clean --minimize Year
+
+        ### Goals
+
+        #### Maximize
+
+        - Nominations
+        - Awards
+
+        #### Minimize
+
+        - Year
+
+        |      | Film                                                                    |   Year |   Awards |   Nominations |      TOPSIS |    MABAC |      SPOTIS |   BORDA |
+        |------|-------------------------------------------------------------------------|--------|----------|---------------|-------------|----------|-------------|---------|
+        |  378 | Titanic                                                                 |   1997 |       11 |            14 | 0.999993    | 1.38014  | 4.85378e-06 | 4116.62 |
+        |  868 | Ben-Hur                                                                 |   1959 |       11 |            12 | 0.902148    | 1.30871  | 0.0714303   | 4116.72 |
+        |  296 | The Lord of the Rings: The Return of the King                           |   2003 |       11 |            11 | 0.8558      | 1.27299  | 0.107147    | 4116.76 |
+        | 1341 | West Side Story                                                         |   1961 |       10 |            11 | 0.837716    | 1.22754  | 0.152599    | 4116.78 |
+        |  389 | The English Patient                                                     |   1996 |        9 |            12 | 0.836725    | 1.2178   | 0.162341    | 4116.78 |
+        | 1007 | Gone with the Wind                                                      |   1939 |        8 |            13 | 0.807086    | 1.20806  | 0.172078    | 4116.81 |
+        |  990 | From Here to Eternity                                                   |   1953 |        8 |            13 | 0.807086    | 1.20806  | 0.172079    | 4116.81 |
+        | 1167 | On the Waterfront                                                       |   1954 |        8 |            12 | 0.785       | 1.17235  | 0.207793    | 4116.83 |
+        | 1145 | My Fair Lady                                                            |   1964 |        8 |            12 | 0.785       | 1.17235  | 0.207793    | 4116.83 |
+        |  591 | Gandhi                                                                  |   1982 |        8 |            11 | 0.755312    | 1.13663  | 0.243509    | 4116.86 |
+
 
 </details>
 
 ###### incremental-diff
 
 <details><summary>Diff large table-like files in chunks</summary>
 
@@ -2589,15 +2617,15 @@
 </details>
 
 ###### search-db
 
 <details><summary>Search a SQLITE database</summary>
 
     $ library search-db -h
-    usage: library search-db DATABASE TABLE SEARCH ... [--delete]
+    usage: library search-db DATABASE TABLE SEARCH ... [--delete-rows]
 
     Search all columns in a SQLITE table. If the table does not exist, uses the table which startswith (if only one match)
 
 
 </details>
 
 ###### optimize
```

### Comparing `xklb-2.6.3/PKG-INFO` & `xklb-2.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: xklb
-Version: 2.6.3
+Version: 2.6.5
 Summary: xk library
 Project-URL: documentation, https://github.com/chapmanjacobd/library#usage
 Project-URL: homepage, https://github.com/chapmanjacobd/library#readme
 Project-URL: repository, https://github.com/chapmanjacobd/library/
 Author-email: Jacob Chapman <7908073+chapmanjacobd@users.noreply.github.com>
 License: BSD 3-Clause No Nuclear License
         
@@ -179,15 +179,15 @@
 To stop playing press Ctrl+C in either the terminal or mpv
 
 </details>
 
 <details><summary>List all subcommands</summary>
 
     $ library
-    xk media library subcommands (v2.6.003)
+    xk media library subcommands (v2.6.005)
 
     Create database subcommands:
     ╭───────────────┬────────────────────────────────────────────────────╮
     │ fsadd         │ Add local media                                    │
     ├───────────────┼────────────────────────────────────────────────────┤
     │ tubeadd       │ Add online video media (yt-dlp)                    │
     ├───────────────┼────────────────────────────────────────────────────┤
@@ -1626,29 +1626,29 @@
         │ path      │   count │
         ╞═══════════╪═════════╡
         │ Aggregate │     134 │
         ╘═══════════╧═════════╛
 
     Delete URLs
 
-        library tb -p -s cyber
+        library tabs -p -s cyber
         ╒═══════════════════════════════════════╤═════════════╤══════════════╕
         │ path                                  │ frequency   │ time_valid   │
         ╞═══════════════════════════════════════╪═════════════╪══════════════╡
         │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
         │ p/?sort=top&t=year                    │             │              │
         ├───────────────────────────────────────┼─────────────┼──────────────┤
         │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
         │ p/?sort=top&t=year                    │             │              │
         ├───────────────────────────────────────┼─────────────┼──────────────┤
         │ https://www.reddit.com/r/cyberDeck/   │ yearly      │ Sep 05 2023  │
         ╘═══════════════════════════════════════╧═════════════╧══════════════╛
-        library tb -p -w "path='https://www.reddit.com/r/cyberDeck/'" --delete
+        library tabs -p -w "path='https://www.reddit.com/r/cyberDeck/'" --delete-rows
         Removed 1 metadata records
-        library tb -p -s cyber
+        library tabs -p -s cyber
         ╒═══════════════════════════════════════╤═════════════╤══════════════╕
         │ path                                  │ frequency   │ time_valid   │
         ╞═══════════════════════════════════════╪═════════════╪══════════════╡
         │ https://old.reddit.com/r/cyberDeck/to │ yearly      │ Dec 31 1970  │
         │ p/?sort=top&t=year                    │             │              │
         ├───────────────────────────────────────┼─────────────┼──────────────┤
         │ https://old.reddit.com/r/Cyberpunk/to │ yearly      │ Aug 29 2023  │
@@ -1710,15 +1710,15 @@
 </details>
 
 ###### playlists
 
 <details><summary>List stored playlists</summary>
 
     $ library playlists -h
-    usage: library playlists DATABASE [--delete ...]
+    usage: library playlists DATABASE
 
     List of Playlists
 
         library playlists
         ╒══════════╤════════════════════╤══════════════════════════════════════════════════════════════════════════╕
         │ extractor_key   │ title              │ path                                                                     │
         ╞══════════╪════════════════════╪══════════════════════════════════════════════════════════════════════════╡
@@ -1745,15 +1745,15 @@
 
     Print only playlist urls:
         Useful for piping to other utilities like xargs or GNU Parallel.
         library playlists -p f
         https://www.youtube.com/playlist?list=PL7gXS9DcOm5-O0Fc1z79M72BsrHByda3n
 
     Remove a playlist/channel and all linked videos:
-        library playlists --remove https://vimeo.com/canal180
+        library playlists --delete-rows https://vimeo.com/canal180
 
 
 
 </details>
 
 ###### download
 
@@ -2212,14 +2212,42 @@
 
         |    |   price |   size |   warranty |   TOPSIS |      MABAC |   SPOTIS |   BORDA |
         |----|---------|--------|------------|----------|------------|----------|---------|
         |  0 |     359 |     36 |          5 | 0.769153 |  0.348907  | 0.230847 | 7.65109 |
         |  1 |     453 |     40 |          2 | 0.419921 |  0.0124531 | 0.567301 | 8.00032 |
         |  2 |     519 |     44 |          2 | 0.230847 | -0.189399  | 0.769153 | 8.1894  |
 
+    It also works with HTTP/GCS/S3 URLs:
+
+    $ library mcda https://en.wikipedia.org/wiki/List_of_Academy_Award-winning_films --clean --minimize Year
+
+        ### Goals
+
+        #### Maximize
+
+        - Nominations
+        - Awards
+
+        #### Minimize
+
+        - Year
+
+        |      | Film                                                                    |   Year |   Awards |   Nominations |      TOPSIS |    MABAC |      SPOTIS |   BORDA |
+        |------|-------------------------------------------------------------------------|--------|----------|---------------|-------------|----------|-------------|---------|
+        |  378 | Titanic                                                                 |   1997 |       11 |            14 | 0.999993    | 1.38014  | 4.85378e-06 | 4116.62 |
+        |  868 | Ben-Hur                                                                 |   1959 |       11 |            12 | 0.902148    | 1.30871  | 0.0714303   | 4116.72 |
+        |  296 | The Lord of the Rings: The Return of the King                           |   2003 |       11 |            11 | 0.8558      | 1.27299  | 0.107147    | 4116.76 |
+        | 1341 | West Side Story                                                         |   1961 |       10 |            11 | 0.837716    | 1.22754  | 0.152599    | 4116.78 |
+        |  389 | The English Patient                                                     |   1996 |        9 |            12 | 0.836725    | 1.2178   | 0.162341    | 4116.78 |
+        | 1007 | Gone with the Wind                                                      |   1939 |        8 |            13 | 0.807086    | 1.20806  | 0.172078    | 4116.81 |
+        |  990 | From Here to Eternity                                                   |   1953 |        8 |            13 | 0.807086    | 1.20806  | 0.172079    | 4116.81 |
+        | 1167 | On the Waterfront                                                       |   1954 |        8 |            12 | 0.785       | 1.17235  | 0.207793    | 4116.83 |
+        | 1145 | My Fair Lady                                                            |   1964 |        8 |            12 | 0.785       | 1.17235  | 0.207793    | 4116.83 |
+        |  591 | Gandhi                                                                  |   1982 |        8 |            11 | 0.755312    | 1.13663  | 0.243509    | 4116.86 |
+
 
 </details>
 
 ###### incremental-diff
 
 <details><summary>Diff large table-like files in chunks</summary>
 
@@ -2677,15 +2705,15 @@
 </details>
 
 ###### search-db
 
 <details><summary>Search a SQLITE database</summary>
 
     $ library search-db -h
-    usage: library search-db DATABASE TABLE SEARCH ... [--delete]
+    usage: library search-db DATABASE TABLE SEARCH ... [--delete-rows]
 
     Search all columns in a SQLITE table. If the table does not exist, uses the table which startswith (if only one match)
 
 
 </details>
 
 ###### optimize
```

