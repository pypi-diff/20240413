# Comparing `tmp/prosperity2bt-0.4.3.tar.gz` & `tmp/prosperity2bt-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prosperity2bt-0.4.3.tar", last modified: Thu Apr 11 22:32:17 2024, max compression
+gzip compressed data, was "prosperity2bt-0.4.4.tar", last modified: Sat Apr 13 14:26:03 2024, max compression
```

## Comparing `prosperity2bt-0.4.3.tar` & `prosperity2bt-0.4.4.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:32:17.571883 prosperity2bt-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-11 22:32:17.571883 prosperity2bt-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:32:17.563883 prosperity2bt-0.4.3/prosperity2bt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11880 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/datamodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:32:17.563883 prosperity2bt-0.4.3/prosperity2bt/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:32:17.567883 prosperity2bt-0.4.3/prosperity2bt/resources/round0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/resources/round0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:32:17.571883 prosperity2bt-0.4.3/prosperity2bt/resources/round1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/resources/round1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
--rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/resources/round1/prices_round_1_day_0.csv
--rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
--rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-11 22:32:13.000000 prosperity2bt-0.4.3/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 22:32:17.571883 prosperity2bt-0.4.3/prosperity2bt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-11 22:32:17.000000 prosperity2bt-0.4.3/prosperity2bt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-11 22:32:17.000000 prosperity2bt-0.4.3/prosperity2bt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 22:32:17.000000 prosperity2bt-0.4.3/prosperity2bt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-11 22:32:17.000000 prosperity2bt-0.4.3/prosperity2bt.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-11 22:32:17.000000 prosperity2bt-0.4.3/prosperity2bt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 22:32:17.000000 prosperity2bt-0.4.3/prosperity2bt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-11 22:32:15.000000 prosperity2bt-0.4.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 22:32:17.571883 prosperity2bt-0.4.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:26:03.916474 prosperity2bt-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-13 14:26:03.916474 prosperity2bt-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:26:03.904474 prosperity2bt-0.4.4/prosperity2bt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8461 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/file_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:26:03.908474 prosperity2bt-0.4.4/prosperity2bt/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:26:03.908474 prosperity2bt-0.4.4/prosperity2bt/resources/round0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   249265 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round0/prices_round_0_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    38097 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:26:03.912474 prosperity2bt-0.4.4/prosperity2bt/resources/round1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1257340 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round1/prices_round_1_day_-1.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1258643 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round1/prices_round_1_day_-2.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  1237383 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round1/prices_round_1_day_0.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   204939 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   208522 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   202884 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     9660 2024-04-13 14:25:59.000000 prosperity2bt-0.4.4/prosperity2bt/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 14:26:03.912474 prosperity2bt-0.4.4/prosperity2bt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5822 2024-04-13 14:26:03.000000 prosperity2bt-0.4.4/prosperity2bt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-04-13 14:26:03.000000 prosperity2bt-0.4.4/prosperity2bt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 14:26:03.000000 prosperity2bt-0.4.4/prosperity2bt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-13 14:26:03.000000 prosperity2bt-0.4.4/prosperity2bt.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-13 14:26:03.000000 prosperity2bt-0.4.4/prosperity2bt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-13 14:26:03.000000 prosperity2bt-0.4.4/prosperity2bt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-13 14:26:01.000000 prosperity2bt-0.4.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 14:26:03.916474 prosperity2bt-0.4.4/setup.cfg
```

### Comparing `prosperity2bt-0.4.3/LICENSE` & `prosperity2bt-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.3/PKG-INFO` & `prosperity2bt-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.4.3
+Version: 0.4.4
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2bt-0.4.3/README.md` & `prosperity2bt-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.3/prosperity2bt/__main__.py` & `prosperity2bt-0.4.4/prosperity2bt/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,73 +1,102 @@
-import json
 import sys
 import webbrowser
 from argparse import ArgumentParser
 from collections import defaultdict
 from datetime import datetime
 from functools import partial, reduce
 from http.server import HTTPServer, SimpleHTTPRequestHandler
-from importlib import import_module, metadata
+from importlib import import_module, metadata, reload
 from pathlib import Path
