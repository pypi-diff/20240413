# Comparing `tmp/investing_algorithm_framework-3.5.0.tar.gz` & `tmp/investing_algorithm_framework-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "investing_algorithm_framework-3.5.0.tar", max compression
+gzip compressed data, was "investing_algorithm_framework-3.5.1.tar", max compression
```

## Comparing `investing_algorithm_framework-3.5.0.tar` & `investing_algorithm_framework-3.5.1.tar`

### file list

```diff
@@ -1,142 +1,142 @@
--rw-r--r--   0        0        0    11343 2024-04-12 09:32:30.550392 investing_algorithm_framework-3.5.0/LICENSE
--rw-r--r--   0        0        0    21956 2024-04-12 09:32:30.550392 investing_algorithm_framework-3.5.0/README.md
--rw-r--r--   0        0        0     2084 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/__init__.py
--rw-r--r--   0        0        0      501 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/__init__.py
--rw-r--r--   0        0        0    34948 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/algorithm.py
--rw-r--r--   0        0        0    32187 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/app.py
--rw-r--r--   0        0        0     1092 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/__init__.py
--rw-r--r--   0        0        0     2362 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
--rw-r--r--   0        0        0      154 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
--rw-r--r--   0        0        0      452 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
--rw-r--r--   0        0        0     1062 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
--rw-r--r--   0        0        0     1085 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/exception_handler.py
--rw-r--r--   0        0        0     3750 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/strategy.py
--rw-r--r--   0        0        0      963 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/task.py
--rw-r--r--   0        0        0      134 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/__init__.py
--rw-r--r--   0        0        0      587 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/__init__.py
--rw-r--r--   0        0        0      694 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/orders.py
--rw-r--r--   0        0        0      727 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/portfolio.py
--rw-r--r--   0        0        0      617 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/positions.py
--rw-r--r--   0        0        0      506 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/create_app.py
--rw-r--r--   0        0        0     2020 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/error_handler.py
--rw-r--r--   0        0        0      585 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/responses.py
--rw-r--r--   0        0        0      158 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/run_strategies.py
--rw-r--r--   0        0        0      361 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/schemas/__init__.py
--rw-r--r--   0        0        0      442 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/schemas/order.py
--rw-r--r--   0        0        0      743 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/schemas/portfolio.py
--rw-r--r--   0        0        0      438 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/schemas/position.py
--rw-r--r--   0        0        0       80 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/setup_cors.py
--rw-r--r--   0        0        0      603 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/create_app.py
--rw-r--r--   0        0        0     6312 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/dependency_container.py
--rw-r--r--   0        0        0     3912 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/__init__.py
--rw-r--r--   0        0        0     3728 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/config.py
--rw-r--r--   0        0        0     2293 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/constants.py
--rw-r--r--   0        0        0      962 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/data_structures.py
--rw-r--r--   0        0        0      823 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/decimal_parsing.py
--rw-r--r--   0        0        0     1628 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/exceptions.py
--rw-r--r--   0        0        0     1121 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/__init__.py
--rw-r--r--   0        0        0      812 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/app_mode.py
--rw-r--r--   0        0        0      253 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/backtesting/__init__.py
--rw-r--r--   0        0        0     2374 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/backtesting/backtest_position.py
--rw-r--r--   0        0        0    13619 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/backtesting/backtest_report.py
--rw-r--r--   0        0        0     2309 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py
--rw-r--r--   0        0        0      659 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/base_model.py
--rw-r--r--   0        0        0       87 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/market/__init__.py
--rw-r--r--   0        0        0      779 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/market/market_credential.py
--rw-r--r--   0        0        0      237 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/__init__.py
--rw-r--r--   0        0        0    10363 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order.py
--rw-r--r--   0        0        0     1110 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_fee.py
--rw-r--r--   0        0        0      814 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_side.py
--rw-r--r--   0        0        0      937 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_status.py
--rw-r--r--   0        0        0      751 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_type.py
--rw-r--r--   0        0        0      230 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/portfolio/__init__.py
--rw-r--r--   0        0        0     2495 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py
--rw-r--r--   0        0        0     1752 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
--rw-r--r--   0        0        0     3141 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py
--rw-r--r--   0        0        0      123 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/position/__init__.py
--rw-r--r--   0        0        0     1251 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/position/position.py
--rw-r--r--   0        0        0     1131 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/position/position_snapshot.py
--rw-r--r--   0        0        0     4598 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/strategy_profile.py
--rw-r--r--   0        0        0     2659 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/time_frame.py
--rw-r--r--   0        0        0     2798 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/time_interval.py
--rw-r--r--   0        0        0     2011 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/time_unit.py
--rw-r--r--   0        0        0       99 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trade/__init__.py
--rw-r--r--   0        0        0     7114 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trade/trade.py
--rw-r--r--   0        0        0      807 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trade/trade_status.py
--rw-r--r--   0        0        0     1119 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trading_data_types.py
--rw-r--r--   0        0        0     6791 2024-04-12 09:32:30.554392 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trading_time_frame.py
--rw-r--r--   0        0        0      634 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/__init__.py
--rw-r--r--   0        0        0     1047 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/market_credential_service.py
--rw-r--r--   0        0        0     9941 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/market_data_sources.py
--rw-r--r--   0        0        0     3522 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/market_service.py
--rw-r--r--   0        0        0      115 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/portfolios/__init__.py
--rw-r--r--   0        0        0      320 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/portfolios/portfolio_sync_service.py
--rw-r--r--   0        0        0      699 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/rounding_service.py
--rw-r--r--   0        0        0      258 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/singleton.py
--rw-r--r--   0        0        0      156 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/stateless_actions.py
--rw-r--r--   0        0        0     1805 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/strategy.py
--rw-r--r--   0        0        0      700 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/__init__.py
--rw-r--r--   0        0        0    25794 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/backtesting.py
--rw-r--r--   0        0        0     2746 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/csv.py
--rw-r--r--   0        0        0      275 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/random.py
--rw-r--r--   0        0        0      417 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/signatures.py
--rw-r--r--   0        0        0      608 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/stoppable_thread.py
--rw-r--r--   0        0        0      253 2024-04-12 09:32:30.558393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/synchronized.py
--rw-r--r--   0        0        0     1361 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/__init__.py
--rw-r--r--   0        0        0      176 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/database/__init__.py
--rw-r--r--   0        0        0     1386 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
--rw-r--r--   0        0        0      732 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/__init__.py
--rw-r--r--   0        0        0      327 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/decimal_parser.py
--rw-r--r--   0        0        0      437 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/market_data_sources/__init__.py
--rw-r--r--   0        0        0    17349 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py
--rw-r--r--   0        0        0     5472 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py
--rw-r--r--   0        0        0      142 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/model_extension.py
--rw-r--r--   0        0        0      102 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/order/__init__.py
--rw-r--r--   0        0        0     4877 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/order/order.py
--rw-r--r--   0        0        0      847 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/order/order_fee.py
--rw-r--r--   0        0        0      141 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
--rw-r--r--   0        0        0     3226 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
--rw-r--r--   0        0        0     1238 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py
--rw-r--r--   0        0        0      135 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/position/__init__.py
--rw-r--r--   0        0        0     1898 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/position/position.py
--rw-r--r--   0        0        0      842 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py
--rw-r--r--   0        0        0      567 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/__init__.py
--rw-r--r--   0        0        0      487 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
--rw-r--r--   0        0        0     3351 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py
--rw-r--r--   0        0        0     1073 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
--rw-r--r--   0        0        0     1967 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py
--rw-r--r--   0        0        0     1994 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py
--rw-r--r--   0        0        0      680 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py
--rw-r--r--   0        0        0     7661 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/repository.py
--rw-r--r--   0        0        0      163 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/__init__.py
--rw-r--r--   0        0        0       91 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/market_service/__init__.py
--rw-r--r--   0        0        0    15303 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py
--rw-r--r--   0        0        0      195 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/performance_service/__init__.py
--rw-r--r--   0        0        0       43 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/performance_service/backtest_performance_service.py
--rw-r--r--   0        0        0    11933 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py
--rw-r--r--   0        0        0     1318 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/__init__.py
--rw-r--r--   0        0        0      191 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/backtesting/__init__.py
--rw-r--r--   0        0        0     1401 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py
--rw-r--r--   0        0        0    15031 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/backtesting/backtest_service.py
--rw-r--r--   0        0        0      624 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/configuration_service.py
--rw-r--r--   0        0        0      821 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/market_credential_service.py
--rw-r--r--   0        0        0      235 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/market_data_source_service/__init__.py
--rw-r--r--   0        0        0     5214 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py
--rw-r--r--   0        0        0     6307 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py
--rw-r--r--   0        0        0      159 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/order_service/__init__.py
--rw-r--r--   0        0        0     7735 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/order_service/order_backtest_service.py
--rw-r--r--   0        0        0    27824 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/order_service/order_service.py
--rw-r--r--   0        0        0      509 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/__init__.py
--rw-r--r--   0        0        0      825 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py
--rw-r--r--   0        0        0     2055 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py
--rw-r--r--   0        0        0     4493 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_service.py
--rw-r--r--   0        0        0     1984 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py
--rw-r--r--   0        0        0    16127 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py
--rw-r--r--   0        0        0     1052 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/position_service.py
--rw-r--r--   0        0        0      525 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/position_snapshot_service.py
--rw-r--r--   0        0        0      995 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/repository_service.py
--rw-r--r--   0        0        0     8077 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/strategy_orchestrator_service.py
--rw-r--r--   0        0        0       68 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/trade_service/__init__.py
--rw-r--r--   0        0        0    14761 2024-04-12 09:32:30.562393 investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/trade_service/trade_service.py
--rw-r--r--   0        0        0      742 2024-04-12 09:32:38.370404 investing_algorithm_framework-3.5.0/pyproject.toml
--rw-r--r--   0        0        0    23028 1970-01-01 00:00:00.000000 investing_algorithm_framework-3.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11343 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/LICENSE
+-rw-r--r--   0        0        0    21956 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/README.md
+-rw-r--r--   0        0        0     2084 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/__init__.py
+-rw-r--r--   0        0        0      501 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/__init__.py
+-rw-r--r--   0        0        0    34948 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/algorithm.py
+-rw-r--r--   0        0        0    32200 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/app.py
+-rw-r--r--   0        0        0     1092 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/stateless/__init__.py
+-rw-r--r--   0        0        0     2362 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/stateless/action_handlers/__init__.py
+-rw-r--r--   0        0        0      154 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/stateless/action_handlers/action_handler_strategy.py
+-rw-r--r--   0        0        0      452 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/stateless/action_handlers/check_online_handler.py
+-rw-r--r--   0        0        0     1062 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py
+-rw-r--r--   0        0        0     1085 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/stateless/exception_handler.py
+-rw-r--r--   0        0        0     3887 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/strategy.py
+-rw-r--r--   0        0        0      963 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/task.py
+-rw-r--r--   0        0        0      134 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/__init__.py
+-rw-r--r--   0        0        0      587 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/controllers/__init__.py
+-rw-r--r--   0        0        0      694 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/controllers/orders.py
+-rw-r--r--   0        0        0      727 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/controllers/portfolio.py
+-rw-r--r--   0        0        0      617 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/controllers/positions.py
+-rw-r--r--   0        0        0      506 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/create_app.py
+-rw-r--r--   0        0        0     2020 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/error_handler.py
+-rw-r--r--   0        0        0      585 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/responses.py
+-rw-r--r--   0        0        0      158 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/run_strategies.py
+-rw-r--r--   0        0        0      361 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/schemas/__init__.py
+-rw-r--r--   0        0        0      442 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/schemas/order.py
+-rw-r--r--   0        0        0      743 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/schemas/portfolio.py
+-rw-r--r--   0        0        0      438 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/schemas/position.py
+-rw-r--r--   0        0        0       80 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/setup_cors.py
+-rw-r--r--   0        0        0      603 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/create_app.py
+-rw-r--r--   0        0        0     6312 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/dependency_container.py
+-rw-r--r--   0        0        0     3912 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/__init__.py
+-rw-r--r--   0        0        0     3728 2024-04-12 23:47:46.777660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/config.py
+-rw-r--r--   0        0        0     2293 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/constants.py
+-rw-r--r--   0        0        0      962 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/data_structures.py
+-rw-r--r--   0        0        0      823 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/decimal_parsing.py
+-rw-r--r--   0        0        0     1628 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/exceptions.py
+-rw-r--r--   0        0        0     1121 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/__init__.py
+-rw-r--r--   0        0        0      812 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/app_mode.py
+-rw-r--r--   0        0        0      253 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/backtesting/__init__.py
+-rw-r--r--   0        0        0     2374 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/backtesting/backtest_position.py
+-rw-r--r--   0        0        0    13619 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/backtesting/backtest_report.py
+-rw-r--r--   0        0        0     2309 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py
+-rw-r--r--   0        0        0      659 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/base_model.py
+-rw-r--r--   0        0        0       87 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/market/__init__.py
+-rw-r--r--   0        0        0      779 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/market/market_credential.py
+-rw-r--r--   0        0        0      237 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/order/__init__.py
+-rw-r--r--   0        0        0    10363 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/order/order.py
+-rw-r--r--   0        0        0     1110 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/order/order_fee.py
+-rw-r--r--   0        0        0      814 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/order/order_side.py
+-rw-r--r--   0        0        0      937 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/order/order_status.py
+-rw-r--r--   0        0        0      751 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/order/order_type.py
+-rw-r--r--   0        0        0      230 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/portfolio/__init__.py
+-rw-r--r--   0        0        0     2495 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/portfolio/portfolio.py
+-rw-r--r--   0        0        0     1752 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py
+-rw-r--r--   0        0        0     3141 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py
+-rw-r--r--   0        0        0      123 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/position/__init__.py
+-rw-r--r--   0        0        0     1251 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/position/position.py
+-rw-r--r--   0        0        0     1131 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/position/position_snapshot.py
+-rw-r--r--   0        0        0     4598 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/strategy_profile.py
+-rw-r--r--   0        0        0     2659 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/time_frame.py
+-rw-r--r--   0        0        0     2798 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/time_interval.py
+-rw-r--r--   0        0        0     2011 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/time_unit.py
+-rw-r--r--   0        0        0       99 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/trade/__init__.py
+-rw-r--r--   0        0        0     7114 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/trade/trade.py
+-rw-r--r--   0        0        0      807 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/trade/trade_status.py
+-rw-r--r--   0        0        0     1119 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/trading_data_types.py
+-rw-r--r--   0        0        0     6791 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/trading_time_frame.py
+-rw-r--r--   0        0        0      634 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/services/__init__.py
+-rw-r--r--   0        0        0     1047 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/services/market_credential_service.py
+-rw-r--r--   0        0        0     9941 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/services/market_data_sources.py
+-rw-r--r--   0        0        0     3522 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/services/market_service.py
+-rw-r--r--   0        0        0      115 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/services/portfolios/__init__.py
+-rw-r--r--   0        0        0      320 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/services/portfolios/portfolio_sync_service.py
+-rw-r--r--   0        0        0      699 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/services/rounding_service.py
+-rw-r--r--   0        0        0      258 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/singleton.py
+-rw-r--r--   0        0        0      156 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/stateless_actions.py
+-rw-r--r--   0        0        0     1805 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/strategy.py
+-rw-r--r--   0        0        0      700 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/utils/__init__.py
+-rw-r--r--   0        0        0    25794 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/utils/backtesting.py
+-rw-r--r--   0        0        0     2746 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/utils/csv.py
+-rw-r--r--   0        0        0      275 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/utils/random.py
+-rw-r--r--   0        0        0      417 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/utils/signatures.py
+-rw-r--r--   0        0        0      608 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/utils/stoppable_thread.py
+-rw-r--r--   0        0        0      253 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/utils/synchronized.py
+-rw-r--r--   0        0        0     1361 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/__init__.py
+-rw-r--r--   0        0        0      176 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/database/__init__.py
+-rw-r--r--   0        0        0     1386 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/database/sql_alchemy.py
+-rw-r--r--   0        0        0      732 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/__init__.py
+-rw-r--r--   0        0        0      327 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/decimal_parser.py
+-rw-r--r--   0        0        0      437 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/market_data_sources/__init__.py
+-rw-r--r--   0        0        0    17538 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py
+-rw-r--r--   0        0        0     5472 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py
+-rw-r--r--   0        0        0      142 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/model_extension.py
+-rw-r--r--   0        0        0      102 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/order/__init__.py
+-rw-r--r--   0        0        0     4877 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/order/order.py
+-rw-r--r--   0        0        0      847 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/order/order_fee.py
+-rw-r--r--   0        0        0      141 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/portfolio/__init__.py
+-rw-r--r--   0        0        0     3226 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py
+-rw-r--r--   0        0        0     1238 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py
+-rw-r--r--   0        0        0      135 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/position/__init__.py
+-rw-r--r--   0        0        0     1898 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/position/position.py
+-rw-r--r--   0        0        0      842 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py
+-rw-r--r--   0        0        0      567 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/repositories/__init__.py
+-rw-r--r--   0        0        0      487 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/repositories/order_fee_repository.py
+-rw-r--r--   0        0        0     3351 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/repositories/order_repository.py
+-rw-r--r--   0        0        0     1073 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py
+-rw-r--r--   0        0        0     1967 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py
+-rw-r--r--   0        0        0     1994 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/repositories/position_repository.py
+-rw-r--r--   0        0        0      680 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py
+-rw-r--r--   0        0        0     7661 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/repositories/repository.py
+-rw-r--r--   0        0        0      163 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/services/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/services/market_service/__init__.py
+-rw-r--r--   0        0        0    15303 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py
+-rw-r--r--   0        0        0      195 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/services/performance_service/__init__.py
+-rw-r--r--   0        0        0       43 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/services/performance_service/backtest_performance_service.py
+-rw-r--r--   0        0        0    11933 2024-04-12 23:47:46.781660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py
+-rw-r--r--   0        0        0     1318 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/__init__.py
+-rw-r--r--   0        0        0      191 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/backtesting/__init__.py
+-rw-r--r--   0        0        0     1401 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py
+-rw-r--r--   0        0        0    15033 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/backtesting/backtest_service.py
+-rw-r--r--   0        0        0      624 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/configuration_service.py
+-rw-r--r--   0        0        0      821 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/market_credential_service.py
+-rw-r--r--   0        0        0      235 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/market_data_source_service/__init__.py
+-rw-r--r--   0        0        0     5264 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py
+-rw-r--r--   0        0        0     6873 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py
+-rw-r--r--   0        0        0      159 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/order_service/__init__.py
+-rw-r--r--   0        0        0     7834 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/order_service/order_backtest_service.py
+-rw-r--r--   0        0        0    27824 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/order_service/order_service.py
+-rw-r--r--   0        0        0      509 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/portfolios/__init__.py
+-rw-r--r--   0        0        0      825 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py
+-rw-r--r--   0        0        0     2055 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py
+-rw-r--r--   0        0        0     4493 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/portfolios/portfolio_service.py
+-rw-r--r--   0        0        0     1984 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py
+-rw-r--r--   0        0        0    16127 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py
+-rw-r--r--   0        0        0     1052 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/position_service.py
+-rw-r--r--   0        0        0      525 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/position_snapshot_service.py
+-rw-r--r--   0        0        0      995 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/repository_service.py
+-rw-r--r--   0        0        0     8077 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/strategy_orchestrator_service.py
+-rw-r--r--   0        0        0       68 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/trade_service/__init__.py
+-rw-r--r--   0        0        0    14761 2024-04-12 23:47:46.785660 investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/trade_service/trade_service.py
+-rw-r--r--   0        0        0      742 2024-04-12 23:47:55.525631 investing_algorithm_framework-3.5.1/pyproject.toml
+-rw-r--r--   0        0        0    23028 1970-01-01 00:00:00.000000 investing_algorithm_framework-3.5.1/PKG-INFO
```

### Comparing `investing_algorithm_framework-3.5.0/LICENSE` & `investing_algorithm_framework-3.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/README.md` & `investing_algorithm_framework-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/__init__.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/algorithm.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/algorithm.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/app.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/app.py`

 * *Files 0% similar despite different names*

```diff
@@ -235,16 +235,16 @@
                 )
             self._create_database_if_not_exists()
 
     def _initialize_app_for_backtest(
         self,
         backtest_start_date,
         backtest_end_date,
-        pending_order_check_interval,
         market_data_sources,
+        pending_order_check_interval=None,
     ) -> None:
         """
         Initialize the app for backtesting by setting the configuration
         parameters for backtesting and overriding the services with the
         backtest services equivalents. This method should only be called
         before running a backtest or a set of backtests and should be called
         once.
@@ -257,17 +257,19 @@
         """
         # Set all config vars for backtesting
         configuration_service = self.container.configuration_service()
         configuration_service.config[BACKTESTING_FLAG] = True
         configuration_service.config[BACKTESTING_START_DATE] = \
             backtest_start_date
         configuration_service.config[BACKTESTING_END_DATE] = backtest_end_date
