# Comparing `tmp/mns-scheduler-1.0.2.1.tar.gz` & `tmp/mns-scheduler-1.0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mns-scheduler-1.0.2.1.tar", last modified: Fri Apr 12 05:30:36 2024, max compression
+gzip compressed data, was "mns-scheduler-1.0.2.2.tar", last modified: Sat Apr 13 06:50:59 2024, max compression
```

## Comparing `mns-scheduler-1.0.2.1.tar` & `mns-scheduler-1.0.2.2.tar`

### file list

```diff
@@ -1,98 +1,99 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.644909 mns-scheduler-1.0.2.1/
--rw-rw-rw-   0        0        0       62 2024-04-12 05:30:36.643911 mns-scheduler-1.0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.611997 mns-scheduler-1.0.2.1/mns_scheduler/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.1/mns_scheduler/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.613992 mns-scheduler-1.0.2.1/mns_scheduler/big_deal/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.1/mns_scheduler/big_deal/__init__.py
--rw-rw-rw-   0        0        0     4555 2023-12-22 04:57:03.000000 mns-scheduler-1.0.2.1/mns_scheduler/big_deal/ths_big_deal_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.615986 mns-scheduler-1.0.2.1/mns_scheduler/company_info/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/company_info/__init__.py
--rw-rw-rw-   0        0        0    15238 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.1/mns_scheduler/company_info/company_constant_data.py
--rw-rw-rw-   0        0        0    20330 2024-04-11 14:07:31.000000 mns-scheduler-1.0.2.1/mns_scheduler/company_info/company_info_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.615986 mns-scheduler-1.0.2.1/mns_scheduler/concept/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.616983 mns-scheduler-1.0.2.1/mns_scheduler/concept/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/clean/__init__.py
--rw-rw-rw-   0        0        0     2440 2024-03-22 08:13:08.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.618978 mns-scheduler-1.0.2.1/mns_scheduler/concept/em/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/em/__init__.py
--rw-rw-rw-   0        0        0     4993 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/em/em_new_concept_his_sync.py
--rw-rw-rw-   0        0        0     7083 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/em/em_new_concept_sync_common_api.py
--rw-rw-rw-   0        0        0     2335 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/em/em_new_concept_sync_web.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.619976 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.620975 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/app/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/app/__init__.py
--rw-rw-rw-   0        0        0     5148 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.621971 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/common/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/common/__init__.py
--rw-rw-rw-   0        0        0    10180 2024-04-11 14:04:04.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.623965 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/symbol/__init__.py
--rw-rw-rw-   0        0        0     1928 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
--rw-rw-rw-   0        0        0     8263 2024-03-22 07:44:40.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.624962 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/web/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/web/__init__.py
--rw-rw-rw-   0        0        0     4996 2024-03-21 16:54:33.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
--rw-rw-rw-   0        0        0     3605 2024-03-21 16:54:56.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.625960 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/wen_cai/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/wen_cai/__init__.py
--rw-rw-rw-   0        0        0     1747 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.626957 mns-scheduler-1.0.2.1/mns_scheduler/db/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/db/__init__.py
--rw-rw-rw-   0        0        0     3952 2024-02-28 08:33:00.000000 mns-scheduler-1.0.2.1/mns_scheduler/db/col_move_service.py
--rw-rw-rw-   0        0        0      747 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/db/db_status.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.627954 mns-scheduler-1.0.2.1/mns_scheduler/dt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/dt/__init__.py
--rw-rw-rw-   0        0        0     3466 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/dt/stock_dt_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.628951 mns-scheduler-1.0.2.1/mns_scheduler/ipo/
--rw-rw-rw-   0        0        0      163 2024-01-08 10:50:26.000000 mns-scheduler-1.0.2.1/mns_scheduler/ipo/__init__.py
--rw-rw-rw-   0        0        0      387 2024-01-08 10:59:33.000000 mns-scheduler-1.0.2.1/mns_scheduler/ipo/auto_ipo_buy_api.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.629949 mns-scheduler-1.0.2.1/mns_scheduler/k_line/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/k_line/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.630946 mns-scheduler-1.0.2.1/mns_scheduler/k_line/clean/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/k_line/clean/__init__.py
--rw-rw-rw-   0        0        0    21833 2024-01-09 10:50:36.000000 mns-scheduler-1.0.2.1/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
--rw-rw-rw-   0        0        0     7028 2024-01-09 10:50:05.000000 mns-scheduler-1.0.2.1/mns_scheduler/k_line/clean/k_line_info_clean_service.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.631944 mns-scheduler-1.0.2.1/mns_scheduler/k_line/sync/
--rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/k_line/sync/__init__.py
--rw-rw-rw-   0        0        0     5654 2024-03-29 10:48:40.000000 mns-scheduler-1.0.2.1/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.632941 mns-scheduler-1.0.2.1/mns_scheduler/kpl/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/kpl/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.632941 mns-scheduler-1.0.2.1/mns_scheduler/kpl/selection/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/kpl/selection/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.633938 mns-scheduler-1.0.2.1/mns_scheduler/kpl/selection/index/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.1/mns_scheduler/kpl/selection/index/__init__.py
--rw-rw-rw-   0        0        0     8016 2024-04-02 13:03:08.000000 mns-scheduler-1.0.2.1/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.634935 mns-scheduler-1.0.2.1/mns_scheduler/kpl/selection/symbol/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.1/mns_scheduler/kpl/selection/symbol/__init__.py
--rw-rw-rw-   0        0        0     4679 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.1/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.635934 mns-scheduler-1.0.2.1/mns_scheduler/kpl/selection/total/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.1/mns_scheduler/kpl/selection/total/__init__.py
--rw-rw-rw-   0        0        0     7527 2024-04-02 14:49:34.000000 mns-scheduler-1.0.2.1/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.637928 mns-scheduler-1.0.2.1/mns_scheduler/real_time/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/real_time/__init__.py
--rw-rw-rw-   0        0        0     1066 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.1/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
--rw-rw-rw-   0        0        0     8850 2024-04-01 01:27:55.000000 mns-scheduler-1.0.2.1/mns_scheduler/real_time/realtime_quotes_now_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.638924 mns-scheduler-1.0.2.1/mns_scheduler/zb/
--rw-rw-rw-   0        0        0      165 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/zb/__init__.py
--rw-rw-rw-   0        0        0     1936 2023-12-17 03:50:52.000000 mns-scheduler-1.0.2.1/mns_scheduler/zb/stock_zb_pool_sync.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.641917 mns-scheduler-1.0.2.1/mns_scheduler/zt/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/zt/__init__.py
--rw-rw-rw-   0        0        0     4015 2023-12-17 13:29:39.000000 mns-scheduler-1.0.2.1/mns_scheduler/zt/export_open_data_to_excel.py
--rw-rw-rw-   0        0        0    17269 2024-03-09 09:58:27.000000 mns-scheduler-1.0.2.1/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
--rw-rw-rw-   0        0        0    21283 2024-01-04 12:05:04.000000 mns-scheduler-1.0.2.1/mns_scheduler/zt/today_high_chg_pool_sync_api.py
--rw-rw-rw-   0        0        0    10916 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.1/mns_scheduler/zt/zt_five_boards_sync_api.py
--rw-rw-rw-   0        0        0     7534 2024-04-12 05:21:45.000000 mns-scheduler-1.0.2.1/mns_scheduler/zt/zt_pool_sync_api.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.642914 mns-scheduler-1.0.2.1/mns_scheduler/zz_task/
--rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.1/mns_scheduler/zz_task/__init__.py
--rw-rw-rw-   0        0        0    13768 2024-04-02 14:52:18.000000 mns-scheduler-1.0.2.1/mns_scheduler/zz_task/data_sync_task.py
--rw-rw-rw-   0        0        0      932 2024-03-23 03:12:05.000000 mns-scheduler-1.0.2.1/mns_scheduler/zz_task/sync_realtime_quotes_task.py
-drwxrwxrwx   0        0        0        0 2024-04-12 05:30:36.643911 mns-scheduler-1.0.2.1/mns_scheduler.egg-info/
--rw-rw-rw-   0        0        0       62 2024-04-12 05:30:36.000000 mns-scheduler-1.0.2.1/mns_scheduler.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2948 2024-04-12 05:30:36.000000 mns-scheduler-1.0.2.1/mns_scheduler.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 05:30:36.000000 mns-scheduler-1.0.2.1/mns_scheduler.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2024-04-12 05:30:36.000000 mns-scheduler-1.0.2.1/mns_scheduler.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 05:30:36.644909 mns-scheduler-1.0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      212 2024-04-12 05:29:56.000000 mns-scheduler-1.0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.316477 mns-scheduler-1.0.2.2/
+-rw-rw-rw-   0        0        0       62 2024-04-13 06:50:59.315478 mns-scheduler-1.0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1357 2023-12-16 03:56:24.000000 mns-scheduler-1.0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.276582 mns-scheduler-1.0.2.2/mns_scheduler/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.2/mns_scheduler/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.279574 mns-scheduler-1.0.2.2/mns_scheduler/big_deal/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.2/mns_scheduler/big_deal/__init__.py
+-rw-rw-rw-   0        0        0     4555 2023-12-22 04:57:03.000000 mns-scheduler-1.0.2.2/mns_scheduler/big_deal/ths_big_deal_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.280572 mns-scheduler-1.0.2.2/mns_scheduler/company_info/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/company_info/__init__.py
+-rw-rw-rw-   0        0        0    15238 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.2/mns_scheduler/company_info/company_constant_data.py
+-rw-rw-rw-   0        0        0    20330 2024-04-11 14:07:31.000000 mns-scheduler-1.0.2.2/mns_scheduler/company_info/company_info_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.281570 mns-scheduler-1.0.2.2/mns_scheduler/concept/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.281570 mns-scheduler-1.0.2.2/mns_scheduler/concept/clean/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/clean/__init__.py
+-rw-rw-rw-   0        0        0     2440 2024-03-22 08:13:08.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.283564 mns-scheduler-1.0.2.2/mns_scheduler/concept/em/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/em/__init__.py
+-rw-rw-rw-   0        0        0     4993 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/em/em_new_concept_his_sync.py
+-rw-rw-rw-   0        0        0     7083 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/em/em_new_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     2335 2023-12-22 05:01:59.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/em/em_new_concept_sync_web.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.284562 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.285559 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/app/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/app/__init__.py
+-rw-rw-rw-   0        0        0     5148 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.286556 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/common/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/common/__init__.py
+-rw-rw-rw-   0        0        0    10238 2024-04-13 05:32:34.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+-rw-rw-rw-   0        0        0     1557 2024-04-13 06:44:39.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.288551 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/symbol/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/symbol/__init__.py
+-rw-rw-rw-   0        0        0     1928 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
+-rw-rw-rw-   0        0        0     8574 2024-04-13 06:40:52.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.289548 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/web/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/web/__init__.py
+-rw-rw-rw-   0        0        0     5001 2024-04-13 05:23:41.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
+-rw-rw-rw-   0        0        0     3605 2024-03-21 16:54:56.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.290545 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/wen_cai/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/wen_cai/__init__.py
+-rw-rw-rw-   0        0        0     1747 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.292540 mns-scheduler-1.0.2.2/mns_scheduler/db/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/db/__init__.py
+-rw-rw-rw-   0        0        0     3952 2024-02-28 08:33:00.000000 mns-scheduler-1.0.2.2/mns_scheduler/db/col_move_service.py
+-rw-rw-rw-   0        0        0      747 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/db/db_status.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.293538 mns-scheduler-1.0.2.2/mns_scheduler/dt/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/dt/__init__.py
+-rw-rw-rw-   0        0        0     3466 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/dt/stock_dt_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.294535 mns-scheduler-1.0.2.2/mns_scheduler/ipo/
+-rw-rw-rw-   0        0        0      163 2024-01-08 10:50:26.000000 mns-scheduler-1.0.2.2/mns_scheduler/ipo/__init__.py
+-rw-rw-rw-   0        0        0      387 2024-01-08 10:59:33.000000 mns-scheduler-1.0.2.2/mns_scheduler/ipo/auto_ipo_buy_api.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.294535 mns-scheduler-1.0.2.2/mns_scheduler/k_line/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/k_line/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.299522 mns-scheduler-1.0.2.2/mns_scheduler/k_line/clean/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/k_line/clean/__init__.py
+-rw-rw-rw-   0        0        0    21833 2024-01-09 10:50:36.000000 mns-scheduler-1.0.2.2/mns_scheduler/k_line/clean/k_line_info_clean_impl.py
+-rw-rw-rw-   0        0        0     7028 2024-01-09 10:50:05.000000 mns-scheduler-1.0.2.2/mns_scheduler/k_line/clean/k_line_info_clean_service.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.302514 mns-scheduler-1.0.2.2/mns_scheduler/k_line/sync/
+-rw-rw-rw-   0        0        0      161 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/k_line/sync/__init__.py
+-rw-rw-rw-   0        0        0     5654 2024-03-29 10:48:40.000000 mns-scheduler-1.0.2.2/mns_scheduler/k_line/sync/daily_week_month_line_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.303511 mns-scheduler-1.0.2.2/mns_scheduler/kpl/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/kpl/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.303511 mns-scheduler-1.0.2.2/mns_scheduler/kpl/selection/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/kpl/selection/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.304507 mns-scheduler-1.0.2.2/mns_scheduler/kpl/selection/index/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.2/mns_scheduler/kpl/selection/index/__init__.py
+-rw-rw-rw-   0        0        0     8016 2024-04-02 13:03:08.000000 mns-scheduler-1.0.2.2/mns_scheduler/kpl/selection/index/sync_best_choose_index.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.305505 mns-scheduler-1.0.2.2/mns_scheduler/kpl/selection/symbol/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.2/mns_scheduler/kpl/selection/symbol/__init__.py
+-rw-rw-rw-   0        0        0     4679 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.2/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.306503 mns-scheduler-1.0.2.2/mns_scheduler/kpl/selection/total/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.2/mns_scheduler/kpl/selection/total/__init__.py
+-rw-rw-rw-   0        0        0     7527 2024-04-02 14:49:34.000000 mns-scheduler-1.0.2.2/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.308497 mns-scheduler-1.0.2.2/mns_scheduler/real_time/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/real_time/__init__.py
+-rw-rw-rw-   0        0        0     1066 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.2/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py
+-rw-rw-rw-   0        0        0     8850 2024-04-01 01:27:55.000000 mns-scheduler-1.0.2.2/mns_scheduler/real_time/realtime_quotes_now_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.309496 mns-scheduler-1.0.2.2/mns_scheduler/zb/
+-rw-rw-rw-   0        0        0      165 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/zb/__init__.py
+-rw-rw-rw-   0        0        0     1936 2023-12-17 03:50:52.000000 mns-scheduler-1.0.2.2/mns_scheduler/zb/stock_zb_pool_sync.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.312486 mns-scheduler-1.0.2.2/mns_scheduler/zt/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/zt/__init__.py
+-rw-rw-rw-   0        0        0     4015 2023-12-17 13:29:39.000000 mns-scheduler-1.0.2.2/mns_scheduler/zt/export_open_data_to_excel.py
+-rw-rw-rw-   0        0        0    17269 2024-03-09 09:58:27.000000 mns-scheduler-1.0.2.2/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py
+-rw-rw-rw-   0        0        0    21283 2024-01-04 12:05:04.000000 mns-scheduler-1.0.2.2/mns_scheduler/zt/today_high_chg_pool_sync_api.py
+-rw-rw-rw-   0        0        0    10916 2023-12-19 00:49:10.000000 mns-scheduler-1.0.2.2/mns_scheduler/zt/zt_five_boards_sync_api.py
+-rw-rw-rw-   0        0        0     7534 2024-04-12 05:21:45.000000 mns-scheduler-1.0.2.2/mns_scheduler/zt/zt_pool_sync_api.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.314482 mns-scheduler-1.0.2.2/mns_scheduler/zz_task/
+-rw-rw-rw-   0        0        0      163 2023-12-19 00:49:11.000000 mns-scheduler-1.0.2.2/mns_scheduler/zz_task/__init__.py
+-rw-rw-rw-   0        0        0    13768 2024-04-02 14:52:18.000000 mns-scheduler-1.0.2.2/mns_scheduler/zz_task/data_sync_task.py
+-rw-rw-rw-   0        0        0      932 2024-03-23 03:12:05.000000 mns-scheduler-1.0.2.2/mns_scheduler/zz_task/sync_realtime_quotes_task.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:50:59.315478 mns-scheduler-1.0.2.2/mns_scheduler.egg-info/
+-rw-rw-rw-   0        0        0       62 2024-04-13 06:50:59.000000 mns-scheduler-1.0.2.2/mns_scheduler.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3014 2024-04-13 06:50:59.000000 mns-scheduler-1.0.2.2/mns_scheduler.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 06:50:59.000000 mns-scheduler-1.0.2.2/mns_scheduler.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2024-04-13 06:50:59.000000 mns-scheduler-1.0.2.2/mns_scheduler.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-13 06:50:59.316477 mns-scheduler-1.0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      212 2024-04-13 06:49:11.000000 mns-scheduler-1.0.2.2/setup.py
```

### Comparing `mns-scheduler-1.0.2.1/README.md` & `mns-scheduler-1.0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/big_deal/ths_big_deal_sync.py` & `mns-scheduler-1.0.2.2/mns_scheduler/big_deal/ths_big_deal_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/company_info/company_constant_data.py` & `mns-scheduler-1.0.2.2/mns_scheduler/company_info/company_constant_data.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/company_info/company_info_sync_api.py` & `mns-scheduler-1.0.2.2/mns_scheduler/company_info/company_info_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py` & `mns-scheduler-1.0.2.2/mns_scheduler/concept/clean/ths_effective_concept_clean_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/concept/em/em_new_concept_his_sync.py` & `mns-scheduler-1.0.2.2/mns_scheduler/concept/em/em_new_concept_his_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/concept/em/em_new_concept_sync_common_api.py` & `mns-scheduler-1.0.2.2/mns_scheduler/concept/em/em_new_concept_sync_common_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/concept/em/em_new_concept_sync_web.py` & `mns-scheduler-1.0.2.2/mns_scheduler/concept/em/em_new_concept_sync_web.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py` & `mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py` & `mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 file_path = os.path.abspath(__file__)
 end = file_path.index('mns') + 17
 project_path = file_path[0:end]
 sys.path.append(project_path)
 mongodb_util = MongodbUtil('27017')
 import mns_common.api.msg.push_msg_api as push_msg_api
 import mns_scheduler.company_info.company_info_sync_api as company_info_sync_api