-from prosperity2bt.core import DayResult, run_backtest
-from prosperity2bt.data import DayData, read_day_data, read_round_data
-from prosperity2bt.datamodel import ProsperityEncoder
+from prosperity2bt.data import BacktestData, read_day_data
+from prosperity2bt.file_reader import FileSystemReader, PackageResourcesReader
+from prosperity2bt.models import BacktestResult
+from prosperity2bt.runner import run_backtest
 from typing import Any, Optional
 
-def parse_algorithm(algorithm: str) -> tuple[Any, Any]:
+def parse_algorithm(algorithm: str) -> Any:
     algorithm_path = Path(algorithm).expanduser().resolve()
 
     sys.path.append(str(algorithm_path.parent))
-    return import_module(algorithm_path.stem).Trader
+    return import_module(algorithm_path.stem)
+
+def parse_days(days: list[str], data_root: Optional[str]) -> list[BacktestData]:
+    if data_root is not None:
+        file_reader = FileSystemReader(Path(data_root).expanduser().resolve())
+    else:
+        file_reader = PackageResourcesReader()
 
-def parse_days(days: list[str], data_root: Optional[str]) -> list[DayData]:
     parsed_days = []
 
     if data_root is not None:
         data_root = Path(data_root).expanduser().resolve()
 
     for arg in days:
         if "-" in arg:
-            round, day = map(int, arg.split("-", 1))
-            parsed_days.append(read_day_data(data_root, round, day))
+            round_num, day_num = map(int, arg.split("-", 1))
+
+            day_data = read_day_data(file_reader, round_num, day_num)
+            if day_data is None:
+                print(f"Warning: no data found for round {round_num} day {day_num}")
+                continue
+
+            parsed_days.append(day_data)
         else:
-            round = int(arg)
-            parsed_days.extend(read_round_data(data_root, round))
+            round_num = int(arg)
+
+            parsed_days_in_round = []
+            for day_num in range(-5, 6):
+                day_data = read_day_data(file_reader, round_num, day_num)
+                if day_data is not None:
+                    parsed_days_in_round.append(day_data)
+
+            if len(parsed_days_in_round) == 0:
+                print(f"Warning: no data found for round {round_num}")
+                continue
+
+            parsed_days.extend(parsed_days_in_round)
 
     return parsed_days
 
 def parse_out(out: Optional[str]) -> Path:
     if out is not None:
         return Path(out).expanduser().resolve()
     else:
         timestamp = datetime.now().strftime("%Y-%m-%d_%H-%M-%S")
         return Path.cwd() / "backtests" / f"{timestamp}.log"
 
-def offset_sandbox_log_row(row: Any, timestamp_offset: int) -> Any:
-    old_timestamp = row["timestamp"]
-    new_timestamp = old_timestamp + timestamp_offset
+def print_day_summary(result: BacktestResult) -> None:
+    last_timestamp = result.activity_logs[-1].timestamp
+
+    product_lines = []
+    total_profit = 0
+
+    for row in reversed(result.activity_logs):
+        if row.timestamp != last_timestamp:
+            break
 
-    row["lambdaLog"] = row["lambdaLog"].replace(f"[[{old_timestamp},", f"[[{new_timestamp},")
-    row["timestamp"] += timestamp_offset
+        product = row.columns[2]
+        profit = row.columns[-1]
 
-    return row
+        product_lines.append(f"{product}: {profit:,.0f}")
+        total_profit += profit
 
-def offset_trade(trade: Any, timestamp_offset: int) -> Any:
-    trade["timestamp"] += timestamp_offset
-    return trade
+    print(*reversed(product_lines), sep="\n")
+    print(f"Total profit: {total_profit:,.0f}\n")
 
-def merge_results(a: DayResult, b: DayResult, merge_profit_loss: bool) -> DayResult:
+def merge_results(a: BacktestResult, b: BacktestResult, merge_profit_loss: bool) -> BacktestResult:
     sandbox_logs = a.sandbox_logs[:]
     activity_logs = a.activity_logs[:]
     trades = a.trades[:]
 
     a_last_timestamp = a.activity_logs[-1].timestamp
     timestamp_offset = a_last_timestamp + 100
 
