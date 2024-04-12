# Comparing `tmp/investing_algorithm_framework-3.4.3.tar.gz` & `tmp/investing_algorithm_framework-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investing_algorithm_framework-3.4.3.tar", max compression
+gzip compressed data, was "investing_algorithm_framework-3.5.0.tar", max compression
```

## Comparing `investing_algorithm_framework-3.4.3.tar` & `investing_algorithm_framework-3.5.0.tar`

### file list

```diff
@@ -1,142 +1,142 @@
--rw-r--r--   0        0        0    11343 2024-04-05 11:08:02.359881 investing_algorithm_framework-3.4.3/LICENSE
--rw-r--r--   0        0        0    19512 2024-04-05 11:08:02.359881 investing_algorithm_framework-3.4.3/README.md
--rw-r--r--   0        0        0     2084 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/__init__.py
--rw-r--r--   0        0        0      501 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/__init__.py
--rw-r--r--   0        0        0    34948 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/algorithm.py
--rw-r--r--   0        0        0    31166 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/app.py
--rw-r--r--   0        0        0     1092 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/stateless/__init__.py
--rw-r--r--   0        0        0     2362 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
--rw-r--r--   0        0        0      154 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
--rw-r--r--   0        0        0      451 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
--rw-r--r--   0        0        0     1062 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
--rw-r--r--   0        0        0     1085 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/stateless/exception_handler.py
--rw-r--r--   0        0        0     3750 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/strategy.py
--rw-r--r--   0        0        0      963 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/task.py
--rw-r--r--   0        0        0      134 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/__init__.py
--rw-r--r--   0        0        0      587 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/controllers/__init__.py
--rw-r--r--   0        0        0      693 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/controllers/orders.py
--rw-r--r--   0        0        0      727 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/controllers/portfolio.py
--rw-r--r--   0        0        0      617 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/controllers/positions.py
--rw-r--r--   0        0        0      506 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/create_app.py
--rw-r--r--   0        0        0     2020 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/error_handler.py
--rw-r--r--   0        0        0      585 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/responses.py
--rw-r--r--   0        0        0      158 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/run_strategies.py
--rw-r--r--   0        0        0      361 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/schemas/__init__.py
--rw-r--r--   0        0        0      442 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/schemas/order.py
--rw-r--r--   0        0        0      743 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/schemas/portfolio.py
--rw-r--r--   0        0        0      437 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/schemas/position.py
--rw-r--r--   0        0        0       80 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/setup_cors.py
--rw-r--r--   0        0        0      603 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/create_app.py
--rw-r--r--   0        0        0     6312 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/dependency_container.py
--rw-r--r--   0        0        0     3913 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/__init__.py
--rw-r--r--   0        0        0     3728 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/config.py
--rw-r--r--   0        0        0     2293 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/constants.py
--rw-r--r--   0        0        0      962 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/data_structures.py
--rw-r--r--   0        0        0      823 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/decimal_parsing.py
--rw-r--r--   0        0        0     1628 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/exceptions.py
--rw-r--r--   0        0        0     1121 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/__init__.py
--rw-r--r--   0        0        0      812 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/app_mode.py
--rw-r--r--   0        0        0      253 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/backtesting/__init__.py
--rw-r--r--   0        0        0     2374 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/backtesting/backtest_position.py
--rw-r--r--   0        0        0    13604 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/backtesting/backtest_report.py
--rw-r--r--   0        0        0      674 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py
--rw-r--r--   0        0        0      659 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/base_model.py
--rw-r--r--   0        0        0       87 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/market/__init__.py
--rw-r--r--   0        0        0      779 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/market/market_credential.py
--rw-r--r--   0        0        0      237 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/order/__init__.py
--rw-r--r--   0        0        0    10194 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/order/order.py
--rw-r--r--   0        0        0     1110 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/order/order_fee.py
--rw-r--r--   0        0        0      814 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/order/order_side.py
--rw-r--r--   0        0        0      937 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/order/order_status.py
--rw-r--r--   0        0        0      751 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/order/order_type.py
--rw-r--r--   0        0        0      230 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/portfolio/__init__.py
--rw-r--r--   0        0        0     2495 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/portfolio/portfolio.py
--rw-r--r--   0        0        0     1752 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
--rw-r--r--   0        0        0     3141 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py
--rw-r--r--   0        0        0      123 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/position/__init__.py
--rw-r--r--   0        0        0     1251 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/position/position.py
--rw-r--r--   0        0        0     1131 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/position/position_snapshot.py
--rw-r--r--   0        0        0     4598 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/strategy_profile.py
--rw-r--r--   0        0        0     2659 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/time_frame.py
--rw-r--r--   0        0        0     2798 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/time_interval.py
--rw-r--r--   0        0        0     2011 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/time_unit.py
--rw-r--r--   0        0        0       99 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/trade/__init__.py
--rw-r--r--   0        0        0     7112 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/trade/trade.py
--rw-r--r--   0        0        0      807 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/trade/trade_status.py
--rw-r--r--   0        0        0     1119 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/trading_data_types.py
--rw-r--r--   0        0        0     6791 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/trading_time_frame.py
--rw-r--r--   0        0        0      634 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/services/__init__.py
--rw-r--r--   0        0        0     1047 2024-04-05 11:08:02.363881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/services/market_credential_service.py
--rw-r--r--   0        0        0     9941 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/services/market_data_sources.py
--rw-r--r--   0        0        0     3520 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/services/market_service.py
--rw-r--r--   0        0        0      115 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/services/portfolios/__init__.py
--rw-r--r--   0        0        0      320 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/services/portfolios/portfolio_sync_service.py
--rw-r--r--   0        0        0      699 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/services/rounding_service.py
--rw-r--r--   0        0        0      258 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/singleton.py
--rw-r--r--   0        0        0      156 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/stateless_actions.py
--rw-r--r--   0        0        0     1805 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/strategy.py
--rw-r--r--   0        0        0      700 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/utils/__init__.py
--rw-r--r--   0        0        0    10969 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/utils/backtesting.py
--rw-r--r--   0        0        0     2746 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/utils/csv.py
--rw-r--r--   0        0        0      275 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/utils/random.py
--rw-r--r--   0        0        0      417 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/utils/signatures.py
--rw-r--r--   0        0        0      608 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/utils/stoppable_thread.py
--rw-r--r--   0        0        0      253 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/utils/synchronized.py
--rw-r--r--   0        0        0     1361 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/__init__.py
--rw-r--r--   0        0        0      176 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/database/__init__.py
--rw-r--r--   0        0        0     1386 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
--rw-r--r--   0        0        0      732 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/__init__.py
--rw-r--r--   0        0        0      327 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/decimal_parser.py
--rw-r--r--   0        0        0      437 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/market_data_sources/__init__.py
--rw-r--r--   0        0        0    17466 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py
--rw-r--r--   0        0        0     5472 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py
--rw-r--r--   0        0        0      142 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/model_extension.py
--rw-r--r--   0        0        0      102 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/order/__init__.py
--rw-r--r--   0        0        0     4877 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/order/order.py
--rw-r--r--   0        0        0      847 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/order/order_fee.py
--rw-r--r--   0        0        0      141 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
--rw-r--r--   0        0        0     3226 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
--rw-r--r--   0        0        0     1238 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py
--rw-r--r--   0        0        0      135 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/position/__init__.py
--rw-r--r--   0        0        0     1898 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/position/position.py
--rw-r--r--   0        0        0      842 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py
--rw-r--r--   0        0        0      567 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/repositories/__init__.py
--rw-r--r--   0        0        0      487 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
--rw-r--r--   0        0        0     3352 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/repositories/order_repository.py
--rw-r--r--   0        0        0     1073 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
--rw-r--r--   0        0        0     1967 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py
--rw-r--r--   0        0        0     1994 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/repositories/position_repository.py
--rw-r--r--   0        0        0      680 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py
--rw-r--r--   0        0        0     7661 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/repositories/repository.py
--rw-r--r--   0        0        0      163 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/services/__init__.py
--rw-r--r--   0        0        0       91 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/services/market_service/__init__.py
--rw-r--r--   0        0        0    15303 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py
--rw-r--r--   0        0        0      195 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/services/performance_service/__init__.py
--rw-r--r--   0        0        0       43 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/services/performance_service/backtest_performance_service.py
--rw-r--r--   0        0        0    11932 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py
--rw-r--r--   0        0        0     1318 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/__init__.py
--rw-r--r--   0        0        0      191 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/backtesting/__init__.py
--rw-r--r--   0        0        0     1025 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py
--rw-r--r--   0        0        0    15007 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/backtesting/backtest_service.py
--rw-r--r--   0        0        0      624 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/configuration_service.py
--rw-r--r--   0        0        0      820 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/market_credential_service.py
--rw-r--r--   0        0        0      235 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/market_data_source_service/__init__.py
--rw-r--r--   0        0        0     5213 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py
--rw-r--r--   0        0        0     6267 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py
--rw-r--r--   0        0        0      159 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/order_service/__init__.py
--rw-r--r--   0        0        0     7735 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/order_service/order_backtest_service.py
--rw-r--r--   0        0        0    27823 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/order_service/order_service.py
--rw-r--r--   0        0        0      510 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/portfolios/__init__.py
--rw-r--r--   0        0        0      825 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py
--rw-r--r--   0        0        0     2055 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py
--rw-r--r--   0        0        0     4493 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/portfolios/portfolio_service.py
--rw-r--r--   0        0        0     1984 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py
--rw-r--r--   0        0        0    16126 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py
--rw-r--r--   0        0        0     1052 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/position_service.py
--rw-r--r--   0        0        0      525 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/position_snapshot_service.py
--rw-r--r--   0        0        0      995 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/repository_service.py
--rw-r--r--   0        0        0     8075 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/strategy_orchestrator_service.py
--rw-r--r--   0        0        0       68 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/trade_service/__init__.py
--rw-r--r--   0        0        0    14761 2024-04-05 11:08:02.367881 investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/trade_service/trade_service.py
--rw-r--r--   0        0        0      742 2024-04-05 11:08:10.351935 investing_algorithm_framework-3.4.3/pyproject.toml
--rw-r--r--   0        0        0    20584 1970-01-01 00:00:00.000000 investing_algorithm_framework-3.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-04-12 09:32:30.550392 investing_algorithm_framework-3.5.0/LICENSE
+-rw-r--r--   0        0        0    21956 2024-04-12 09:32:30.550392 investing_algorithm_framework-3.5.0/README.md
+-rw-r--r--   0        0        0     2084 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/__init__.py
+-rw-r--r--   0        0        0      501 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/__init__.py
+-rw-r--r--   0        0        0    34948 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/algorithm.py
+-rw-r--r--   0        0        0    32187 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/app.py
+-rw-r--r--   0        0        0     1092 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/__init__.py
+-rw-r--r--   0        0        0     2362 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
+-rw-r--r--   0        0        0      452 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
+-rw-r--r--   0        0        0     1062 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
+-rw-r--r--   0        0        0     1085 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/exception_handler.py
+-rw-r--r--   0        0        0     3750 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/strategy.py
+-rw-r--r--   0        0        0      963 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/task.py
+-rw-r--r--   0        0        0      134 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/__init__.py
+-rw-r--r--   0        0        0      694 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/orders.py
+-rw-r--r--   0        0        0      727 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/portfolio.py
+-rw-r--r--   0        0        0      617 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/positions.py
+-rw-r--r--   0        0        0      506 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/create_app.py
+-rw-r--r--   0        0        0     2020 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/error_handler.py
+-rw-r--r--   0        0        0      585 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/responses.py
+-rw-r--r--   0        0        0      158 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/run_strategies.py
+-rw-r--r--   0        0        0      361 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/schemas/__init__.py
+-rw-r--r--   0        0        0      442 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/schemas/order.py
+-rw-r--r--   0        0        0      743 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/schemas/portfolio.py
+-rw-r--r--   0        0        0      438 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/schemas/position.py
+-rw-r--r--   0        0        0       80 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/setup_cors.py
+-rw-r--r--   0        0        0      603 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/create_app.py
+-rw-r--r--   0        0        0     6312 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/dependency_container.py
+-rw-r--r--   0        0        0     3912 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/__init__.py
+-rw-r--r--   0        0        0     3728 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/config.py
+-rw-r--r--   0        0        0     2293 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/constants.py
+-rw-r--r--   0        0        0      962 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/data_structures.py
+-rw-r--r--   0        0        0      823 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/decimal_parsing.py
+-rw-r--r--   0        0        0     1628 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/exceptions.py
+-rw-r--r--   0        0        0     1121 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/app_mode.py
+-rw-r--r--   0        0        0      253 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/backtesting/__init__.py
+-rw-r--r--   0        0        0     2374 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/backtesting/backtest_position.py
+-rw-r--r--   0        0        0    13619 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/backtesting/backtest_report.py
+-rw-r--r--   0        0        0     2309 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py
+-rw-r--r--   0        0        0      659 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/base_model.py
+-rw-r--r--   0        0        0       87 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/market/__init__.py
+-rw-r--r--   0        0        0      779 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/market/market_credential.py
+-rw-r--r--   0        0        0      237 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/__init__.py
+-rw-r--r--   0        0        0    10363 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order.py
+-rw-r--r--   0        0        0     1110 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_fee.py
+-rw-r--r--   0        0        0      814 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_side.py
+-rw-r--r--   0        0        0      937 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_status.py
+-rw-r--r--   0        0        0      751 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_type.py
+-rw-r--r--   0        0        0      230 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/portfolio/__init__.py
+-rw-r--r--   0        0        0     2495 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py
+-rw-r--r--   0        0        0     1752 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
+-rw-r--r--   0        0        0     3141 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py
+-rw-r--r--   0        0        0      123 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/position/__init__.py
+-rw-r--r--   0        0        0     1251 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/position/position.py
+-rw-r--r--   0        0        0     1131 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/position/position_snapshot.py
+-rw-r--r--   0        0        0     4598 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/strategy_profile.py
+-rw-r--r--   0        0        0     2659 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/time_frame.py
+-rw-r--r--   0        0        0     2798 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/time_interval.py
+-rw-r--r--   0        0        0     2011 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/time_unit.py
+-rw-r--r--   0        0        0       99 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trade/__init__.py
+-rw-r--r--   0        0        0     7114 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trade/trade.py
+-rw-r--r--   0        0        0      807 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trade/trade_status.py
+-rw-r--r--   0        0        0     1119 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trading_data_types.py
+-rw-r--r--   0        0        0     6791 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trading_time_frame.py
+-rw-r--r--   0        0        0      634 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/__init__.py
+-rw-r--r--   0        0        0     1047 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/market_credential_service.py
+-rw-r--r--   0        0        0     9941 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/market_data_sources.py
+-rw-r--r--   0        0        0     3522 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/market_service.py
+-rw-r--r--   0        0        0      115 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/portfolios/__init__.py
+-rw-r--r--   0        0        0      320 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/portfolios/portfolio_sync_service.py
+-rw-r--r--   0        0        0      699 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/rounding_service.py
+-rw-r--r--   0        0        0      258 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/singleton.py
+-rw-r--r--   0        0        0      156 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/stateless_actions.py
+-rw-r--r--   0        0        0     1805 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/strategy.py
+-rw-r--r--   0        0        0      700 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/__init__.py
+-rw-r--r--   0        0        0    25794 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/backtesting.py
+-rw-r--r--   0        0        0     2746 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/csv.py
+-rw-r--r--   0        0        0      275 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/random.py
+-rw-r--r--   0        0        0      417 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/signatures.py
+-rw-r--r--   0        0        0      608 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/stoppable_thread.py
+-rw-r--r--   0        0        0      253 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/synchronized.py
+-rw-r--r--   0        0        0     1361 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/database/__init__.py
+-rw-r--r--   0        0        0     1386 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
+-rw-r--r--   0        0        0      732 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/__init__.py
+-rw-r--r--   0        0        0      327 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/decimal_parser.py
+-rw-r--r--   0        0        0      437 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/market_data_sources/__init__.py
+-rw-r--r--   0        0        0    17349 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py
+-rw-r--r--   0        0        0     5472 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py
+-rw-r--r--   0        0        0      142 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/model_extension.py
+-rw-r--r--   0        0        0      102 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/order/__init__.py
+-rw-r--r--   0        0        0     4877 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/order/order.py
+-rw-r--r--   0        0        0      847 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/order/order_fee.py
+-rw-r--r--   0        0        0      141 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
+-rw-r--r--   0        0        0     3226 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
+-rw-r--r--   0        0        0     1238 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py
+-rw-r--r--   0        0        0      135 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/position/__init__.py
+-rw-r--r--   0        0        0     1898 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/position/position.py
+-rw-r--r--   0        0        0      842 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py
+-rw-r--r--   0        0        0      567 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/__init__.py
+-rw-r--r--   0        0        0      487 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
+-rw-r--r--   0        0        0     3351 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py
+-rw-r--r--   0        0        0     1073 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
+-rw-r--r--   0        0        0     1967 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py
+-rw-r--r--   0        0        0     1994 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py
+-rw-r--r--   0        0        0      680 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py
+-rw-r--r--   0        0        0     7661 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/repository.py
+-rw-r--r--   0        0        0      163 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/market_service/__init__.py
+-rw-r--r--   0        0        0    15303 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py
+-rw-r--r--   0        0        0      195 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/performance_service/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/performance_service/backtest_performance_service.py
+-rw-r--r--   0        0        0    11933 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py
+-rw-r--r--   0        0        0     1318 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/backtesting/__init__.py
+-rw-r--r--   0        0        0     1401 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py
+-rw-r--r--   0        0        0    15031 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/backtesting/backtest_service.py
+-rw-r--r--   0        0        0      624 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/configuration_service.py
+-rw-r--r--   0        0        0      821 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/market_credential_service.py
+-rw-r--r--   0        0        0      235 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/market_data_source_service/__init__.py
+-rw-r--r--   0        0        0     5214 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py
+-rw-r--r--   0        0        0     6307 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py
+-rw-r--r--   0        0        0      159 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/order_service/__init__.py
+-rw-r--r--   0        0        0     7735 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/order_service/order_backtest_service.py
+-rw-r--r--   0        0        0    27824 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/order_service/order_service.py
+-rw-r--r--   0        0        0      509 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/__init__.py
+-rw-r--r--   0        0        0      825 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py
+-rw-r--r--   0        0        0     2055 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py
+-rw-r--r--   0        0        0     4493 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_service.py
+-rw-r--r--   0        0        0     1984 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py
+-rw-r--r--   0        0        0    16127 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py
+-rw-r--r--   0        0        0     1052 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/position_service.py
+-rw-r--r--   0        0        0      525 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/position_snapshot_service.py
+-rw-r--r--   0        0        0      995 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/repository_service.py
+-rw-r--r--   0        0        0     8077 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/strategy_orchestrator_service.py
+-rw-r--r--   0        0        0       68 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/trade_service/__init__.py
+-rw-r--r--   0        0        0    14761 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/trade_service/trade_service.py
+-rw-r--r--   0        0        0      742 2024-04-12 09:32:38.370404 investing_algorithm_framework-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0    23028 1970-01-01 00:00:00.000000 investing_algorithm_framework-3.5.0/PKG-INFO
```

### Comparing `investing_algorithm_framework-3.4.3/LICENSE` & `investing_algorithm_framework-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/README.md` & `investing_algorithm_framework-3.5.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -135,60 +135,74 @@
 
 ### Backtesting report
 You can use the ```pretty_print_backtest``` function to print a backtest report.
 For example if you run the [moving average example trading bot](./examples/crossover_moving_average_trading_bot)
 you will get the following backtesting report:
  
 ```bash
-====================Backtest report===============================
-* Start date: 2023-08-24 00:00:00
-* End date: 2023-12-02 00:00:00
-* Number of days: 100
-* Number of runs: 1201
-====================Portfolio overview============================
-* Number of orders: 10
-* Initial balance: 400.0000 EUR
-* Final balance: 431.8837 EUR
-* Total net gain: 28.4171 EUR
-* Total net gain percentage: 7.1043%
-* Growth rate: 7.9709%
-* Growth 31.8837 EUR
-====================Positions overview========================
+
+                          /&#                                      #&(                 Backtest report
+                          &&&&&&&&&&&#                       &&&&&&&&&&&&              ---------------------------
+                         &&&&&&&&&&&&&&&&                (&&&&&&&&&&&&&&&              Start date: 2023-08-24 00:00:00
+                         &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&              End date: 2023-12-02 00:00:00
+                         &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&              Number of days: 100 
+                          &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&              Number of runs: 1201
+                          .&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&               Number of orders: 10
+                           &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&.               Initial balance: 400.0
+                          &&&&&&&#  /(((   &&&&&&&&&&&&*(((     .&&&&&&&.              Final balance: 431.1499      
+              &&&&&&&&&&&&&&&&&&&    ((((    &&&&&&&&   ((((     &&&&&&&&&&&&&&&&&&&   Total net gain: 28.5542 7.139%  
+                       (((&&&&&&&&    ((((    &&&&&&     ((((   &&&&&&&&&((            Growth: 31.1499 7.787%             
+               /((((((((((&&&&&&&&&&   (((,   &&&&&&      (((**&&&&&&&&&(((((((((((    Number of trades closed: 4
+                     &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&          Number of trades open(end of backtest): 2
+                            &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&                 Percentage positive trades: 60.0%
+                              &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&                   Percentage negative trades: 20.0%
+                     (((((      &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&(                      Average trade size: 98.9886 EUR
+                    (((((           &&&&&&&&&&&&&&&&&&&&&&&&,                          Average trade duration: 184.0 hours
+                   (((((                 &&&&&&&&&&&&&#                            
+                  (((((                  #&&&&&&&&&&###                            
+                 (((((                   &&&&&&&&&&&###.                           
+               .(((((                   &&&&&&&&&&&&&&###(                          
+              (((((                   &&&&&&&&&&&&&&&&#(((/                        
+             (((((                  &&&&&&&&&&&&&&&&&&&@((((                       
+            (((((                  &&&&&&&&&&&&&&&&&&&&&&((((                      
+           (((((                  &&&&&&&&&&&&&&&&&&&&&&&&((((,                    
+         .(((((                   &&&&&&&&&&&&&&&&&&&&&&&&&&((((                    
+        (((((                   &&&&&&&&&&&&&&&&&&&&&&&&&&&&((((                   
+       (((((                    &&&&&&&&&&&&&&&&&&&&&&&&&&&&&((((                  
+      (((((                    &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&((((                  
+     (((((                     &&&&&&&&&&&&&&&&&&&&&&&&&&&&&#((((                  
+     (((((((((((((((((((#########&&&&&&&&&&&&&&&&&&&&&&&&&&&&(((((                  
+      (((((((((((((((((((((######&&&&&&&&&&&&&&&&&&&&&&&&&&&&((((                   
+        
+Positions overview
 ╭────────────┬──────────┬──────────────────────┬───────────────────────┬──────────────┬───────────────┬───────────────────────────┬────────────────┬───────────────╮
 │ Position   │   Amount │   Pending buy amount │   Pending sell amount │   Cost (EUR) │   Value (EUR) │ Percentage of portfolio   │   Growth (EUR) │ Growth_rate   │
 ├────────────┼──────────┼──────────────────────┼───────────────────────┼──────────────┼───────────────┼───────────────────────────┼────────────────┼───────────────┤
-│ EUR        │ 214.219  │                    0 │                     0 │      214.219 │       214.219 │ 49.6010%                  │         0      │ 0.0000%       │
+│ EUR        │ 217.044  │                    0 │                     0 │      217.044 │       217.044 │ 50.3407%                  │         0      │ 0.0000%       │
 ├────────────┼──────────┼──────────────────────┼───────────────────────┼──────────────┼───────────────┼───────────────────────────┼────────────────┼───────────────┤
-│ BTC        │   0.0031 │                    0 │                     0 │      107.095 │       110.401 │ 25.5627%                  │         3.3066 │ 3.0875%       │
+│ BTC        │   0.003  │                    0 │                     0 │      104.372 │       106.84  │ 24.7802%                  │         2.4678 │ 2.3644%       │
 ├────────────┼──────────┼──────────────────────┼───────────────────────┼──────────────┼───────────────┼───────────────────────────┼────────────────┼───────────────┤
-│ DOT        │  21.3291 │                    0 │                     0 │      107.104 │       107.264 │ 24.8363%                  │         0.16   │ 0.1494%       │
+│ DOT        │  21.3295 │                    0 │                     0 │      107.138 │       107.266 │ 24.8791%                  │         0.128  │ 0.1195%       │
 ╰────────────┴──────────┴──────────────────────┴───────────────────────┴──────────────┴───────────────┴───────────────────────────┴────────────────┴───────────────╯
-====================Trades overview===========================
-* Number of trades closed: 4
-* Number of trades open: 2
-* Percentage of positive trades: 60.0%
-* Percentage of negative trades: 20.0%
-* Average trade size: 98.8728 EUR
-* Average trade duration: 183.5 hours
+Trades overview
 ╭─────────┬─────────────────────┬─────────────────────┬────────────────────┬──────────────┬──────────────────┬───────────────────────┬────────────────────┬─────────────────────╮
 │ Pair    │ Open date           │ Close date          │   Duration (hours) │   Size (EUR) │   Net gain (EUR) │ Net gain percentage   │   Open price (EUR) │   Close price (EUR) │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ DOT-EUR │ 2023-11-30 20:00:00 │                     │            2976.65 │     107.104  │           0      │ 0.0000%               │             5.0215 │                     │
+│ DOT-EUR │ 2023-11-30 18:00:00 │                     │            3207.26 │     107.138  │           0      │ 0.0000%               │             5.023  │                     │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-11-29 14:00:00 │                     │            3006.65 │     107.095  │           0      │ 0.0000%               │         34546.6    │                     │
+│ BTC-EUR │ 2023-11-29 12:00:00 │                     │            3237.26 │     104.372  │           0      │ 0.0000%               │         34790.7    │                     │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-11-08 00:00:00 │ 2023-11-14 16:00:00 │             160    │      99.2265 │           1.3352 │ 1.3456%               │         33075.5    │          33520.6    │
+│ BTC-EUR │ 2023-11-07 22:00:00 │ 2023-11-14 14:00:00 │             160    │      99.2337 │           2.5395 │ 2.5591%               │         33077.9    │          33924.4    │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-11-06 16:00:00 │ 2023-11-06 20:00:00 │               4    │      97.8607 │          -0.0026 │ -0.0026%              │         32620.2    │          32619.4    │
+│ BTC-EUR │ 2023-11-06 14:00:00 │ 2023-11-06 18:00:00 │               4    │      98.2854 │          -0.4248 │ -0.4322%              │         32761.8    │          32620.2    │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ DOT-EUR │ 2023-10-30 06:00:00 │ 2023-11-14 00:00:00 │             354    │     100.551  │          24.8794 │ 24.7430%              │             4.0375 │              5.0365 │
+│ DOT-EUR │ 2023-10-30 04:00:00 │ 2023-11-14 00:00:00 │             356    │     100.537  │          24.2886 │ 24.1588%              │             4.0565 │              5.0365 │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-09-13 16:00:00 │ 2023-09-22 16:00:00 │             216    │      97.8529 │           2.2051 │ 2.2534%               │         24463.2    │          25014.5    │
+│ BTC-EUR │ 2023-09-13 14:00:00 │ 2023-09-22 14:00:00 │             216    │      97.8976 │           2.1508 │ 2.1970%               │         24474.4    │          25012.1    │
 ╰─────────┴─────────────────────┴─────────────────────┴────────────────────┴──────────────┴──────────────────┴───────────────────────┴────────────────────┴─────────────────────╯
-==================================================================
 ```
 
 ### Backtest experiments
 The framework also supports backtest experiments. Backtest experiments allows you to 
 compare multiple algorithms and evaluate their performance. Ideally, 
 you would do this by parameterizing your strategy and creating a factory function that
 creates the algorithm with the different parameters. You can find an example of this