-
+import mns_common.utils.data_frame_util as data_frame_util
 max_concept_code = 886110
 
 order_fields = [
     "index",
     "symbol",
     "name",
     "now_price",
```

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py` & `mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py` & `mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 from mns_common.db.MongodbUtil import MongodbUtil
 from loguru import logger
 import mns_common.utils.data_frame_util as data_frame_util
 from datetime import datetime
 from mns_common.utils.async_fun import async_fun
 import mns_scheduler.concept.ths.common.ths_concept_sync_common_api as ths_concept_sync_common_api
 import threading
+import mns_scheduler.concept.ths.common.ths_concept_update_common_api as ths_concept_update_common_api
 
 file_path = os.path.abspath(__file__)
 end = file_path.index('mns') + 17
 project_path = file_path[0:end]
 sys.path.append(project_path)
 mongodb_util = MongodbUtil('27017')
 # 分页大小
@@ -86,14 +87,16 @@
         try:
             ths_concept_json = ths_stock_api.get_symbol_add_new_concept(stock_one.symbol)
             logger.info("同步symbol概念信息:{}", stock_one.symbol)
             symbol_ths_concept_all_df = pd.DataFrame(ths_concept_json)
             if data_frame_util.is_empty(symbol_ths_concept_all_df):
                 continue
 
+            ths_concept_update_common_api.update_ths_concept_detail(symbol_ths_concept_all_df, stock_one.symbol)
+
             now_date = datetime.now()
             str_day = now_date.strftime('%Y-%m-%d')
             str_now_date = now_date.strftime('%Y-%m-%d %H:%M:%S')
             symbol_ths_concept_all_df.loc[:, 'str_day'] = str_day
             symbol_ths_concept_all_df.loc[:, 'str_now_date'] = str_now_date
             symbol_ths_concept_all_df.loc[:, 'symbol'] = stock_one.symbol
             symbol_ths_concept_all_df.loc[:, 'name'] = stock_one.name
@@ -154,15 +157,18 @@
     page_number = round(count / MAX_PAGE_NUMBER, 0) + 1
     page_number = int(page_number)
     threads = []
     # 创建多个线程来获取数据
     for page in range(page_number):  # 0到100页
         end_count = (page + 1) * MAX_PAGE_NUMBER
         begin_count = page * MAX_PAGE_NUMBER
-        page_df = real_time_quotes_now.loc[begin_count:end_count]
+        if symbol is None:
+            page_df = real_time_quotes_now.loc[begin_count:end_count]
+        else:
+            page_df = real_time_quotes_now
         thread = threading.Thread(target=update_symbol_new_concept, args=(page_df, page_number))
         threads.append(thread)
         thread.start()
 
     # 等待所有线程完成
     for thread in threads:
         thread.join()
```

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py` & `mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
                     '_id': int(concept_code),
                     'symbol': int(concept_code),
                     'name': concept_one.concept_name,
                     'url': concept_one.url,
                     'str_day': str_day,
                     'success': True,
                     'str_now_time': str_now_time,
-                    'web_concept_code': concept_one.concept_code,
+                    'web_concept_code': int(concept_one.concept_code),
                     'web_concept_url': concept_one.url,
                     'valid': True
                 }
                 diff_one_df = pd.DataFrame(diff_one, index=[1])
                 mongodb_util.save_mongo(diff_one_df, 'ths_concept_list')
                 url = 'http://q.10jqka.com.cn/gn/detail/code/' + str(concept_one.concept_code)
                 # 推送新概念信息到微信