-    sandbox_logs.extend([offset_sandbox_log_row(row, timestamp_offset) for row in b.sandbox_logs])
+    sandbox_logs.extend([row.with_offset(timestamp_offset) for row in b.sandbox_logs])
+    trades.extend([row.with_offset(timestamp_offset) for row in b.trades])
 
     if merge_profit_loss:
         profit_loss_offsets = defaultdict(float)
         for row in reversed(a.activity_logs):
             if row.timestamp != a_last_timestamp:
                 break
 
@@ -76,46 +105,46 @@
         activity_logs.extend([
             row.with_offset(timestamp_offset, profit_loss_offsets[row.columns[2]])
             for row in b.activity_logs
         ])
     else:
         activity_logs.extend([row.with_offset(timestamp_offset, 0) for row in b.activity_logs])
 
-    trades.extend([offset_trade(trade, timestamp_offset) for trade in b.trades])
+    return BacktestResult(a.round_num, a.day_num, sandbox_logs, activity_logs, trades)
 
-    return DayResult(a.round, a.day, sandbox_logs, activity_logs, trades)
-
-def write_output(output_file: Path, merged_results: DayResult) -> None:
+def write_output(output_file: Path, merged_results: BacktestResult) -> None:
     output_file.parent.mkdir(parents=True, exist_ok=True)
     with output_file.open("w+", encoding="utf-8") as file:
         file.write("Sandbox logs:\n")
-        file.write("\n".join(json.dumps(row, indent=2) for row in merged_results.sandbox_logs))
+        file.write("\n".join(map(str, merged_results.sandbox_logs)))
 
         file.write("\n\n\n\nActivities log:\n")
         file.write("day;timestamp;product;bid_price_1;bid_volume_1;bid_price_2;bid_volume_2;bid_price_3;bid_volume_3;ask_price_1;ask_volume_1;ask_price_2;ask_volume_2;ask_price_3;ask_volume_3;mid_price;profit_and_loss\n")
         file.write("\n".join(map(str, merged_results.activity_logs)))
 
         file.write("\n\n\n\n\nTrade History:\n")
-        file.write(json.dumps(merged_results.trades, cls=ProsperityEncoder, indent=2))
+        file.write("[\n")
+        file.write(",\n".join(map(str, merged_results.trades)))
+        file.write("]")
 
-def print_overall_summary(results: list[DayResult]) -> None:
+def print_overall_summary(results: list[BacktestResult]) -> None:
     print(f"Profit summary:")
 
     total_profit = 0
     for result in results:
         last_timestamp = result.activity_logs[-1].timestamp
 
         profit = 0
         for row in reversed(result.activity_logs):
             if row.timestamp != last_timestamp:
                 break
 
             profit += row.columns[-1]
 
-        print(f"Round {result.round} day {result.day}: {profit:,.0f}")
+        print(f"Round {result.round_num} day {result.day_num}: {profit:,.0f}")
         total_profit += profit
 
     print(f"Total profit: {total_profit:,.0f}\n")
 
 class HTTPRequestHandler(SimpleHTTPRequestHandler):
     def end_headers(self) -> None:
         self.send_header("Access-Control-Allow-Origin", "*")
@@ -149,19 +178,39 @@
     parser.add_argument("--data", type=str, help="path to data directory (must look similar in structure to https://github.com/jmerle/imc-prosperity-2-backtester/tree/master/prosperity2bt/resources)")
     parser.add_argument("--print", action="store_true", help="print the trader's output to stdout while it's running")
     parser.add_argument("--no-trades-matching", action="store_true", help="disable matching orders against market trades")
     parser.add_argument("-v", "--version", action="version", version=f"%(prog)s {metadata.version(__package__)}")
 
     args = parser.parse_args()
 