-        configuration_service.config[
-            BACKTESTING_PENDING_ORDER_CHECK_INTERVAL
-        ] = pending_order_check_interval
+
+        if pending_order_check_interval is not None:
+            configuration_service.config[
+                BACKTESTING_PENDING_ORDER_CHECK_INTERVAL
+            ] = pending_order_check_interval
 
         # Create resource dir if not exits
         self._create_resource_directory_if_not_exists()
 
         # Override the MarketDataSourceService service with the backtest
         # market data source service equivalent. Additionally, convert the
         # market data sources to backtest market data sources
@@ -494,15 +496,14 @@
         number_of_iterations_since_last_orders_check = 1
         self.algorithm.check_pending_orders()
 
         try:
             while self.algorithm.running:
                 if number_of_iterations_since_last_orders_check == 30:
                     logger.info("Checking pending orders")
-                    self.algorithm.check_pending_orders()
                     number_of_iterations_since_last_orders_check = 1
 
                 self.algorithm.run_jobs()
                 number_of_iterations_since_last_orders_check += 1
                 sleep(1)
         except KeyboardInterrupt:
             exit(0)
@@ -671,15 +672,15 @@
         return self.algorithm.get_portfolio_configurations()
 
     def run_backtest(
         self,
         algorithm,
         start_date,
         end_date,
-        pending_order_check_interval='1h',
+        pending_order_check_interval=None,
         output_directory=None
     ) -> BacktestReport:
         """
         Run a backtest for an algorithm. This method should be called when
         running a backtest.
 
         :param algorithm: The algorithm to run a backtest for (instance of
@@ -736,15 +737,15 @@
 
     def run_backtests(
         self,
         algorithms,
         start_date: Optional[datetime] = None,
         end_date: Optional[datetime] = None,
         date_ranges: Optional[Tuple[datetime, datetime]] = None,
-        pending_order_check_interval='1h',
+        pending_order_check_interval=None,
         output_directory=None
     ) -> List[BacktestReport]:
         """
         Run a backtest for a set algorithm. This method should be called when
         running a backtest.
 
         :param algorithms: The algorithms to run backtests for (list of
```

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/__init__.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/stateless/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/action_handlers/__init__.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/stateless/action_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/stateless/action_handlers/run_strategy_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/stateless/exception_handler.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/stateless/exception_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/strategy.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/strategy.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,14 +56,18 @@
         # Check if interval is None
         if self.interval is None:
             raise OperationalException(
                 f"Interval not set for strategy instance {self.strategy_id}"
             )
 
     def run_strategy(self, algorithm, market_data):
+        # Check pending orders before running the strategy
+        algorithm.check_pending_orders()
+
+        # Run user defined strategy
         self.apply_strategy(algorithm=algorithm, market_data=market_data)
 
     def apply_strategy(self, algorithm, market_data):
         if self.decorated:
             self.decorated(algorithm=algorithm, market_data=market_data)
         else:
             raise NotImplementedError("Apply strategy is not implemented")
```

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/task.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/task.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/__init__.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/orders.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/controllers/orders.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/portfolio.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/controllers/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/controllers/positions.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/controllers/positions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/error_handler.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/error_handler.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/responses.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/responses.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/app/web/schemas/portfolio.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/app/web/schemas/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/create_app.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/create_app.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/dependency_container.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/dependency_container.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/__init__.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/config.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/config.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/constants.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/constants.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/data_structures.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/data_structures.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/decimal_parsing.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/decimal_parsing.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/exceptions.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/exceptions.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/__init__.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/app_mode.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/app_mode.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/backtesting/backtest_position.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/backtesting/backtest_position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/backtesting/backtest_report.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/backtesting/backtest_report.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/backtesting/backtest_reports_evaluation.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/base_model.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/base_model.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/market/market_credential.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/market/market_credential.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/order/order.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_fee.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/order/order_fee.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_side.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/order/order_side.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_status.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/order/order_status.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/order/order_type.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/order/order_type.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/portfolio/portfolio.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/portfolio/portfolio_configuration.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/portfolio/portfolio_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/position/position.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/position/position_snapshot.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/position/position_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/strategy_profile.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/strategy_profile.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/time_frame.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/time_interval.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/time_interval.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/time_unit.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/time_unit.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trade/trade.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/trade/trade.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trade/trade_status.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/trade/trade_status.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trading_data_types.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/trading_data_types.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/models/trading_time_frame.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/models/trading_time_frame.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/__init__.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/services/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/market_credential_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/services/market_credential_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/market_data_sources.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/services/market_data_sources.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/market_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/services/market_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/services/rounding_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/services/rounding_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/strategy.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/strategy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/__init__.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/backtesting.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/utils/backtesting.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/csv.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/utils/csv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/domain/utils/stoppable_thread.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/domain/utils/stoppable_thread.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/__init__.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/database/sql_alchemy.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/database/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/__init__.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/market_data_sources/ccxt.py`

 * *Files 1% similar despite different names*

```diff
@@ -233,32 +233,39 @@
 
     To achieve this, a backtest_data_start_date attribute is used. This
     attribute is indexed on this calculated date.
     """
     backtest_data_directory = None
     backtest_data_start_date = None
     backtest_data_end_date = None
-    timeframe = "15m"
+    timeframe = None
     column_names = ["Datetime", "Open", "High", "Low", "Close", "Volume"]
 
     def __init__(
         self,
         identifier,
         market,
         symbol=None,
-        timeframe="15m",
+        timeframe=None,
     ):
         super().__init__(
             identifier=identifier,
             market=market,
             symbol=symbol,
         )
+
         if timeframe is not None:
             self.timeframe = timeframe
 
+        if self.timeframe is None:
+            raise OperationalException(
+                "timeframe should be set for "
+                "CCXTTickerBacktestMarketDataSource"
+            )
+
     def prepare_data(
         self,
         config,
         backtest_start_date,
         backtest_end_date,
         **kwargs
     ):
```

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/market_data_sources/csv.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/order/order.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/order/order.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/order/order_fee.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/order/order_fee.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/portfolio/portfolio_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/position/position.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/position/position.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/models/position/position_snapshot.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/__init__.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/repositories/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/order_repository.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/repositories/order_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/repositories/portfolio_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/repositories/portfolio_snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/position_repository.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/repositories/position_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/repositories/position_snapshot_repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/repositories/repository.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/repositories/repository.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/services/market_service/ccxt_market_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/infrastructure/services/performance_service/performance_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/__init__.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/__init__.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/backtesting/backtest_report_writer_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/backtesting/backtest_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/backtesting/backtest_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
                         self._market_data_source_service.get_data(
                             data_id.get_identifier()
                         )
                 else:
                     market_data[data_id] = \
                         self._market_data_source_service.get_data(data_id)
 
-        self._order_service.check_pending_orders()
+        # self._order_service.check_pending_orders()
         strategy.run_strategy(algorithm=algorithm, market_data=market_data)
 
     def generate_schedule(
         self,
         strategies,
         start_date,
         end_date
```

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/configuration_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/configuration_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/market_credential_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/market_credential_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/market_data_source_service/backtest_market_data_source_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,15 +105,20 @@
             self._market_credential_service
         return market_data_source.get_data(
             backtest_index_date=self._configuration_service
             .config[BACKTESTING_INDEX_DATETIME],
         )
 
     def get_ohlcv(
-        self, symbol, from_timestamp, market, time_frame, to_timestamp=None
+        self,
+        symbol,
+        from_timestamp,
+        time_frame=None,
+        market=None,
+        to_timestamp=None
     ):
         market_data_source = self.get_ohlcv_market_data_source(
             symbol=symbol, market=market, time_frame=time_frame
         )
         market_data_source.market_credential_service = \
             self._market_credential_service
         return market_data_source.get_data(
```

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/market_data_source_service/market_data_source_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,16 +56,16 @@
             )
 
         return self._market_service.get_order_book(symbol, market)
 
     def get_ohlcv(
         self,
         symbol,
-        time_frame,
         from_timestamp,
+        time_frame,
         market=None,
         to_timestamp=None
     ):
         ohlcv_market_data_source = self.get_ohlcv_market_data_source(
             symbol=symbol, market=market, time_frame=time_frame
         )
 
@@ -106,32 +106,44 @@
                     else:
                         if market_data_source.symbol.lower() \
                                 == symbol.lower():
                             return market_data_source
 
         return None
 
-    def get_ohlcv_market_data_source(self, symbol, time_frame, market=None):
+    def get_ohlcv_market_data_source(
+        self, symbol, time_frame=None, market=None
+    ):
 
         if self.market_data_sources is not None:
+
             for market_data_source in self._market_data_sources:
                 if isinstance(market_data_source, OHLCVMarketDataSource):
 
-                    if market is not None:
+                    if market is not None and time_frame is not None:
 
                         if market_data_source.market.lower() == market.lower()\
                                 and market_data_source.symbol.lower() \
                                 == symbol.lower() and \
                                 market_data_source.timeframe == time_frame:
                             return market_data_source
-                    else:
+                    elif market is not None:
+                        if market_data_source.market.lower() == market.lower()\
+                                and market_data_source.symbol.lower() \
+                                == symbol.lower():
+                            return market_data_source
+                    elif time_frame is not None:
                         if market_data_source.symbol.lower() \
                                 == symbol.lower() and \
                                 market_data_source.timeframe == time_frame:
                             return market_data_source
+                    else:
+                        if market_data_source.symbol.lower() \
+                                == symbol.lower():
+                            return market_data_source
 
         return None
 
     def get_order_book_market_data_source(self, symbol, market=None):
 
         if self.market_data_sources is not None:
             for market_data_source in self._market_data_sources:
```

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/order_service/order_backtest_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/order_service/order_backtest_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,21 +63,26 @@
         config = self.configuration_service.get_config()
 
         for order in pending_orders:
             symbol = f"{order.target_symbol.upper()}" \
                      f"/{order.trading_symbol.upper()}"
             position = self.position_repository.get(order.position_id)
             portfolio = self.portfolio_repository.get(position.portfolio_id)
+            timeframe = None
+
+            if BACKTESTING_PENDING_ORDER_CHECK_INTERVAL in \
+                    self.configuration_service.config:
+                timeframe = self.configuration_service\
+                    .config[BACKTESTING_PENDING_ORDER_CHECK_INTERVAL]
 
             if not self._market_data_source_service\
                     .is_ohlcv_data_source_present(
                         symbol=symbol,
                         market=portfolio.market,
-                        time_frame=self.configuration_service
-                        .config[BACKTESTING_PENDING_ORDER_CHECK_INTERVAL]
+                        time_frame=timeframe
                     ):
                 raise OperationalException(
                     f"OHLCV data source not found for {symbol} "
                     f"and market {portfolio.market} for order check "
                     f"time frame "
                     f"{config[BACKTESTING_PENDING_ORDER_CHECK_INTERVAL]}. "
                     f"Cannot check pending orders for symbol {symbol} "
@@ -86,20 +91,19 @@
                     f"time frame "
                     f"{config[BACKTESTING_PENDING_ORDER_CHECK_INTERVAL]} "
                 )
 
             df = self._market_data_source_service.get_ohlcv(
                 symbol=symbol,
                 market=portfolio.market,
+                time_frame=timeframe,
                 to_timestamp=self.configuration_service.config.get(
                     BACKTESTING_INDEX_DATETIME
                 ),
                 from_timestamp=order.get_created_at(),
-                time_frame=self.configuration_service
-                .config[BACKTESTING_PENDING_ORDER_CHECK_INTERVAL]
             )
 
             if self.has_executed(order, df):
                 self.update(
                     order.id,
                     {
                         "status": OrderStatus.CLOSED.value,
```

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/order_service/order_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/order_service/order_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/portfolios/backtest_portfolio_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/portfolios/portfolio_configuration_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/portfolios/portfolio_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/portfolios/portfolio_snapshot_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/portfolios/portfolio_sync_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/position_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/position_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/position_snapshot_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/position_snapshot_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/repository_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/repository_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/strategy_orchestrator_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/strategy_orchestrator_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/investing_algorithm_framework/services/trade_service/trade_service.py` & `investing_algorithm_framework-3.5.1/investing_algorithm_framework/services/trade_service/trade_service.py`

 * *Files identical despite different names*

### Comparing `investing_algorithm_framework-3.5.0/pyproject.toml` & `investing_algorithm_framework-3.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "investing-algorithm-framework"
-version = "v3.5.0"
+version = "v3.5.1"
 description = "A framework for creating trading bots"
 authors = ["MDUYN"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 wrapt = "^1.16.0"
```

### Comparing `investing_algorithm_framework-3.5.0/PKG-INFO` & `investing_algorithm_framework-3.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: investing-algorithm-framework
-Version: 3.5.0
+Version: 3.5.1
 Summary: A framework for creating trading bots
 Author: MDUYN
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: investing-algorithm-framework Version: 3.5.0
+Metadata-Version: 2.1 Name: investing-algorithm-framework Version: 3.5.1
 Summary: A framework for creating trading bots Author: MDUYN Requires-Python:
 >=3.8.1,<4.0.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Requires-Dist: Flask (>=2.3.2,<3.0.0)
 Requires-Dist: Flask-Cors (>=3.0.9,<4.0.0) Requires-Dist: Flask-Migrate
 (>=2.6.0,<3.0.0) Requires-Dist: MarkupSafe (>=2.1.2,<3.0.0) Requires-Dist:
```