```

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py` & `mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py` & `mns-scheduler-1.0.2.2/mns_scheduler/concept/ths/wen_cai/wen_cai_concept_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/db/col_move_service.py` & `mns-scheduler-1.0.2.2/mns_scheduler/db/col_move_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/db/db_status.py` & `mns-scheduler-1.0.2.2/mns_scheduler/db/db_status.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/dt/stock_dt_pool_sync.py` & `mns-scheduler-1.0.2.2/mns_scheduler/dt/stock_dt_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/k_line/clean/k_line_info_clean_impl.py` & `mns-scheduler-1.0.2.2/mns_scheduler/k_line/clean/k_line_info_clean_impl.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/k_line/clean/k_line_info_clean_service.py` & `mns-scheduler-1.0.2.2/mns_scheduler/k_line/clean/k_line_info_clean_service.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/k_line/sync/daily_week_month_line_sync.py` & `mns-scheduler-1.0.2.2/mns_scheduler/k_line/sync/daily_week_month_line_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/kpl/selection/index/sync_best_choose_index.py` & `mns-scheduler-1.0.2.2/mns_scheduler/kpl/selection/index/sync_best_choose_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py` & `mns-scheduler-1.0.2.2/mns_scheduler/kpl/selection/symbol/sync_best_choose_symbol.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py` & `mns-scheduler-1.0.2.2/mns_scheduler/kpl/selection/total/sync_kpl_best_total_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py` & `mns-scheduler-1.0.2.2/mns_scheduler/real_time/realtime_quotes_now_create_db_index.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/real_time/realtime_quotes_now_sync.py` & `mns-scheduler-1.0.2.2/mns_scheduler/real_time/realtime_quotes_now_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/zb/stock_zb_pool_sync.py` & `mns-scheduler-1.0.2.2/mns_scheduler/zb/stock_zb_pool_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/zt/export_open_data_to_excel.py` & `mns-scheduler-1.0.2.2/mns_scheduler/zt/export_open_data_to_excel.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py` & `mns-scheduler-1.0.2.2/mns_scheduler/zt/realtime_quotes_now_zt_kc_sync.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/zt/today_high_chg_pool_sync_api.py` & `mns-scheduler-1.0.2.2/mns_scheduler/zt/today_high_chg_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/zt/zt_five_boards_sync_api.py` & `mns-scheduler-1.0.2.2/mns_scheduler/zt/zt_five_boards_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/zt/zt_pool_sync_api.py` & `mns-scheduler-1.0.2.2/mns_scheduler/zt/zt_pool_sync_api.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/zz_task/data_sync_task.py` & `mns-scheduler-1.0.2.2/mns_scheduler/zz_task/data_sync_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler/zz_task/sync_realtime_quotes_task.py` & `mns-scheduler-1.0.2.2/mns_scheduler/zz_task/sync_realtime_quotes_task.py`

 * *Files identical despite different names*

### Comparing `mns-scheduler-1.0.2.1/mns_scheduler.egg-info/SOURCES.txt` & `mns-scheduler-1.0.2.2/mns_scheduler.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 mns_scheduler/concept/em/em_new_concept_sync_common_api.py
 mns_scheduler/concept/em/em_new_concept_sync_web.py
 mns_scheduler/concept/ths/__init__.py
 mns_scheduler/concept/ths/app/__init__.py
 mns_scheduler/concept/ths/app/ths_new_concept_sync_app.py
 mns_scheduler/concept/ths/common/__init__.py
 mns_scheduler/concept/ths/common/ths_concept_sync_common_api.py
+mns_scheduler/concept/ths/common/ths_concept_update_common_api.py
 mns_scheduler/concept/ths/symbol/__init__.py
 mns_scheduler/concept/ths/symbol/sync_concept_all_symbols_api.py
 mns_scheduler/concept/ths/symbol/sync_symbol_all_concepts_api.py
 mns_scheduler/concept/ths/web/__init__.py
 mns_scheduler/concept/ths/web/sync_ths_concept_by_ak_api.py
 mns_scheduler/concept/ths/web/sync_ths_new_concept_by_web_api.py
 mns_scheduler/concept/ths/wen_cai/__init__.py
```