```

#### html2text {}

```diff
@@ -67,68 +67,80 @@
 framework also supports backtesting and performing backtest experiments. After
 a backtest, you can print a report that shows the performance of your trading
 bot. To run a single backtest you can use the example code that can be found
 [here](./examples/backtest). ### Backtesting report You can use the
 ```pretty_print_backtest``` function to print a backtest report. For example if
 you run the [moving average example trading bot](./examples/
 crossover_moving_average_trading_bot) you will get the following backtesting
-report: ```bash ====================Backtest
-report=============================== * Start date: 2023-08-24 00:00:00 * End
-date: 2023-12-02 00:00:00 * Number of days: 100 * Number of runs: 1201
-====================Portfolio overview============================ * Number of
-orders: 10 * Initial balance: 400.0000 EUR * Final balance: 431.8837 EUR *
-Total net gain: 28.4171 EUR * Total net gain percentage: 7.1043% * Growth rate:
-7.9709% * Growth 31.8837 EUR ====================Positions
-overview========================
+report: ```bash /&# #&( Backtest report &&&&&&&&&&&# &&&&&&&&&&&& -------------
+-------------- &&&&&&&&&&&&&&&& (&&&&&&&&&&&&&&& Start date: 2023-08-24 00:00:
+00 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&& End date: 2023-12-02 00:00:
+00 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&& Number of days: 100
+&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&& Number of runs: 1201
+.&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&& Number of orders: 10
+&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&. Initial balance: 400.0 &&&&&&&# /
+((( &&&&&&&&&&&&*((( .&&&&&&&. Final balance: 431.1499 &&&&&&&&&&&&&&&&&&& (((
+( &&&&&&&& (((( &&&&&&&&&&&&&&&&&&& Total net gain: 28.5542 7.139% (((&&&&&&&&
+(((( &&&&&& (((( &&&&&&&&&(( Growth: 31.1499 7.787% /((((((((((&&&&&&&&&& (((,
+&&&&&& (((**&&&&&&&&&((((((((((( Number of trades closed: 4
+&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&& Number of trades open
+(end of backtest): 2 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&& Percentage
+positive trades: 60.0% &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&& Percentage
+negative trades: 20.0% ((((( &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&( Average trade
+size: 98.9886 EUR ((((( &&&&&&&&&&&&&&&&&&&&&&&&, Average trade duration: 184.0
+hours ((((( &&&&&&&&&&&&&# ((((( #&&&&&&&&&&### ((((( &&&&&&&&&&&###. .((((
+( &&&&&&&&&&&&&&###( ((((( &&&&&&&&&&&&&&&&#(((/ ((((( &&&&&&&&&&&&&&&&&&&@(((
+( ((((( &&&&&&&&&&&&&&&&&&&&&&(((( ((((( &&&&&&&&&&&&&&&&&&&&&&&&((((, .((((
+( &&&&&&&&&&&&&&&&&&&&&&&&&&(((( ((((( &&&&&&&&&&&&&&&&&&&&&&&&&&&&(((( ((((
+( &&&&&&&&&&&&&&&&&&&&&&&&&&&&&(((( ((((( &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&(((( ((
+((( &&&&&&&&&&&&&&&&&&&&&&&&&&&&&#(((( ((((((((((((((((((
+(#########&&&&&&&&&&&&&&&&&&&&&&&&&&&&((((( ((((((((((((((((((((
+(######&&&&&&&&&&&&&&&&&&&&&&&&&&&&(((( Positions overview
 â­âââââââââââââ¬âââââââââââ¬âââââââââââââââââââââââ¬ââââââââââââââââââââââââ¬âââââââââââââââ¬ââââââââââââââââ¬ââââââââââââââââââââââââââââ¬âââââââââââââââââ¬ââââââââââââââââ®
 â Position â Amount â Pending buy amount â Pending sell amount â Cost
 (EUR) â Value (EUR) â Percentage of portfolio â Growth (EUR) â
 Growth_rate â
 ââââââââââââââ¼âââââââââââ¼âââââââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââ¼ââââââââââââââââ¼ââââââââââââââââââââââââââââ¼âââââââââââââââââ¼ââââââââââââââââ¤
-â EUR â 214.219 â 0 â 0 â 214.219 â 214.219 â 49.6010% â 0 â
+â EUR â 217.044 â 0 â 0 â 217.044 â 217.044 â 50.3407% â 0 â
 0.0000% â
 ââââââââââââââ¼âââââââââââ¼âââââââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââ¼ââââââââââââââââ¼ââââââââââââââââââââââââââââ¼âââââââââââââââââ¼ââââââââââââââââ¤
-â BTC â 0.0031 â 0 â 0 â 107.095 â 110.401 â 25.5627% â 3.3066
-â 3.0875% â
+â BTC â 0.003 â 0 â 0 â 104.372 â 106.84 â 24.7802% â 2.4678
+â 2.3644% â
 ââââââââââââââ¼âââââââââââ¼âââââââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââ¼ââââââââââââââââ¼ââââââââââââââââââââââââââââ¼âââââââââââââââââ¼ââââââââââââââââ¤
-â DOT â 21.3291 â 0 â 0 â 107.104 â 107.264 â 24.8363% â 0.16
-â 0.1494% â
+â DOT â 21.3295 â 0 â 0 â 107.138 â 107.266 â 24.8791% â 0.128
+â 0.1195% â
 â°âââââââââââââ´âââââââââââ´âââââââââââââââââââââââ´ââââââââââââââââââââââââ´âââââââââââââââ´ââââââââââââââââ´ââââââââââââââââââââââââââââ´âââââââââââââââââ´ââââââââââââââââ¯
-====================Trades overview=========================== * Number of
-trades closed: 4 * Number of trades open: 2 * Percentage of positive trades:
-60.0% * Percentage of negative trades: 20.0% * Average trade size: 98.8728 EUR
-* Average trade duration: 183.5 hours
+Trades overview
 â­ââââââââââ¬ââââââââââââââââââââââ¬ââââââââââââââââââââââ¬âââââââââââââââââââââ¬âââââââââââââââ¬âââââââââââââââââââ¬ââââââââââââââââââââââââ¬âââââââââââââââââââââ¬ââââââââââââââââââââââ®
 â Pair â Open date â Close date â Duration (hours) â Size (EUR) â
 Net gain (EUR) â Net gain percentage â Open price (EUR) â Close price
 (EUR) â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â DOT-EUR â 2023-11-30 20:00:00 â â 2976.65 â 107.104 â 0 â
-0.0000% â 5.0215 â â
+â DOT-EUR â 2023-11-30 18:00:00 â â 3207.26 â 107.138 â 0 â
+0.0000% â 5.023 â â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â BTC-EUR â 2023-11-29 14:00:00 â â 3006.65 â 107.095 â 0 â
-0.0000% â 34546.6 â â
+â BTC-EUR â 2023-11-29 12:00:00 â â 3237.26 â 104.372 â 0 â
+0.0000% â 34790.7 â â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â BTC-EUR â 2023-11-08 00:00:00 â 2023-11-14 16:00:00 â 160 â 99.2265
-â 1.3352 â 1.3456% â 33075.5 â 33520.6 â
+â BTC-EUR â 2023-11-07 22:00:00 â 2023-11-14 14:00:00 â 160 â 99.2337
+â 2.5395 â 2.5591% â 33077.9 â 33924.4 â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â BTC-EUR â 2023-11-06 16:00:00 â 2023-11-06 20:00:00 â 4 â 97.8607
-â -0.0026 â -0.0026% â 32620.2 â 32619.4 â
+â BTC-EUR â 2023-11-06 14:00:00 â 2023-11-06 18:00:00 â 4 â 98.2854
+â -0.4248 â -0.4322% â 32761.8 â 32620.2 â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â DOT-EUR â 2023-10-30 06:00:00 â 2023-11-14 00:00:00 â 354 â 100.551
-â 24.8794 â 24.7430% â 4.0375 â 5.0365 â
+â DOT-EUR â 2023-10-30 04:00:00 â 2023-11-14 00:00:00 â 356 â 100.537
+â 24.2886 â 24.1588% â 4.0565 â 5.0365 â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â BTC-EUR â 2023-09-13 16:00:00 â 2023-09-22 16:00:00 â 216 â 97.8529
-â 2.2051 â 2.2534% â 24463.2 â 25014.5 â
+â BTC-EUR â 2023-09-13 14:00:00 â 2023-09-22 14:00:00 â 216 â 97.8976
+â 2.1508 â 2.1970% â 24474.4 â 25012.1 â
 â°ââââââââââ´ââââââââââââââââââââââ´ââââââââââââââââââââââ´âââââââââââââââââââââ´âââââââââââââââ´âââââââââââââââââââ´ââââââââââââââââââââââââ´âââââââââââââââââââââ´ââââââââââââââââââââââ¯
-================================================================== ``` ###
-Backtest experiments The framework also supports backtest experiments. Backtest
-experiments allows you to compare multiple algorithms and evaluate their
-performance. Ideally, you would do this by parameterizing your strategy and
-creating a factory function that creates the algorithm with the different
+``` ### Backtest experiments The framework also supports backtest experiments.
+Backtest experiments allows you to compare multiple algorithms and evaluate
+their performance. Ideally, you would do this by parameterizing your strategy
+and creating a factory function that creates the algorithm with the different
 parameters. You can find an example of this in the [backtest experiments
 example](./examples/backtest_experiment). ## Broker/Exchange configuration The
 framework has by default support for [ccxt](https://github.com/ccxt/ccxt). This
 should allow you to connect to a lot of brokers/exchanges. ```python from
 investing_algorithm_framework import PortfolioConfiguration, \
 MarketCredential, create_app app = create_app() app.add_market_credential
 ( MarketCredential( market="", api_key="", secret_key="", ) )
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/__init__.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/__init__.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from investing_algorithm_framework.app import App, Algorithm, AppHook
-from .create_app import create_app
+from investing_algorithm_framework.app import TradingStrategy, \
+    StatelessAction, Task
 from investing_algorithm_framework.domain import ApiException, \
     TradingDataType, TradingTimeFrame, OrderType, OperationalException, \
     OrderStatus, OrderSide, Config, TimeUnit, TimeInterval, Order, Portfolio, \
     Position, TimeFrame, BACKTESTING_INDEX_DATETIME, MarketCredential, \
     PortfolioConfiguration, RESOURCE_DIRECTORY, pretty_print_backtest, \
     Trade, OHLCVMarketDataSource, OrderBookMarketDataSource, SYMBOLS, \
     TickerMarketDataSource, MarketService, BacktestReportsEvaluation, \
     pretty_print_backtest_reports_evaluation, load_backtest_reports, \
     RESERVED_BALANCES, APP_MODE, AppMode, DATETIME_FORMAT
-from investing_algorithm_framework.app import TradingStrategy, \
-    StatelessAction, Task
 from investing_algorithm_framework.infrastructure import \
     CCXTOrderBookMarketDataSource, CCXTOHLCVMarketDataSource, \
     CCXTTickerMarketDataSource, CSVOHLCVMarketDataSource, \
     CSVTickerMarketDataSource
+from .create_app import create_app
 
 __all__ = [
     "Algorithm",
     "RESOURCE_DIRECTORY",
     "App",
     "AppHook",
     "create_app",
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/algorithm.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/algorithm.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/app.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+import inspect
 import logging
 import os
 import shutil
 import threading
+from abc import abstractmethod
 from datetime import datetime
 from distutils.sysconfig import get_python_lib
 from time import sleep
-from typing import List
-import inspect
+from typing import List, Optional, Tuple
 
-from abc import abstractmethod
 from flask import Flask
 
 from investing_algorithm_framework.app.algorithm import Algorithm
 from investing_algorithm_framework.app.stateless import ActionHandler
 from investing_algorithm_framework.app.task import Task
 from investing_algorithm_framework.app.web import create_flask_app
 from investing_algorithm_framework.domain import DATABASE_NAME, TimeUnit, \
@@ -24,14 +24,17 @@
 from investing_algorithm_framework.infrastructure import setup_sqlalchemy, \
     create_all_tables
 from investing_algorithm_framework.services import OrderBacktestService, \
     BacktestMarketDataSourceService, BacktestPortfolioService, \
     MarketDataSourceService, MarketCredentialService
 
 logger = logging.getLogger("investing_algorithm_framework")
+COLOR_RESET = '\033[0m'
+COLOR_GREEN = '\033[92m'
+COLOR_YELLOW = '\033[93m'
 
 
 class AppHook:
 
     @abstractmethod
     def on_run(self, app, algorithm: Algorithm):
         raise NotImplementedError()
@@ -232,15 +235,16 @@
                 )
             self._create_database_if_not_exists()
 
     def _initialize_app_for_backtest(
         self,
         backtest_start_date,
         backtest_end_date,
-        pending_order_check_interval
+        pending_order_check_interval,
+        market_data_sources,
     ) -> None:
         """
         Initialize the app for backtesting by setting the configuration
         parameters for backtesting and overriding the services with the
         backtest services equivalents. This method should only be called
         before running a backtest or a set of backtests and should be called
         once.
@@ -263,20 +267,14 @@
 
         # Create resource dir if not exits
         self._create_resource_directory_if_not_exists()
 
         # Override the MarketDataSourceService service with the backtest
         # market data source service equivalent. Additionally, convert the
         # market data sources to backtest market data sources
-        # market_data_sources = self.get_market_data_sources()
-        # backtest_market_data_sources = []
-        market_data_source_service: MarketDataSourceService = \
-            self.container.market_data_source_service()
-        market_data_sources = market_data_source_service \
-            .get_market_data_sources()
 
         if market_data_sources is not None:
             backtest_market_data_sources = [
                 market_data_source.to_backtest_market_data_source()
                 for market_data_source in market_data_sources
                 if market_data_source is not None
             ]
@@ -431,18 +429,18 @@
                 self.config.get(RESOURCE_DIRECTORY), "manage.py"
             )
 
             if not os.path.exists(destination):
                 shutil.copy(management_commands_template, destination)
 
     def run(
-            self,
-            payload: dict = None,
-            number_of_iterations: int = None,
-            sync=False
+        self,
+        payload: dict = None,
+        number_of_iterations: int = None,
+        sync=False
     ):
         """
         Entry point to run the application. This method should be called to
         start the algorithm. The method runs the algorithm for the specified
         number of iterations and handles the payload if the app is running in
         stateless mode.
 
@@ -669,20 +667,20 @@
                     "Could not create database directory"
                 )
 
     def get_portfolio_configurations(self):
         return self.algorithm.get_portfolio_configurations()
 
     def run_backtest(
-            self,
-            algorithm,
-            start_date,
-            end_date,
-            pending_order_check_interval='1h',
-            output_directory=None
+        self,
+        algorithm,
+        start_date,
+        end_date,
+        pending_order_check_interval='1h',
+        output_directory=None
     ) -> BacktestReport:
         """
         Run a backtest for an algorithm. This method should be called when
         running a backtest.
 
         :param algorithm: The algorithm to run a backtest for (instance of
         Algorithm)
@@ -695,18 +693,22 @@
         """
         logger.info("Initializing backtest")
         self.algorithm = algorithm
 
         if end_date is None:
             end_date = datetime.utcnow()
 
+        market_data_sources = self._market_data_source_service\
+            .get_market_data_sources()
+
         self._initialize_app_for_backtest(
             backtest_start_date=start_date,
             backtest_end_date=end_date,
-            pending_order_check_interval=pending_order_check_interval
+            pending_order_check_interval=pending_order_check_interval,
+            market_data_sources=market_data_sources
         )
 
         self._initialize_algorithm_for_backtest(
             algorithm=self.algorithm
         )
         backtest_service = self.container.backtest_service()
         backtest_service.resource_directory = self.config.get(
@@ -729,70 +731,95 @@
         backtest_report_writer_service.write_report_to_csv(
             report=report, output_directory=output_directory
         )
 
         return report
 
     def run_backtests(
-            self,
-            algorithms,
-            start_date,
-            end_date,
-            pending_order_check_interval='1h',
-            output_directory=None
+        self,
+        algorithms,
+        start_date: Optional[datetime] = None,
+        end_date: Optional[datetime] = None,
+        date_ranges: Optional[Tuple[datetime, datetime]] = None,
+        pending_order_check_interval='1h',
+        output_directory=None
     ) -> List[BacktestReport]:
         """
         Run a backtest for a set algorithm. This method should be called when
         running a backtest.
 
         :param algorithms: The algorithms to run backtests for (list of
         Algorithm instances)
         :param start_date: The start date of the backtest
         :param end_date: The end date of the backtest
         :param pending_order_check_interval: The interval at which to check
+        :param date_ranges: The date ranges to run the backtests for (list of
+        tuples of start and end dates)
         pending orders
         :param output_directory: The directory to write the backtest report to
         :return: List of BacktestReport intances
         """
         logger.info("Initializing backtests")
         reports = []
 
-        if end_date is None:
-            end_date = datetime.utcnow()
+        if start_date is not None:
 
-        self._initialize_app_for_backtest(
-            backtest_start_date=start_date,
-            backtest_end_date=end_date,
-            pending_order_check_interval=pending_order_check_interval
-        )
+            if end_date is None:
+                end_date = datetime.utcnow()
 
-        for algorithm in algorithms:
-            self._initialize_algorithm_for_backtest(algorithm)
-            backtest_service = self.container.backtest_service()
-            backtest_service.resource_directory = self.config.get(
-                RESOURCE_DIRECTORY
-            )
+            date_ranges = [(start_date, end_date)]
+        else:
+            if date_ranges is None:
+                raise OperationalException("No date ranges specified")
 
-            # Run the backtest with the backtest_service and collect the report
-            report = backtest_service.run_backtest(
-                algorithm=algorithm, start_date=start_date, end_date=end_date
-            )
-            backtest_report_writer_service = self.container \
-                .backtest_report_writer_service()
+        market_data_sources = self._market_data_source_service\
+            .get_market_data_sources()
 
-            if output_directory is None:
-                output_directory = os.path.join(
-                    self.config.get(RESOURCE_DIRECTORY),
-                    "backtest_reports"
+        for date_range in date_ranges:
+            start_date, end_date = date_range
+            self._initialize_app_for_backtest(
+                backtest_start_date=start_date,
+                backtest_end_date=end_date,
+                pending_order_check_interval=pending_order_check_interval,
+                market_data_sources=market_data_sources
+            )
+
+            print(
+                f"{COLOR_YELLOW}Running backtests for date "
+                f"range:{COLOR_RESET} {COLOR_GREEN}{start_date} - "
+                f"{end_date} for a "
+                f"total of {len(algorithms)} algorithms.{COLOR_RESET}"
+            )
+            for algorithm in algorithms:
+                self._initialize_algorithm_for_backtest(algorithm)
+                backtest_service = self.container.backtest_service()
+                backtest_service.resource_directory = self.config.get(
+                    RESOURCE_DIRECTORY
                 )
 
-            backtest_report_writer_service.write_report_to_csv(
-                report=report, output_directory=output_directory
-            )
-            reports.append(report)
+                # Run the backtest with the backtest_service
+                # and collect the report
+                report = backtest_service.run_backtest(
+                    algorithm=algorithm,
+                    start_date=start_date,
+                    end_date=end_date
+                )
+                backtest_report_writer_service = self.container \
+                    .backtest_report_writer_service()
+
+                if output_directory is None:
+                    output_directory = os.path.join(
+                        self.config.get(RESOURCE_DIRECTORY),
+                        "backtest_reports"
+                    )
+
+                backtest_report_writer_service.write_report_to_csv(
+                    report=report, output_directory=output_directory
+                )
+                reports.append(report)
 
         return reports
 
     def add_market_data_source(self, market_data_source):
         market_data_source.config = self.config
         self._market_data_source_service.add(market_data_source)
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/stateless/__init__.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/stateless/action_handlers/__init__.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/stateless/exception_handler.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/exception_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/strategy.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/strategy.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from investing_algorithm_framework.domain import OperationalException
 from investing_algorithm_framework.domain import \
     TimeUnit, StrategyProfile, Trade
 from .algorithm import Algorithm
-from investing_algorithm_framework.domain import OperationalException
 
 
 class TradingStrategy:
     time_unit: str = None
     interval: int = None
     worker_id: str = None
     strategy_id: str = None
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/task.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/task.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/controllers/__init__.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from investing_algorithm_framework.app.web.controllers.portfolio \
-    import blueprint as portfolio_blueprint
 from investing_algorithm_framework.app.web.controllers.orders import \
     blueprint as orders_blueprint
+from investing_algorithm_framework.app.web.controllers.portfolio \
+    import blueprint as portfolio_blueprint
 from investing_algorithm_framework.app.web.controllers.positions import \
     blueprint as positions_blueprint
 
 
 def setup_blueprints(flask_app):
     flask_app.register_blueprint(portfolio_blueprint, prefix="/api")
     flask_app.register_blueprint(orders_blueprint, prefix="/api")
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/controllers/orders.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/orders.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 
-from flask import Blueprint, request
 from dependency_injector.wiring import inject, Provide
-from investing_algorithm_framework.app.web.schemas import OrderSerializer
+from flask import Blueprint, request
+
 from investing_algorithm_framework.app.web.responses import create_response
+from investing_algorithm_framework.app.web.schemas import OrderSerializer
 from investing_algorithm_framework.dependency_container import \
     DependencyContainer
 
 logger = logging.getLogger("investing_algorithm_framework")
 
 blueprint = Blueprint("order-views", __name__)
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/controllers/portfolio.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/controllers/positions.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/positions.py`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import logging
 
-from flask import Blueprint, request
 from dependency_injector.wiring import inject, Provide
+from flask import Blueprint, request
 
-from investing_algorithm_framework.app.web.schemas import PositionSerializer
 from investing_algorithm_framework.app.web.responses import create_response
+from investing_algorithm_framework.app.web.schemas import PositionSerializer
 
 logger = logging.getLogger("investing_algorithm_framework")
 
 blueprint = Blueprint("position-views", __name__)
 
 
 @blueprint.route("/api/positions", methods=["GET"])
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/error_handler.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/error_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/responses.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/responses.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/app/web/schemas/portfolio.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/schemas/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/create_app.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/create_app.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/dependency_container.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/dependency_container.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/__init__.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 from .config import Config, Environment
-from .models import OrderStatus, OrderSide, OrderType, TimeInterval, \
-    TimeUnit, TimeFrame, TradingTimeFrame, TradingDataType, \
-    PortfolioConfiguration, Portfolio, Position, Order, TradeStatus, \
-    OrderFee, BacktestReport, PortfolioSnapshot, StrategyProfile, \
-    BacktestPosition, Trade, MarketCredential, PositionSnapshot, \
-    BacktestReportsEvaluation, AppMode
-from .exceptions import OperationalException, ApiException, \
-    PermissionDeniedApiException, ImproperlyConfigured
 from .constants import ITEMIZE, ITEMIZED, PER_PAGE, PAGE, ENVIRONMENT, \
     DATABASE_DIRECTORY_PATH, DATABASE_NAME, DEFAULT_PER_PAGE_VALUE, \
     DEFAULT_PAGE_VALUE, SQLALCHEMY_DATABASE_URI, RESOURCE_DIRECTORY, \
     DATETIME_FORMAT, DATETIME_FORMAT_BACKTESTING, BACKTESTING_FLAG, \
     BACKTESTING_INDEX_DATETIME, BACKTESTING_START_DATE, CCXT_DATETIME_FORMAT, \
     BACKTEST_DATA_DIRECTORY_NAME, TICKER_DATA_TYPE, OHLCV_DATA_TYPE, \
-    CURRENT_UTC_DATETIME, BACKTESTING_END_DATE,  SYMBOLS, \
+    CURRENT_UTC_DATETIME, BACKTESTING_END_DATE, SYMBOLS, \
     CCXT_DATETIME_FORMAT_WITH_TIMEZONE, RESERVED_BALANCES, \
     BACKTESTING_PENDING_ORDER_CHECK_INTERVAL, APP_MODE
-from .singleton import Singleton
-from .utils import random_string, append_dict_as_row_to_csv, \
-    add_column_headers_to_csv, get_total_amount_of_rows, \
-    csv_to_list, StoppableThread, pretty_print_backtest_reports_evaluation, \
-    pretty_print_backtest, load_csv_into_dict, load_backtest_reports
-from .strategy import Strategy
-from .stateless_actions import StatelessActions
+from .data_structures import PeekableQueue
 from .decimal_parsing import parse_decimal_to_string, parse_string_to_decimal
+from .exceptions import OperationalException, ApiException, \
+    PermissionDeniedApiException, ImproperlyConfigured
+from .models import OrderStatus, OrderSide, OrderType, TimeInterval, \
+    TimeUnit, TimeFrame, TradingTimeFrame, TradingDataType, \
+    PortfolioConfiguration, Portfolio, Position, Order, TradeStatus, \
+    OrderFee, BacktestReport, PortfolioSnapshot, StrategyProfile, \
+    BacktestPosition, Trade, MarketCredential, PositionSnapshot, \
+    BacktestReportsEvaluation, AppMode
 from .services import TickerMarketDataSource, OrderBookMarketDataSource, \
     OHLCVMarketDataSource, BacktestMarketDataSource, MarketDataSource, \
     MarketService, MarketCredentialService, AbstractPortfolioSyncService, \
     RoundingService
-from .data_structures import PeekableQueue
+from .singleton import Singleton
+from .stateless_actions import StatelessActions
+from .strategy import Strategy
+from .utils import random_string, append_dict_as_row_to_csv, \
+    add_column_headers_to_csv, get_total_amount_of_rows, \
+    csv_to_list, StoppableThread, pretty_print_backtest_reports_evaluation, \
+    pretty_print_backtest, load_csv_into_dict, load_backtest_reports
 
 __all__ = [
     'Config',
     "OrderStatus",
     "OrderSide",
     "OrderType",
     "OperationalException",
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/config.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/config.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/constants.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/constants.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/data_structures.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/data_structures.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/decimal_parsing.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/decimal_parsing.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/exceptions.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/__init__.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/__init__.py`

 * *Ordering differences only*

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
+from .app_mode import AppMode
+from .backtesting import BacktestReport, BacktestPosition, \
+    BacktestReportsEvaluation
+from .market import MarketCredential
 from .order import OrderStatus, OrderSide, OrderType, Order, OrderFee
+from .portfolio import PortfolioConfiguration, Portfolio, PortfolioSnapshot
+from .position import Position, PositionSnapshot
+from .strategy_profile import StrategyProfile
 from .time_frame import TimeFrame
 from .time_interval import TimeInterval
 from .time_unit import TimeUnit
-from .market import MarketCredential
+from .trade import Trade, TradeStatus
 from .trading_data_types import TradingDataType
 from .trading_time_frame import TradingTimeFrame
-from .portfolio import PortfolioConfiguration, Portfolio, PortfolioSnapshot
-from .position import Position, PositionSnapshot
-from .backtesting import BacktestReport, BacktestPosition, \
-    BacktestReportsEvaluation
-from .strategy_profile import StrategyProfile
-from .trade import Trade, TradeStatus
-from .app_mode import AppMode
 
 __all__ = [
     "OrderStatus",
     "OrderSide",
     "OrderType",
     "Order",
     "TimeFrame",
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/app_mode.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/app_mode.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/backtesting/backtest_position.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/backtesting/backtest_position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/backtesting/backtest_report.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/backtesting/backtest_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+
 from investing_algorithm_framework.domain.models.base_model import BaseModel
 from investing_algorithm_framework.domain.models.time_unit import TimeUnit
 
 
 class BacktestReport(BaseModel):
 
     def __init__(
@@ -209,23 +210,23 @@
 
     @market_data_file.setter
     def market_data_file(self, value):
         self._market_data_file = value
 
     @property
     def percentage_positive_trades(self):
-        return self._percentage_positive_trades
+        return float(self._percentage_positive_trades)
 
     @percentage_positive_trades.setter
     def percentage_positive_trades(self, value):
         self._percentage_positive_trades = value
 
     @property
     def percentage_negative_trades(self):
-        return self._percentage_negative_trades
+        return float(self._percentage_negative_trades)
 
     @percentage_negative_trades.setter
     def percentage_negative_trades(self, value):
         self._percentage_negative_trades = value
 
     @property
     def number_of_trades_closed(self):
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/base_model.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/base_model.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/market/market_credential.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/market/market_credential.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/order/order.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 import logging
 
 from dateutil.parser import parse
 
 from investing_algorithm_framework.domain.exceptions import \
     OperationalException
 from investing_algorithm_framework.domain.models.base_model import BaseModel
-from investing_algorithm_framework.domain.models.order import OrderStatus, \
-    OrderType, OrderSide
+from investing_algorithm_framework.domain.models.order.order_status import \
+    OrderStatus
+from investing_algorithm_framework.domain.models.order.order_type import \
+    OrderType
+from investing_algorithm_framework.domain.models.order.order_side import \
+    OrderSide
 from investing_algorithm_framework.domain.models.order.order_fee import \
     OrderFee
 
 logger = logging.getLogger("investing_algorithm_framework")
 
 
 class Order(BaseModel):
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/order/order_fee.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_fee.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/order/order_side.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_side.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/order/order_status.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_status.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/order/order_type.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_type.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/portfolio/portfolio.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/position/position.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/position/position_snapshot.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/position/position_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/strategy_profile.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/strategy_profile.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/time_frame.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/time_interval.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/time_interval.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/time_unit.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/time_unit.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/trade/trade.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trade/trade.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
+from datetime import datetime
 from typing import List
-from polars import DataFrame
+
 import polars as pl
-from datetime import datetime
-from investing_algorithm_framework.domain.models.base_model import BaseModel
+from polars import DataFrame
+
+from investing_algorithm_framework.domain.constants import DATETIME_FORMAT
 from investing_algorithm_framework.domain.exceptions import \
     OperationalException
-from investing_algorithm_framework.domain.constants import DATETIME_FORMAT
+from investing_algorithm_framework.domain.models.base_model import BaseModel
 
 
 class Trade(BaseModel):
     """
     Trade model
 
     A trade is a combination of a buy and sell order that has been opened or
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/trade/trade_status.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trade/trade_status.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/trading_data_types.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trading_data_types.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/models/trading_time_frame.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trading_time_frame.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from enum import Enum
 from datetime import timedelta, datetime
+from enum import Enum
 
 from investing_algorithm_framework.domain.exceptions import \
     OperationalException
 
 
 class TradingTimeFrame(Enum):
     ONE_MINUTE = "ONE_MINUTE"
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/services/__init__.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
+from .market_credential_service import MarketCredentialService
 from .market_data_sources import MarketDataSource, TickerMarketDataSource, \
     OHLCVMarketDataSource, OrderBookMarketDataSource, BacktestMarketDataSource
 from .market_service import MarketService
-from .market_credential_service import MarketCredentialService
 from .portfolios import AbstractPortfolioSyncService
 from .rounding_service import RoundingService
 
 __all__ = [
     "MarketDataSource",
     "TickerMarketDataSource",
     "OHLCVMarketDataSource",
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/services/market_credential_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/market_credential_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/services/market_data_sources.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/market_data_sources.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
+import csv
 import logging
 import os
-import csv
 from abc import abstractmethod, ABC
 from datetime import datetime, timedelta
 from typing import Callable
 
 import polars
 
 from investing_algorithm_framework.domain import TimeFrame, \
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/services/market_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/market_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import logging
-from typing import Dict
 from abc import ABC, abstractmethod
 from datetime import datetime
+from typing import Dict
+
 from polars import DataFrame
+
 logger = logging.getLogger("investing_algorithm_framework")
 
 
 class MarketService(ABC):
 
     def __init__(self, market_credential_service):
         self._market_credential_service = market_credential_service
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/services/rounding_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/rounding_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/strategy.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/utils/__init__.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/__init__.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+from .backtesting import pretty_print_backtest, \
+    pretty_print_backtest_reports_evaluation, load_backtest_reports
+from .csv import get_total_amount_of_rows, append_dict_as_row_to_csv, \
+    add_column_headers_to_csv, csv_to_list, load_csv_into_dict
 from .random import random_string
 from .stoppable_thread import StoppableThread
 from .synchronized import synchronized
-from .csv import get_total_amount_of_rows, append_dict_as_row_to_csv, \
-    add_column_headers_to_csv, csv_to_list, load_csv_into_dict
-from .backtesting import pretty_print_backtest, \
-    pretty_print_backtest_reports_evaluation, load_backtest_reports
 
 __all__ = [
     'synchronized',
     'StoppableThread',
     'random_string',
     'get_total_amount_of_rows',
     'append_dict_as_row_to_csv',
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/utils/csv.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/csv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/domain/utils/stoppable_thread.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/__init__.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from .repositories import SQLOrderRepository, SQLPositionRepository, \
-    SQLPortfolioRepository, SQLOrderFeeRepository, \
-    SQLPortfolioSnapshotRepository, SQLPositionSnapshotRepository
-from .services import PerformanceService, CCXTMarketService
 from .database import setup_sqlalchemy, Session, \
     create_all_tables
 from .models import SQLPortfolio, SQLOrder, SQLPosition, SQLOrderFee, \
     SQLPortfolioSnapshot, SQLPositionSnapshot, \
     CCXTOHLCVBacktestMarketDataSource, CCXTOrderBookMarketDataSource, \
     CCXTTickerMarketDataSource, CCXTOHLCVMarketDataSource, \
     CSVOHLCVMarketDataSource, CSVTickerMarketDataSource
+from .repositories import SQLOrderRepository, SQLPositionRepository, \
+    SQLPortfolioRepository, SQLOrderFeeRepository, \
+    SQLPortfolioSnapshotRepository, SQLPositionSnapshotRepository
+from .services import PerformanceService, CCXTMarketService
 
 __all__ = [
     "create_all_tables",
     "SQLPositionRepository",
     "SQLPortfolioRepository",
     "SQLOrderRepository",
     "SQLOrderFeeRepository",
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/database/sql_alchemy.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/__init__.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/__init__.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from .order import SQLOrder, SQLOrderFee
-from .portfolio import SQLPortfolio, SQLPortfolioSnapshot
-from .position import SQLPosition, SQLPositionSnapshot
 from .market_data_sources import CCXTOrderBookMarketDataSource, \
     CCXTTickerMarketDataSource, CCXTOHLCVMarketDataSource, \
     CCXTOHLCVBacktestMarketDataSource, CSVOHLCVMarketDataSource, \
     CSVTickerMarketDataSource
+from .order import SQLOrder, SQLOrderFee
+from .portfolio import SQLPortfolio, SQLPortfolioSnapshot
+from .position import SQLPosition, SQLPositionSnapshot
 
 __all__ = [
     "SQLOrder",
     "SQLPosition",
     "SQLPortfolio",
     "SQLOrderFee",
     "SQLPositionSnapshot",
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py`

 * *Files 2% similar despite different names*

```diff
@@ -361,42 +361,42 @@
         if "backtest_index_date" not in kwargs:
             raise OperationalException(
                 "backtest_index_date should be passed as a parameter "
                 "for CCXTTickerBacktestMarketDataSource"
             )
 
         file_path = self._create_file_path()
-        timeframe_minutes = TimeFrame.from_string(self.timeframe)\
-            .amount_of_minutes
         backtest_index_date = kwargs["backtest_index_date"]
-        end_date = backtest_index_date + timedelta(minutes=timeframe_minutes)
 
         # Filter the data based on the backtest index date and the end date
         df = polars.read_csv(file_path)
-        df = df.filter(
+        filtered_df = df.filter(
             (df['Datetime'] >= backtest_index_date.strftime(DATETIME_FORMAT))
         )
-        first_row = df.head(1)[0]
-        first_row_datetime = parser.parse(first_row["Datetime"][0])
 
-        if first_row_datetime > end_date:
-            logger.warning(
-                f"No ticker data available for the given backtest "
-                f"index date {backtest_index_date} and symbol {self.symbol} "
-                f"and market {self.market}"
+        # If nothing is found, get all dates before the index date
+        if len(filtered_df) == 0:
+            filtered_df = df.filter(
+                (df['Datetime'] <= backtest_index_date.strftime(
+                    DATETIME_FORMAT))
             )
+            first_row = filtered_df.tail(1)[0]
+        else:
+            first_row = filtered_df.head(1)[0]
+
+        first_row_datetime = parser.parse(first_row["Datetime"][0])
 
         # Calculate the bid and ask price based on the high and low price
         return {
             "symbol": self.symbol,
             "bid": float((first_row["Low"][0])
                          + float(first_row["High"][0]))/2,
             "ask": float((first_row["Low"][0])
                          + float(first_row["High"][0]))/2,
-            "datetime": first_row["Datetime"][0],
+            "datetime": first_row_datetime,
         }
 
     def write_data_to_file_path(self, data_file, data: polars.DataFrame):
         data.write_csv(data_file)
 
 
 class CCXTOHLCVMarketDataSource(OHLCVMarketDataSource):
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from datetime import datetime
-import polars
 import logging
+from datetime import datetime
 
+import polars
 from dateutil.parser import parse
 
 from investing_algorithm_framework.domain import OHLCVMarketDataSource, \
     BacktestMarketDataSource, OperationalException, TickerMarketDataSource, \
     DATETIME_FORMAT
 
 logger = logging.getLogger(__name__)
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/order/order.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/order/order.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/order/order_fee.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/order/order_fee.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/position/position.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/repositories/__init__.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from .order_repository import SQLOrderRepository
 from .order_fee_repository import SQLOrderFeeRepository
-from .position_repository import SQLPositionRepository
-from .position_snapshot_repository import SQLPositionSnapshotRepository
+from .order_repository import SQLOrderRepository
 from .portfolio_repository import SQLPortfolioRepository
 from .portfolio_snapshot_repository import SQLPortfolioSnapshotRepository
+from .position_repository import SQLPositionRepository
+from .position_snapshot_repository import SQLPositionSnapshotRepository
 
 __all__ = [
     "SQLOrderFeeRepository",
     "SQLOrderRepository",
     "SQLPositionRepository",
     "SQLPositionSnapshotRepository",
     "SQLPortfolioRepository",
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/repositories/order_repository.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
-from .repository import Repository
-
-from investing_algorithm_framework.infrastructure.models import SQLOrder, \
-    SQLPosition, SQLPortfolio
 from investing_algorithm_framework.domain import OrderStatus, OrderType, \
     OrderSide
+from investing_algorithm_framework.infrastructure.models import SQLOrder, \
+    SQLPosition, SQLPortfolio
+from .repository import Repository
 
 
 class SQLOrderRepository(Repository):
     base_class = SQLOrder
 
     def _apply_query_params(self, db, query, query_params):
         external_id_query_param = self.get_query_param(
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/repositories/position_repository.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/repositories/repository.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+
 from investing_algorithm_framework.domain import OrderStatus, OrderSide
 
 logger = logging.getLogger(__name__)
 
 
 class PerformanceService:
     """
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/__init__.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-import os
 import csv
+import os
 
 from investing_algorithm_framework.domain import BacktestReport, \
-    DATETIME_FORMAT
+    DATETIME_FORMAT_BACKTESTING
 
 
 class BacktestReportWriterService:
     """
     Service to write backtest reports to a file.
 
     Service supports writing backtest reports to the following formats:
@@ -17,19 +17,24 @@
     ) -> str:
         """
         Write a backtest report to a CSV file.
         """
 
         if not os.path.exists(output_directory):
             os.makedirs(output_directory)
-
+        backtest_start_date = report.backtest_start_date\
+            .strftime(DATETIME_FORMAT_BACKTESTING)
+        backtest_end_date = report.backtest_end_date\
+            .strftime(DATETIME_FORMAT_BACKTESTING)
+        created_at = report.created_at.strftime(DATETIME_FORMAT_BACKTESTING)
         csv_file_path = os.path.join(
             output_directory,
-            f"report_{report.name}"
-            f"_{report.created_at.strftime(DATETIME_FORMAT)}.csv"
+            f"report_{report.name}_backtest_start_date_"
+            f"{backtest_start_date}_backtest_end_date_"
+            f"{backtest_end_date}_created_at_{created_at}.csv"
         )
         report_dict = report.to_dict()
 
         with open(csv_file_path, 'w', newline='') as csv_file:
             writer = csv.DictWriter(csv_file, fieldnames=report_dict.keys())
             writer.writeheader()
             writer.writerow(report_dict)
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/backtesting/backtest_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/backtesting/backtest_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import datetime, timedelta
-from dateutil import parser
+
 import pandas as pd
+from dateutil import parser
 from tqdm import tqdm
 
 from investing_algorithm_framework.domain import BacktestReport, \
     BACKTESTING_INDEX_DATETIME, TimeUnit, BacktestPosition, \
     TradingDataType, OrderStatus, OperationalException, MarketDataSource, \
     OrderSide
 from investing_algorithm_framework.services.market_data_source_service import \
@@ -88,15 +89,15 @@
             start_date=start_date,
             end_date=end_date
         )
 
         for index, row in tqdm(
             schedule.iterrows(),
             total=len(schedule),
-            desc=f"Running backtests {algorithm.name}",
+            desc=f"Running backtest for algorithm with name {algorithm.name}",
             colour="GREEN"
         ):
             strategy_profile = self.get_strategy_from_strategy_profiles(
                 strategy_profiles, row['id']
             )
             index_date = parser.parse(str(index))
             self.run_backtest_for_profile(
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/configuration_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/configuration_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/market_credential_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/market_credential_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Union, List
+
 from investing_algorithm_framework.domain import MarketCredential
 
 
 class MarketCredentialService:
     _market_credentials = {}
 
     def add(self, market_data_credential: MarketCredential):
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import List
+
 from tqdm import tqdm
 
 from investing_algorithm_framework.domain import MarketService, \
     BacktestMarketDataSource, BACKTESTING_END_DATE, BACKTESTING_START_DATE, \
     BACKTESTING_INDEX_DATETIME, OperationalException
 from investing_algorithm_framework.services.configuration_service import \
     ConfigurationService
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -81,15 +81,15 @@
             time_frame=time_frame,
             from_timestamp=from_timestamp,
             market=market,
             to_timestamp=to_timestamp
         )
 
     def get_data(self, identifier):
-
+        print(self._market_data_sources)
         for market_data_source in self._market_data_sources:
             if market_data_source.get_identifier() == identifier:
                 return market_data_source.get_data(
                     market_credential_service=self._market_credential_service
                 )
 
     def get_ticker_market_data_source(self, symbol, market=None):
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/order_service/order_backtest_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/order_service/order_backtest_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/order_service/order_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/order_service/order_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import logging
 from datetime import datetime
-from dateutil.tz import tzutc
 from queue import PriorityQueue
 
+from dateutil.tz import tzutc
+
 from investing_algorithm_framework.domain import OrderType, OrderSide, \
     OperationalException, OrderStatus, MarketService, Order
 from investing_algorithm_framework.services.repository_service \
     import RepositoryService
 
 logger = logging.getLogger("investing_algorithm_framework")
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/portfolios/portfolio_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import logging
+
 from investing_algorithm_framework.domain import OperationalException, \
     AbstractPortfolioSyncService, RESERVED_BALANCES, APP_MODE, SYMBOLS, \
     OrderSide, AppMode
 from investing_algorithm_framework.services.trade_service import TradeService
 
 logger = logging.getLogger(__name__)
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/position_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/position_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/position_snapshot_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/position_snapshot_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/repository_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/repository_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/strategy_orchestrator_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/strategy_orchestrator_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import logging
-import schedule
 from datetime import datetime
+
+import schedule
+
 from investing_algorithm_framework.domain import StoppableThread, TimeUnit, \
     OperationalException, MarketDataSource
 from investing_algorithm_framework.services.market_data_source_service \
     import MarketDataSourceService
 
 logger = logging.getLogger("investing_algorithm_framework")
```

### Comparing `investing_algorithm_framework-3.4.3/investing_algorithm_framework/services/trade_service/trade_service.py` & `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/trade_service/trade_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.4.3/pyproject.toml` & `investing_algorithm_framework-3.5.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "investing-algorithm-framework"
-version = "v3.4.3"
+version = "v3.5.0"
 description = "A framework for creating trading bots"
 authors = ["MDUYN"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 wrapt = "^1.16.0"
```

### Comparing `investing_algorithm_framework-3.4.3/PKG-INFO` & `investing_algorithm_framework-3.5.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investing-algorithm-framework
-Version: 3.4.3
+Version: 3.5.0
 Summary: A framework for creating trading bots
 Author: MDUYN
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -162,60 +162,74 @@
 
 ### Backtesting report
 You can use the ```pretty_print_backtest``` function to print a backtest report.
 For example if you run the [moving average example trading bot](./examples/crossover_moving_average_trading_bot)
 you will get the following backtesting report:
  
 ```bash
-====================Backtest report===============================
-* Start date: 2023-08-24 00:00:00
-* End date: 2023-12-02 00:00:00
-* Number of days: 100
-* Number of runs: 1201
-====================Portfolio overview============================
-* Number of orders: 10
-* Initial balance: 400.0000 EUR
-* Final balance: 431.8837 EUR
-* Total net gain: 28.4171 EUR
-* Total net gain percentage: 7.1043%
-* Growth rate: 7.9709%
-* Growth 31.8837 EUR
-====================Positions overview========================
+
+                          /&#                                      #&(                 Backtest report
+                          &&&&&&&&&&&#                       &&&&&&&&&&&&              ---------------------------
+                         &&&&&&&&&&&&&&&&                (&&&&&&&&&&&&&&&              Start date: 2023-08-24 00:00:00
+                         &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&              End date: 2023-12-02 00:00:00
+                         &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&              Number of days: 100 
+                          &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&              Number of runs: 1201
+                          .&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&               Number of orders: 10
+                           &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&.               Initial balance: 400.0
+                          &&&&&&&#  /(((   &&&&&&&&&&&&*(((     .&&&&&&&.              Final balance: 431.1499      
+              &&&&&&&&&&&&&&&&&&&    ((((    &&&&&&&&   ((((     &&&&&&&&&&&&&&&&&&&   Total net gain: 28.5542 7.139%  
+                       (((&&&&&&&&    ((((    &&&&&&     ((((   &&&&&&&&&((            Growth: 31.1499 7.787%             
+               /((((((((((&&&&&&&&&&   (((,   &&&&&&      (((**&&&&&&&&&(((((((((((    Number of trades closed: 4
+                     &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&          Number of trades open(end of backtest): 2
+                            &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&                 Percentage positive trades: 60.0%
+                              &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&                   Percentage negative trades: 20.0%
+                     (((((      &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&(                      Average trade size: 98.9886 EUR
+                    (((((           &&&&&&&&&&&&&&&&&&&&&&&&,                          Average trade duration: 184.0 hours
+                   (((((                 &&&&&&&&&&&&&#                            
+                  (((((                  #&&&&&&&&&&###                            
+                 (((((                   &&&&&&&&&&&###.                           
+               .(((((                   &&&&&&&&&&&&&&###(                          
+              (((((                   &&&&&&&&&&&&&&&&#(((/                        
+             (((((                  &&&&&&&&&&&&&&&&&&&@((((                       
+            (((((                  &&&&&&&&&&&&&&&&&&&&&&((((                      
+           (((((                  &&&&&&&&&&&&&&&&&&&&&&&&((((,                    
+         .(((((                   &&&&&&&&&&&&&&&&&&&&&&&&&&((((                    
+        (((((                   &&&&&&&&&&&&&&&&&&&&&&&&&&&&((((                   
+       (((((                    &&&&&&&&&&&&&&&&&&&&&&&&&&&&&((((                  
+      (((((                    &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&((((                  
+     (((((                     &&&&&&&&&&&&&&&&&&&&&&&&&&&&&#((((                  
+     (((((((((((((((((((#########&&&&&&&&&&&&&&&&&&&&&&&&&&&&(((((                  
+      (((((((((((((((((((((######&&&&&&&&&&&&&&&&&&&&&&&&&&&&((((                   
+        
+Positions overview
 ╭────────────┬──────────┬──────────────────────┬───────────────────────┬──────────────┬───────────────┬───────────────────────────┬────────────────┬───────────────╮
 │ Position   │   Amount │   Pending buy amount │   Pending sell amount │   Cost (EUR) │   Value (EUR) │ Percentage of portfolio   │   Growth (EUR) │ Growth_rate   │
 ├────────────┼──────────┼──────────────────────┼───────────────────────┼──────────────┼───────────────┼───────────────────────────┼────────────────┼───────────────┤
-│ EUR        │ 214.219  │                    0 │                     0 │      214.219 │       214.219 │ 49.6010%                  │         0      │ 0.0000%       │
+│ EUR        │ 217.044  │                    0 │                     0 │      217.044 │       217.044 │ 50.3407%                  │         0      │ 0.0000%       │
 ├────────────┼──────────┼──────────────────────┼───────────────────────┼──────────────┼───────────────┼───────────────────────────┼────────────────┼───────────────┤
-│ BTC        │   0.0031 │                    0 │                     0 │      107.095 │       110.401 │ 25.5627%                  │         3.3066 │ 3.0875%       │
+│ BTC        │   0.003  │                    0 │                     0 │      104.372 │       106.84  │ 24.7802%                  │         2.4678 │ 2.3644%       │
 ├────────────┼──────────┼──────────────────────┼───────────────────────┼──────────────┼───────────────┼───────────────────────────┼────────────────┼───────────────┤
-│ DOT        │  21.3291 │                    0 │                     0 │      107.104 │       107.264 │ 24.8363%                  │         0.16   │ 0.1494%       │
+│ DOT        │  21.3295 │                    0 │                     0 │      107.138 │       107.266 │ 24.8791%                  │         0.128  │ 0.1195%       │
 ╰────────────┴──────────┴──────────────────────┴───────────────────────┴──────────────┴───────────────┴───────────────────────────┴────────────────┴───────────────╯
-====================Trades overview===========================
-* Number of trades closed: 4
-* Number of trades open: 2
-* Percentage of positive trades: 60.0%
-* Percentage of negative trades: 20.0%
-* Average trade size: 98.8728 EUR
-* Average trade duration: 183.5 hours
+Trades overview
 ╭─────────┬─────────────────────┬─────────────────────┬────────────────────┬──────────────┬──────────────────┬───────────────────────┬────────────────────┬─────────────────────╮
 │ Pair    │ Open date           │ Close date          │   Duration (hours) │   Size (EUR) │   Net gain (EUR) │ Net gain percentage   │   Open price (EUR) │   Close price (EUR) │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ DOT-EUR │ 2023-11-30 20:00:00 │                     │            2976.65 │     107.104  │           0      │ 0.0000%               │             5.0215 │                     │
+│ DOT-EUR │ 2023-11-30 18:00:00 │                     │            3207.26 │     107.138  │           0      │ 0.0000%               │             5.023  │                     │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-11-29 14:00:00 │                     │            3006.65 │     107.095  │           0      │ 0.0000%               │         34546.6    │                     │
+│ BTC-EUR │ 2023-11-29 12:00:00 │                     │            3237.26 │     104.372  │           0      │ 0.0000%               │         34790.7    │                     │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-11-08 00:00:00 │ 2023-11-14 16:00:00 │             160    │      99.2265 │           1.3352 │ 1.3456%               │         33075.5    │          33520.6    │
+│ BTC-EUR │ 2023-11-07 22:00:00 │ 2023-11-14 14:00:00 │             160    │      99.2337 │           2.5395 │ 2.5591%               │         33077.9    │          33924.4    │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-11-06 16:00:00 │ 2023-11-06 20:00:00 │               4    │      97.8607 │          -0.0026 │ -0.0026%              │         32620.2    │          32619.4    │
+│ BTC-EUR │ 2023-11-06 14:00:00 │ 2023-11-06 18:00:00 │               4    │      98.2854 │          -0.4248 │ -0.4322%              │         32761.8    │          32620.2    │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ DOT-EUR │ 2023-10-30 06:00:00 │ 2023-11-14 00:00:00 │             354    │     100.551  │          24.8794 │ 24.7430%              │             4.0375 │              5.0365 │
+│ DOT-EUR │ 2023-10-30 04:00:00 │ 2023-11-14 00:00:00 │             356    │     100.537  │          24.2886 │ 24.1588%              │             4.0565 │              5.0365 │
 ├─────────┼─────────────────────┼─────────────────────┼────────────────────┼──────────────┼──────────────────┼───────────────────────┼────────────────────┼─────────────────────┤
-│ BTC-EUR │ 2023-09-13 16:00:00 │ 2023-09-22 16:00:00 │             216    │      97.8529 │           2.2051 │ 2.2534%               │         24463.2    │          25014.5    │
+│ BTC-EUR │ 2023-09-13 14:00:00 │ 2023-09-22 14:00:00 │             216    │      97.8976 │           2.1508 │ 2.1970%               │         24474.4    │          25012.1    │
 ╰─────────┴─────────────────────┴─────────────────────┴────────────────────┴──────────────┴──────────────────┴───────────────────────┴────────────────────┴─────────────────────╯
-==================================================================
 ```
 
 ### Backtest experiments
 The framework also supports backtest experiments. Backtest experiments allows you to 
 compare multiple algorithms and evaluate their performance. Ideally, 
 you would do this by parameterizing your strategy and creating a factory function that
 creates the algorithm with the different parameters. You can find an example of this
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: investing-algorithm-framework Version: 3.4.3
+Metadata-Version: 2.1 Name: investing-algorithm-framework Version: 3.5.0
 Summary: A framework for creating trading bots Author: MDUYN Requires-Python:
 >=3.8.1,<4.0.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: Flask (>=2.3.2,<3.0.0)
 Requires-Dist: Flask-Cors (>=3.0.9,<4.0.0) Requires-Dist: Flask-Migrate
 (>=2.6.0,<3.0.0) Requires-Dist: MarkupSafe (>=2.1.2,<3.0.0) Requires-Dist:
@@ -81,68 +81,80 @@
 framework also supports backtesting and performing backtest experiments. After
 a backtest, you can print a report that shows the performance of your trading
 bot. To run a single backtest you can use the example code that can be found
 [here](./examples/backtest). ### Backtesting report You can use the
 ```pretty_print_backtest``` function to print a backtest report. For example if
 you run the [moving average example trading bot](./examples/
 crossover_moving_average_trading_bot) you will get the following backtesting
-report: ```bash ====================Backtest
-report=============================== * Start date: 2023-08-24 00:00:00 * End
-date: 2023-12-02 00:00:00 * Number of days: 100 * Number of runs: 1201
-====================Portfolio overview============================ * Number of
-orders: 10 * Initial balance: 400.0000 EUR * Final balance: 431.8837 EUR *
-Total net gain: 28.4171 EUR * Total net gain percentage: 7.1043% * Growth rate:
-7.9709% * Growth 31.8837 EUR ====================Positions
-overview========================
+report: ```bash /&# #&( Backtest report &&&&&&&&&&&# &&&&&&&&&&&& -------------
+-------------- &&&&&&&&&&&&&&&& (&&&&&&&&&&&&&&& Start date: 2023-08-24 00:00:
+00 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&& End date: 2023-12-02 00:00:
+00 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&& Number of days: 100
+&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&& Number of runs: 1201
+.&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&& Number of orders: 10
+&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&. Initial balance: 400.0 &&&&&&&# /
+((( &&&&&&&&&&&&*((( .&&&&&&&. Final balance: 431.1499 &&&&&&&&&&&&&&&&&&& (((
+( &&&&&&&& (((( &&&&&&&&&&&&&&&&&&& Total net gain: 28.5542 7.139% (((&&&&&&&&
+(((( &&&&&& (((( &&&&&&&&&(( Growth: 31.1499 7.787% /((((((((((&&&&&&&&&& (((,
+&&&&&& (((**&&&&&&&&&((((((((((( Number of trades closed: 4
+&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&& Number of trades open
+(end of backtest): 2 &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&& Percentage
+positive trades: 60.0% &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&& Percentage
+negative trades: 20.0% ((((( &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&&( Average trade
+size: 98.9886 EUR ((((( &&&&&&&&&&&&&&&&&&&&&&&&, Average trade duration: 184.0
+hours ((((( &&&&&&&&&&&&&# ((((( #&&&&&&&&&&### ((((( &&&&&&&&&&&###. .((((
+( &&&&&&&&&&&&&&###( ((((( &&&&&&&&&&&&&&&&#(((/ ((((( &&&&&&&&&&&&&&&&&&&@(((
+( ((((( &&&&&&&&&&&&&&&&&&&&&&(((( ((((( &&&&&&&&&&&&&&&&&&&&&&&&((((, .((((
+( &&&&&&&&&&&&&&&&&&&&&&&&&&(((( ((((( &&&&&&&&&&&&&&&&&&&&&&&&&&&&(((( ((((
+( &&&&&&&&&&&&&&&&&&&&&&&&&&&&&(((( ((((( &&&&&&&&&&&&&&&&&&&&&&&&&&&&&&(((( ((
+((( &&&&&&&&&&&&&&&&&&&&&&&&&&&&&#(((( ((((((((((((((((((
+(#########&&&&&&&&&&&&&&&&&&&&&&&&&&&&((((( ((((((((((((((((((((
+(######&&&&&&&&&&&&&&&&&&&&&&&&&&&&(((( Positions overview
 â­âââââââââââââ¬âââââââââââ¬âââââââââââââââââââââââ¬ââââââââââââââââââââââââ¬âââââââââââââââ¬ââââââââââââââââ¬ââââââââââââââââââââââââââââ¬âââââââââââââââââ¬ââââââââââââââââ®
 â Position â Amount â Pending buy amount â Pending sell amount â Cost
 (EUR) â Value (EUR) â Percentage of portfolio â Growth (EUR) â
 Growth_rate â
 ââââââââââââââ¼âââââââââââ¼âââââââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââ¼ââââââââââââââââ¼ââââââââââââââââââââââââââââ¼âââââââââââââââââ¼ââââââââââââââââ¤
-â EUR â 214.219 â 0 â 0 â 214.219 â 214.219 â 49.6010% â 0 â
+â EUR â 217.044 â 0 â 0 â 217.044 â 217.044 â 50.3407% â 0 â
 0.0000% â
 ââââââââââââââ¼âââââââââââ¼âââââââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââ¼ââââââââââââââââ¼ââââââââââââââââââââââââââââ¼âââââââââââââââââ¼ââââââââââââââââ¤
-â BTC â 0.0031 â 0 â 0 â 107.095 â 110.401 â 25.5627% â 3.3066
-â 3.0875% â
+â BTC â 0.003 â 0 â 0 â 104.372 â 106.84 â 24.7802% â 2.4678
+â 2.3644% â
 ââââââââââââââ¼âââââââââââ¼âââââââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââ¼ââââââââââââââââ¼ââââââââââââââââââââââââââââ¼âââââââââââââââââ¼ââââââââââââââââ¤
-â DOT â 21.3291 â 0 â 0 â 107.104 â 107.264 â 24.8363% â 0.16
-â 0.1494% â
+â DOT â 21.3295 â 0 â 0 â 107.138 â 107.266 â 24.8791% â 0.128
+â 0.1195% â
 â°âââââââââââââ´âââââââââââ´âââââââââââââââââââââââ´ââââââââââââââââââââââââ´âââââââââââââââ´ââââââââââââââââ´ââââââââââââââââââââââââââââ´âââââââââââââââââ´ââââââââââââââââ¯
-====================Trades overview=========================== * Number of
-trades closed: 4 * Number of trades open: 2 * Percentage of positive trades:
-60.0% * Percentage of negative trades: 20.0% * Average trade size: 98.8728 EUR
-* Average trade duration: 183.5 hours
+Trades overview
 â­ââââââââââ¬ââââââââââââââââââââââ¬ââââââââââââââââââââââ¬âââââââââââââââââââââ¬âââââââââââââââ¬âââââââââââââââââââ¬ââââââââââââââââââââââââ¬âââââââââââââââââââââ¬ââââââââââââââââââââââ®
 â Pair â Open date â Close date â Duration (hours) â Size (EUR) â
 Net gain (EUR) â Net gain percentage â Open price (EUR) â Close price
 (EUR) â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â DOT-EUR â 2023-11-30 20:00:00 â â 2976.65 â 107.104 â 0 â
-0.0000% â 5.0215 â â
+â DOT-EUR â 2023-11-30 18:00:00 â â 3207.26 â 107.138 â 0 â
+0.0000% â 5.023 â â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â BTC-EUR â 2023-11-29 14:00:00 â â 3006.65 â 107.095 â 0 â
-0.0000% â 34546.6 â â
+â BTC-EUR â 2023-11-29 12:00:00 â â 3237.26 â 104.372 â 0 â
+0.0000% â 34790.7 â â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â BTC-EUR â 2023-11-08 00:00:00 â 2023-11-14 16:00:00 â 160 â 99.2265
-â 1.3352 â 1.3456% â 33075.5 â 33520.6 â
+â BTC-EUR â 2023-11-07 22:00:00 â 2023-11-14 14:00:00 â 160 â 99.2337
+â 2.5395 â 2.5591% â 33077.9 â 33924.4 â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â BTC-EUR â 2023-11-06 16:00:00 â 2023-11-06 20:00:00 â 4 â 97.8607
-â -0.0026 â -0.0026% â 32620.2 â 32619.4 â
+â BTC-EUR â 2023-11-06 14:00:00 â 2023-11-06 18:00:00 â 4 â 98.2854
+â -0.4248 â -0.4322% â 32761.8 â 32620.2 â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â DOT-EUR â 2023-10-30 06:00:00 â 2023-11-14 00:00:00 â 354 â 100.551
-â 24.8794 â 24.7430% â 4.0375 â 5.0365 â
+â DOT-EUR â 2023-10-30 04:00:00 â 2023-11-14 00:00:00 â 356 â 100.537
+â 24.2886 â 24.1588% â 4.0565 â 5.0365 â
 âââââââââââ¼ââââââââââââââââââââââ¼ââââââââââââââââââââââ¼âââââââââââââââââââââ¼âââââââââââââââ¼âââââââââââââââââââ¼ââââââââââââââââââââââââ¼âââââââââââââââââââââ¼ââââââââââââââââââââââ¤
-â BTC-EUR â 2023-09-13 16:00:00 â 2023-09-22 16:00:00 â 216 â 97.8529
-â 2.2051 â 2.2534% â 24463.2 â 25014.5 â
+â BTC-EUR â 2023-09-13 14:00:00 â 2023-09-22 14:00:00 â 216 â 97.8976
+â 2.1508 â 2.1970% â 24474.4 â 25012.1 â
 â°ââââââââââ´ââââââââââââââââââââââ´ââââââââââââââââââââââ´âââââââââââââââââââââ´âââââââââââââââ´âââââââââââââââââââ´ââââââââââââââââââââââââ´âââââââââââââââââââââ´ââââââââââââââââââââââ¯
-================================================================== ``` ###
-Backtest experiments The framework also supports backtest experiments. Backtest
-experiments allows you to compare multiple algorithms and evaluate their
-performance. Ideally, you would do this by parameterizing your strategy and
-creating a factory function that creates the algorithm with the different
+``` ### Backtest experiments The framework also supports backtest experiments.
+Backtest experiments allows you to compare multiple algorithms and evaluate
+their performance. Ideally, you would do this by parameterizing your strategy
+and creating a factory function that creates the algorithm with the different
 parameters. You can find an example of this in the [backtest experiments
 example](./examples/backtest_experiment). ## Broker/Exchange configuration The
 framework has by default support for [ccxt](https://github.com/ccxt/ccxt). This
 should allow you to connect to a lot of brokers/exchanges. ```python from
 investing_algorithm_framework import PortfolioConfiguration, \
 MarketCredential, create_app app = create_app() app.add_market_credential
 ( MarketCredential( market="", api_key="", secret_key="", ) )
```

