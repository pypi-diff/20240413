# Comparing `tmp/isbtchot-1.0.5.tar.gz` & `tmp/isbtchot-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isbtchot-1.0.5.tar", last modified: Tue Jan 30 22:09:37 2024, max compression
+gzip compressed data, was "isbtchot-1.1.0.tar", last modified: Sat Apr 13 10:49:43 2024, max compression
```

## Comparing `isbtchot-1.0.5.tar` & `isbtchot-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 22:09:37.278651 isbtchot-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-30 22:09:26.000000 isbtchot-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-01-30 22:09:37.278651 isbtchot-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-01-30 22:09:26.000000 isbtchot-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-01-30 22:09:26.000000 isbtchot-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-30 22:09:37.278651 isbtchot-1.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 22:09:37.278651 isbtchot-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 22:09:37.278651 isbtchot-1.0.5/src/isbtchot/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-01-30 22:09:26.000000 isbtchot-1.0.5/src/isbtchot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-01-30 22:09:26.000000 isbtchot-1.0.5/src/isbtchot/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-01-30 22:09:26.000000 isbtchot-1.0.5/src/isbtchot/controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-01-30 22:09:26.000000 isbtchot-1.0.5/src/isbtchot/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 22:09:37.278651 isbtchot-1.0.5/src/isbtchot/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-01-30 22:09:26.000000 isbtchot-1.0.5/src/isbtchot/schemas/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-01-30 22:09:26.000000 isbtchot-1.0.5/src/isbtchot/view.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-30 22:09:37.278651 isbtchot-1.0.5/src/isbtchot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-01-30 22:09:37.000000 isbtchot-1.0.5/src/isbtchot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-01-30 22:09:37.000000 isbtchot-1.0.5/src/isbtchot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-30 22:09:37.000000 isbtchot-1.0.5/src/isbtchot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-01-30 22:09:37.000000 isbtchot-1.0.5/src/isbtchot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-30 22:09:37.000000 isbtchot-1.0.5/src/isbtchot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:49:43.844064 isbtchot-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-13 10:49:36.000000 isbtchot-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-13 10:49:43.844064 isbtchot-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-04-13 10:49:36.000000 isbtchot-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-13 10:49:36.000000 isbtchot-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 10:49:43.844064 isbtchot-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:49:43.840064 isbtchot-1.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:49:43.840064 isbtchot-1.1.0/src/isbtchot/
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-13 10:49:36.000000 isbtchot-1.1.0/src/isbtchot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-13 10:49:36.000000 isbtchot-1.1.0/src/isbtchot/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2145 2024-04-13 10:49:36.000000 isbtchot-1.1.0/src/isbtchot/controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-13 10:49:36.000000 isbtchot-1.1.0/src/isbtchot/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:49:43.844064 isbtchot-1.1.0/src/isbtchot/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-13 10:49:36.000000 isbtchot-1.1.0/src/isbtchot/schemas/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-13 10:49:36.000000 isbtchot-1.1.0/src/isbtchot/view.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 10:49:43.844064 isbtchot-1.1.0/src/isbtchot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-13 10:49:43.000000 isbtchot-1.1.0/src/isbtchot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-13 10:49:43.000000 isbtchot-1.1.0/src/isbtchot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 10:49:43.000000 isbtchot-1.1.0/src/isbtchot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-13 10:49:43.000000 isbtchot-1.1.0/src/isbtchot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 10:49:43.000000 isbtchot-1.1.0/src/isbtchot.egg-info/top_level.txt
```

### Comparing `isbtchot-1.0.5/LICENSE` & `isbtchot-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `isbtchot-1.0.5/PKG-INFO` & `isbtchot-1.1.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,67 @@
 Metadata-Version: 2.1
 Name: isbtchot
-Version: 1.0.5
+Version: 1.1.0
 Summary: TBD
 Author-email: Daniel <dakixr@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: plotext
 Requires-Dist: requests
 
 # isbtchot: BTC Hotness Index Dashboard
 
-The `isbtchot` package provides a minimalist terminal dashboard for BTC's hotness index. It uses historical BTC data to create both BTC's price and Hotness Index visualizations right in your terminal.
-
-# Demo
-
-![BTC Hotness Index Dashboard Demo](media/demo.png)
+The `isbtchot` package provides a minimalist terminal dashboard for visualizing Bitcoin's (BTC) hotness index. It utilizes historical BTC data to generate visualizations of BTC's price alongside the Hotness Index, directly in your terminal.
 
 ## Features:
 
-- BTC monthly candlestick plot with log scale.
-- Hotness index based on PI with buy/sell signals.
-- Data is cached to speed up subsequent requests.
+- Visualizes BTC candlestick plots with log scale options.
+- Displays the Hotness Index based on proprietary indicators with buy/sell signals.
+- Supports different time frames and custom period back settings to tailor the data.
+- Offers multiple dashboard views including standard hotness index and power-law delta.
+- Data is cached locally to expedite subsequent visualizations.
 
 ## Installation
 
 ```bash
 pip install isbtchot
 ```
 
 ## Usage
 
-You can run the main dashboard with:
+You can run the main dashboard with flexible command-line options:
 
 ```bash