-    Trader = parse_algorithm(args.algorithm)
+    try:
+        trader_module = parse_algorithm(args.algorithm)
+    except ModuleNotFoundError:
+        print(f"{args.algorithm} is not a valid algorithm file")
+        sys.exit(1)
+
+    if not hasattr(trader_module, "Trader"):
+        print(f"{args.algorithm} does not expose a Trader class")
+        sys.exit(1)
+
     days = parse_days(args.days, args.data)
     output_file = parse_out(args.out)
 
-    results = [run_backtest(Trader(), day, args.print, args.no_trades_matching) for day in days]
+    results = []
+    for day in days:
+        print(f"Backtesting {args.algorithm} on round {day.round_num} day {day.day_num}")
+
+        reload(trader_module)
+        trader = trader_module.Trader()
+
+        result = run_backtest(trader, day, args.print, args.no_trades_matching)
+        print_day_summary(result)
+
+        results.append(result)
+
     merged_results = reduce(lambda a, b: merge_results(a, b, args.merge_pnl), results)
 
     write_output(output_file, merged_results)
 
     if len(days) > 1:
         print_overall_summary(results)
```

### Comparing `prosperity2bt-0.4.3/prosperity2bt/datamodel.py` & `prosperity2bt-0.4.4/prosperity2bt/datamodel.py`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.3/prosperity2bt/resources/round0/prices_round_0_day_-2.csv` & `prosperity2bt-0.4.4/prosperity2bt/resources/round0/prices_round_0_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.3/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv` & `prosperity2bt-0.4.4/prosperity2bt/resources/round0/trades_round_0_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.3/prosperity2bt/resources/round1/prices_round_1_day_-1.csv` & `prosperity2bt-0.4.4/prosperity2bt/resources/round1/prices_round_1_day_-1.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.3/prosperity2bt/resources/round1/prices_round_1_day_-2.csv` & `prosperity2bt-0.4.4/prosperity2bt/resources/round1/prices_round_1_day_-2.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.3/prosperity2bt/resources/round1/prices_round_1_day_0.csv` & `prosperity2bt-0.4.4/prosperity2bt/resources/round1/prices_round_1_day_0.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.3/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv` & `prosperity2bt-0.4.4/prosperity2bt/resources/round1/trades_round_1_day_-1_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.3/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv` & `prosperity2bt-0.4.4/prosperity2bt/resources/round1/trades_round_1_day_-2_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.3/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv` & `prosperity2bt-0.4.4/prosperity2bt/resources/round1/trades_round_1_day_0_nn.csv`

 * *Files identical despite different names*

### Comparing `prosperity2bt-0.4.3/prosperity2bt.egg-info/PKG-INFO` & `prosperity2bt-0.4.4/prosperity2bt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prosperity2bt
-Version: 0.4.3
+Version: 0.4.4
 Summary: Backtester for IMC Prosperity 2 algorithms
 Author-email: Jasper van Merle <jaspervmerle@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Jasper van Merle
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `prosperity2bt-0.4.3/prosperity2bt.egg-info/SOURCES.txt` & `prosperity2bt-0.4.4/prosperity2bt.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 LICENSE
 README.md
 pyproject.toml
 prosperity2bt/__init__.py
 prosperity2bt/__main__.py
-prosperity2bt/core.py
 prosperity2bt/data.py
 prosperity2bt/datamodel.py
+prosperity2bt/file_reader.py
+prosperity2bt/models.py
+prosperity2bt/runner.py
 prosperity2bt.egg-info/PKG-INFO
 prosperity2bt.egg-info/SOURCES.txt
 prosperity2bt.egg-info/dependency_links.txt
 prosperity2bt.egg-info/entry_points.txt
 prosperity2bt.egg-info/requires.txt
 prosperity2bt.egg-info/top_level.txt
 prosperity2bt/resources/__init__.py
```

### Comparing `prosperity2bt-0.4.3/pyproject.toml` & `prosperity2bt-0.4.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "prosperity2bt"
 description = "Backtester for IMC Prosperity 2 algorithms"
-version = "0.4.3"
+version = "0.4.4"
 readme = "README.md"
 license = {file = "LICENSE"}
 authors = [{name = "Jasper van Merle", email = "jaspervmerle@gmail.com"}]
 keywords = ["imc", "prosperity", "backtest", "backtester"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