-isbtchot [-periods_back P] [-time T]
+isbtchot [--periods_back P] [--time T] [--dashboard D]
 ```
 
-- `-periods_back` or `--p`: Specifies the number of periods (e.g., weeks, months) of data you want to visualize. By default, it uses 85 periods.
-- `-time` or `--t`: Specifies the candlestick time to use (e.g., Daily, Weekly). By default, it uses Weekly.
+- `--periods_back`, `-p`: Specifies the number of periods back to process for generating the visualization. Defaults to 85.
+- `--time`, `-t`: Specifies the candlestick time frame (e.g., Weekly, Monthly). Defaults to Weekly.
+- `--dashboard`, `-d`: Choose the type of dashboard to display: `isbtchot` for the standard hotness index or `power_law` for the power-law distribution analysis. Defaults to `isbtchot`.
 
 ### Command Line Arguments
 
-| Argument        | Short Form | Description                                                | Default               |
-|-----------------|------------|------------------------------------------------------------|-----------------------|
-| `--periods_back`| `-p`       | Number of periods to be processed.                         | 85                    |
-| `--time`        | `-t`       | Candlestick time to use (e.g., D for Daily, W for Weekly). | W                     |
+| Argument       | Short Form | Description                                                                     | Default   |
+|----------------|------------|---------------------------------------------------------------------------------|-----------|
+| `--periods_back` | `-p`       | Number of periods to be processed for the data visualization.                    | 85        |
+| `--time`        | `-t`       | Candlestick time to use (e.g., ME for Monthly, W for Weekly).                   | W         |
+| `--dashboard`   | `-d`       | Dashboard type to display: `isbtchot` or `power_law`.                           | isbtchot  |
+
+## Demo
+
+### Hotness Index Dashboard
+Historically very reliable for bull market tops:
+![BTC Hotness Index Dashboard Demo](media/demo.png)
+
+### Power Law Delta Dashboard
+Historically very reliable for bull market bottoms:
+![BTC Power Law Delta Dashboard Demo](media/demo2.png)
 
 ## Notes
 
-- Ensure the terminal window is maximized for optimal visualization.
-- Data is fetched from CryptoCompare API and cached locally for performance.
+- For optimal visualization, maximize your terminal window.
+- Data is fetched from CryptoCompare API and cached to enhance performance and responsiveness.
 
 ## Contributions
 
-Please raise an issue or provide a pull request for any enhancements, bug fixes or features you'd like to add.
+Contributions are welcome! Please feel free to submit issues, enhancements, or pull requests. If you encounter a bug or have a feature suggestion, please open an issue on GitHub.
```

### Comparing `isbtchot-1.0.5/README.md` & `isbtchot-1.1.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,56 @@
 # isbtchot: BTC Hotness Index Dashboard
 
-The `isbtchot` package provides a minimalist terminal dashboard for BTC's hotness index. It uses historical BTC data to create both BTC's price and Hotness Index visualizations right in your terminal.
-
-# Demo
-
-![BTC Hotness Index Dashboard Demo](media/demo.png)
+The `isbtchot` package provides a minimalist terminal dashboard for visualizing Bitcoin's (BTC) hotness index. It utilizes historical BTC data to generate visualizations of BTC's price alongside the Hotness Index, directly in your terminal.
 
 ## Features:
 
-- BTC monthly candlestick plot with log scale.
-- Hotness index based on PI with buy/sell signals.
-- Data is cached to speed up subsequent requests.
+- Visualizes BTC candlestick plots with log scale options.
+- Displays the Hotness Index based on proprietary indicators with buy/sell signals.
+- Supports different time frames and custom period back settings to tailor the data.
+- Offers multiple dashboard views including standard hotness index and power-law delta.
+- Data is cached locally to expedite subsequent visualizations.
 
 ## Installation
 
 ```bash
 pip install isbtchot
 ```
 
 ## Usage
 
-You can run the main dashboard with:
+You can run the main dashboard with flexible command-line options:
 
 ```bash
-isbtchot [-periods_back P] [-time T]
+isbtchot [--periods_back P] [--time T] [--dashboard D]
 ```
 
-- `-periods_back` or `--p`: Specifies the number of periods (e.g., weeks, months) of data you want to visualize. By default, it uses 85 periods.
-- `-time` or `--t`: Specifies the candlestick time to use (e.g., Daily, Weekly). By default, it uses Weekly.
+- `--periods_back`, `-p`: Specifies the number of periods back to process for generating the visualization. Defaults to 85.
+- `--time`, `-t`: Specifies the candlestick time frame (e.g., Weekly, Monthly). Defaults to Weekly.
+- `--dashboard`, `-d`: Choose the type of dashboard to display: `isbtchot` for the standard hotness index or `power_law` for the power-law distribution analysis. Defaults to `isbtchot`.
 
 ### Command Line Arguments
 
-| Argument        | Short Form | Description                                                | Default               |
-|-----------------|------------|------------------------------------------------------------|-----------------------|
-| `--periods_back`| `-p`       | Number of periods to be processed.                         | 85                    |
-| `--time`        | `-t`       | Candlestick time to use (e.g., D for Daily, W for Weekly). | W                     |
+| Argument       | Short Form | Description                                                                     | Default   |
+|----------------|------------|---------------------------------------------------------------------------------|-----------|
+| `--periods_back` | `-p`       | Number of periods to be processed for the data visualization.                    | 85        |
+| `--time`        | `-t`       | Candlestick time to use (e.g., ME for Monthly, W for Weekly).                   | W         |
+| `--dashboard`   | `-d`       | Dashboard type to display: `isbtchot` or `power_law`.                           | isbtchot  |
+
+## Demo
+
+### Hotness Index Dashboard
+Historically very reliable for bull market tops:
+![BTC Hotness Index Dashboard Demo](media/demo.png)
+
+### Power Law Delta Dashboard
+Historically very reliable for bull market bottoms:
+![BTC Power Law Delta Dashboard Demo](media/demo2.png)
 
 ## Notes
 
-- Ensure the terminal window is maximized for optimal visualization.
-- Data is fetched from CryptoCompare API and cached locally for performance.
+- For optimal visualization, maximize your terminal window.
+- Data is fetched from CryptoCompare API and cached to enhance performance and responsiveness.
 
 ## Contributions
 
-Please raise an issue or provide a pull request for any enhancements, bug fixes or features you'd like to add.
+Contributions are welcome! Please feel free to submit issues, enhancements, or pull requests. If you encounter a bug or have a feature suggestion, please open an issue on GitHub.
```

### Comparing `isbtchot-1.0.5/src/isbtchot/__main__.py` & `isbtchot-1.1.0/src/isbtchot/__main__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,52 @@
 from isbtchot import controller
 from isbtchot.schemas.args import TypeTime
 import argparse
 
 parser = argparse.ArgumentParser(description="BTC Hotness Index", prog="isbtchot")
 
-# Add an optional positional argument named 'year' with default value of 6
 parser.add_argument(
     "-p",
     "--periods_back",
     type=int,
     default=85,
-    help="Periods back to be processed. Defaults to 50 if not provided.",
+    help="Periods back to be processed. Defaults to 85 if not provided.",
 )
 
 parser.add_argument(
     "-t",
     "--time",
     type=TypeTime,
     default=TypeTime.WEEK,
-    help="Candle stick time to use. Defaults to W (Weekly),"
+    help="Candle stick time to use: ME or W. Defaults to W (Weekly)",
+)
+
+parser.add_argument(
+    "-d",
+    "--dashboard",
+    type=str,
+    default="isbtchot",
+    help="Dashboard to display: 'isbtchot' or 'power_law'. Defaults to 'isbtchot'.",
 )
 
 
 def main():
 
     # Parse args
     args = parser.parse_args()
     time_grouping: TypeTime = args.time
     periods_back: int = args.periods_back
+    dashboard: str = args.dashboard
 
-    controller.dashboard(periods_back=periods_back, time_grouping=time_grouping)
+    if dashboard == "isbtchot":
+        controller.dashboard_isbtchot(
+            periods_back=periods_back, time_grouping=time_grouping
+        )
+    elif dashboard == "power_law":
+        controller.dashboard_power_law(
+            periods_back=periods_back, time_grouping=time_grouping
+        )
+    else:
+        raise ValueError(f"Unknown dashboard: '{dashboard}'. Expected 'isbtchot' or 'power_law'.")
 
 if __name__ == "__main__":
-    main()
+    main()
```

### Comparing `isbtchot-1.0.5/src/isbtchot/view.py` & `isbtchot-1.1.0/src/isbtchot/view.py`

 * *Files identical despite different names*

### Comparing `isbtchot-1.0.5/src/isbtchot.egg-info/PKG-INFO` & `isbtchot-1.1.0/src/isbtchot.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,57 +1,67 @@
 Metadata-Version: 2.1
 Name: isbtchot
-Version: 1.0.5
+Version: 1.1.0
 Summary: TBD
 Author-email: Daniel <dakixr@gmail.com>
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pandas
 Requires-Dist: plotext
 Requires-Dist: requests
 
 # isbtchot: BTC Hotness Index Dashboard
 
-The `isbtchot` package provides a minimalist terminal dashboard for BTC's hotness index. It uses historical BTC data to create both BTC's price and Hotness Index visualizations right in your terminal.
-
-# Demo
-
-![BTC Hotness Index Dashboard Demo](media/demo.png)
+The `isbtchot` package provides a minimalist terminal dashboard for visualizing Bitcoin's (BTC) hotness index. It utilizes historical BTC data to generate visualizations of BTC's price alongside the Hotness Index, directly in your terminal.
 
 ## Features:
 
-- BTC monthly candlestick plot with log scale.
-- Hotness index based on PI with buy/sell signals.
-- Data is cached to speed up subsequent requests.
+- Visualizes BTC candlestick plots with log scale options.
+- Displays the Hotness Index based on proprietary indicators with buy/sell signals.
+- Supports different time frames and custom period back settings to tailor the data.
+- Offers multiple dashboard views including standard hotness index and power-law delta.
+- Data is cached locally to expedite subsequent visualizations.
 
 ## Installation
 
 ```bash
 pip install isbtchot
 ```
 
 ## Usage
 
-You can run the main dashboard with:
+You can run the main dashboard with flexible command-line options:
 
 ```bash
-isbtchot [-periods_back P] [-time T]
+isbtchot [--periods_back P] [--time T] [--dashboard D]
 ```
 
-- `-periods_back` or `--p`: Specifies the number of periods (e.g., weeks, months) of data you want to visualize. By default, it uses 85 periods.
-- `-time` or `--t`: Specifies the candlestick time to use (e.g., Daily, Weekly). By default, it uses Weekly.
+- `--periods_back`, `-p`: Specifies the number of periods back to process for generating the visualization. Defaults to 85.
+- `--time`, `-t`: Specifies the candlestick time frame (e.g., Weekly, Monthly). Defaults to Weekly.
+- `--dashboard`, `-d`: Choose the type of dashboard to display: `isbtchot` for the standard hotness index or `power_law` for the power-law distribution analysis. Defaults to `isbtchot`.
 
 ### Command Line Arguments
 
-| Argument        | Short Form | Description                                                | Default               |
-|-----------------|------------|------------------------------------------------------------|-----------------------|
-| `--periods_back`| `-p`       | Number of periods to be processed.                         | 85                    |
-| `--time`        | `-t`       | Candlestick time to use (e.g., D for Daily, W for Weekly). | W                     |
+| Argument       | Short Form | Description                                                                     | Default   |
+|----------------|------------|---------------------------------------------------------------------------------|-----------|
+| `--periods_back` | `-p`       | Number of periods to be processed for the data visualization.                    | 85        |
+| `--time`        | `-t`       | Candlestick time to use (e.g., ME for Monthly, W for Weekly).                   | W         |
+| `--dashboard`   | `-d`       | Dashboard type to display: `isbtchot` or `power_law`.                           | isbtchot  |
+
+## Demo
+
+### Hotness Index Dashboard
+Historically very reliable for bull market tops:
+![BTC Hotness Index Dashboard Demo](media/demo.png)
+
+### Power Law Delta Dashboard
+Historically very reliable for bull market bottoms:
+![BTC Power Law Delta Dashboard Demo](media/demo2.png)
 
 ## Notes
 
-- Ensure the terminal window is maximized for optimal visualization.
-- Data is fetched from CryptoCompare API and cached locally for performance.
+- For optimal visualization, maximize your terminal window.
+- Data is fetched from CryptoCompare API and cached to enhance performance and responsiveness.
 
 ## Contributions
 
-Please raise an issue or provide a pull request for any enhancements, bug fixes or features you'd like to add.
+Contributions are welcome! Please feel free to submit issues, enhancements, or pull requests. If you encounter a bug or have a feature suggestion, please open an issue on GitHub.
```

