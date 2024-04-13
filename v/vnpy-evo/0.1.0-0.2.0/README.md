# Comparing `tmp/vnpy_evo-0.1.0.tar.gz` & `tmp/vnpy_evo-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnpy_evo-0.1.0.tar", last modified: Mon Mar 11 11:35:10 2024, max compression
+gzip compressed data, was "vnpy_evo-0.2.0.tar", last modified: Sat Apr 13 06:10:07 2024, max compression
```

## Comparing `vnpy_evo-0.1.0.tar` & `vnpy_evo-0.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-03-11 11:35:10.120886 vnpy_evo-0.1.0/
--rw-rw-rw-   0        0        0     1109 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       30 2024-03-10 12:14:20.000000 vnpy_evo-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0    11306 2024-03-11 11:35:10.121882 vnpy_evo-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0    10228 2024-03-11 11:19:35.000000 vnpy_evo-0.1.0/README.md
--rw-rw-rw-   0        0        0     1251 2024-03-11 11:35:10.128906 vnpy_evo-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0       43 2024-03-05 02:02:42.000000 vnpy_evo-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:35:10.078275 vnpy_evo-0.1.0/vnpy_evo/
--rw-rw-rw-   0        0        0     1172 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:35:10.098830 vnpy_evo-0.1.0/vnpy_evo/chart/
--rw-rw-rw-   0        0        0       26 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/chart/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:35:10.099802 vnpy_evo-0.1.0/vnpy_evo/event/
--rw-rw-rw-   0        0        0       26 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/event/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:35:10.100812 vnpy_evo-0.1.0/vnpy_evo/rpc/
--rw-rw-rw-   0        0        0       22 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/rpc/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:35:10.110804 vnpy_evo-0.1.0/vnpy_evo/trader/
--rw-rw-rw-   0        0        0        0 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/trader/__init__.py
--rw-rw-rw-   0        0        0       31 2024-03-08 07:51:09.000000 vnpy_evo-0.1.0/vnpy_evo/trader/app.py
--rw-rw-rw-   0        0        0      426 2024-03-08 07:51:03.000000 vnpy_evo-0.1.0/vnpy_evo/trader/constant.py
--rw-rw-rw-   0        0        0       37 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/trader/converter.py
--rw-rw-rw-   0        0        0       36 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/trader/database.py
--rw-rw-rw-   0        0        0       36 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/trader/datafeed.py
--rw-rw-rw-   0        0        0       34 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/trader/engine.py
--rw-rw-rw-   0        0        0       33 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/trader/event.py
--rw-rw-rw-   0        0        0       35 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/trader/gateway.py
--rw-rw-rw-   0        0        0       34 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/trader/object.py
--rw-rw-rw-   0        0        0       36 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/trader/optimize.py
--rw-rw-rw-   0        0        0       35 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/trader/setting.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:35:10.116871 vnpy_evo-0.1.0/vnpy_evo/trader/ui/
--rw-rw-rw-   0        0        0       95 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/trader/ui/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:35:10.118878 vnpy_evo-0.1.0/vnpy_evo/trader/ui/ico/
--rw-rw-rw-   0        0        0        0 2024-03-11 11:13:46.000000 vnpy_evo-0.1.0/vnpy_evo/trader/ui/ico/__init__.py
--rw-rw-rw-   0        0        0    35149 2022-05-31 14:57:28.000000 vnpy_evo-0.1.0/vnpy_evo/trader/ui/ico/veighna.ico
--rw-rw-rw-   0        0        0     7955 2024-03-11 11:19:39.000000 vnpy_evo-0.1.0/vnpy_evo/trader/ui/mainwindow.py
--rw-rw-rw-   0        0        0    22851 2024-03-08 08:00:11.000000 vnpy_evo-0.1.0/vnpy_evo/trader/ui/monitor.py
--rw-rw-rw-   0        0        0     3960 2024-03-11 11:19:42.000000 vnpy_evo-0.1.0/vnpy_evo/trader/ui/qt.py
--rw-rw-rw-   0        0        0    23192 2024-03-11 11:20:14.000000 vnpy_evo-0.1.0/vnpy_evo/trader/ui/widget.py
--rw-rw-rw-   0        0        0       35 2024-03-06 03:15:52.000000 vnpy_evo-0.1.0/vnpy_evo/trader/utility.py
-drwxrwxrwx   0        0        0        0 2024-03-11 11:35:10.097807 vnpy_evo-0.1.0/vnpy_evo.egg-info/
--rw-rw-rw-   0        0        0    11306 2024-03-11 11:35:09.000000 vnpy_evo-0.1.0/vnpy_evo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      906 2024-03-11 11:35:10.000000 vnpy_evo-0.1.0/vnpy_evo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-11 11:35:09.000000 vnpy_evo-0.1.0/vnpy_evo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-11 11:34:45.000000 vnpy_evo-0.1.0/vnpy_evo.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       28 2024-03-11 11:35:09.000000 vnpy_evo-0.1.0/vnpy_evo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-03-11 11:35:09.000000 vnpy_evo-0.1.0/vnpy_evo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.070781 vnpy_evo-0.2.0/
+-rw-rw-rw-   0        0        0     1109 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       30 2024-03-10 12:14:20.000000 vnpy_evo-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    11325 2024-04-13 06:10:07.070781 vnpy_evo-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    10247 2024-04-13 06:07:39.000000 vnpy_evo-0.2.0/README.md
+-rw-rw-rw-   0        0        0     1251 2024-04-13 06:10:07.072789 vnpy_evo-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0       43 2024-03-05 02:02:42.000000 vnpy_evo-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.009396 vnpy_evo-0.2.0/vnpy_evo/
+-rw-rw-rw-   0        0        0     1241 2024-04-13 06:06:30.000000 vnpy_evo-0.2.0/vnpy_evo/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.026934 vnpy_evo-0.2.0/vnpy_evo/chart/
+-rw-rw-rw-   0        0        0       26 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/chart/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.027943 vnpy_evo-0.2.0/vnpy_evo/event/
+-rw-rw-rw-   0        0        0       26 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/event/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.046401 vnpy_evo-0.2.0/vnpy_evo/rpc/
+-rw-rw-rw-   0        0        0       22 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/rpc/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.061091 vnpy_evo-0.2.0/vnpy_evo/trader/
+-rw-rw-rw-   0        0        0        0 2024-03-18 09:46:57.000000 vnpy_evo-0.2.0/vnpy_evo/trader/__init__.py
+-rw-rw-rw-   0        0        0       31 2024-03-08 07:51:09.000000 vnpy_evo-0.2.0/vnpy_evo/trader/app.py
+-rw-rw-rw-   0        0        0      459 2024-04-06 05:51:44.000000 vnpy_evo-0.2.0/vnpy_evo/trader/constant.py
+-rw-rw-rw-   0        0        0       37 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/converter.py
+-rw-rw-rw-   0        0        0       36 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/database.py
+-rw-rw-rw-   0        0        0       36 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/datafeed.py
+-rw-rw-rw-   0        0        0       34 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/engine.py
+-rw-rw-rw-   0        0        0       33 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/event.py
+-rw-rw-rw-   0        0        0       35 2024-04-06 05:51:44.000000 vnpy_evo-0.2.0/vnpy_evo/trader/gateway.py
+-rw-rw-rw-   0        0        0       34 2024-04-06 05:51:44.000000 vnpy_evo-0.2.0/vnpy_evo/trader/object.py
+-rw-rw-rw-   0        0        0       36 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/optimize.py
+-rw-rw-rw-   0        0        0       35 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/setting.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.065788 vnpy_evo-0.2.0/vnpy_evo/trader/ui/
+-rw-rw-rw-   0        0        0       95 2024-03-18 09:46:51.000000 vnpy_evo-0.2.0/vnpy_evo/trader/ui/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.069785 vnpy_evo-0.2.0/vnpy_evo/trader/ui/ico/
+-rw-rw-rw-   0        0        0        0 2024-03-11 11:13:46.000000 vnpy_evo-0.2.0/vnpy_evo/trader/ui/ico/__init__.py
+-rw-rw-rw-   0        0        0    35149 2022-05-31 14:57:28.000000 vnpy_evo-0.2.0/vnpy_evo/trader/ui/ico/veighna.ico
+-rw-rw-rw-   0        0        0     7951 2024-03-18 09:40:05.000000 vnpy_evo-0.2.0/vnpy_evo/trader/ui/mainwindow.py
+-rw-rw-rw-   0        0        0    22875 2024-04-05 09:48:27.000000 vnpy_evo-0.2.0/vnpy_evo/trader/ui/monitor.py
+-rw-rw-rw-   0        0        0     3960 2024-03-18 09:49:02.000000 vnpy_evo-0.2.0/vnpy_evo/trader/ui/qt.py
+-rw-rw-rw-   0        0        0    23194 2024-03-18 09:48:54.000000 vnpy_evo-0.2.0/vnpy_evo/trader/ui/widget.py
+-rw-rw-rw-   0        0        0       35 2024-03-06 03:15:52.000000 vnpy_evo-0.2.0/vnpy_evo/trader/utility.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:10:07.025938 vnpy_evo-0.2.0/vnpy_evo.egg-info/
+-rw-rw-rw-   0        0        0    11325 2024-04-13 06:10:06.000000 vnpy_evo-0.2.0/vnpy_evo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      906 2024-04-13 06:10:06.000000 vnpy_evo-0.2.0/vnpy_evo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 06:10:06.000000 vnpy_evo-0.2.0/vnpy_evo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-04-13 06:10:06.000000 vnpy_evo-0.2.0/vnpy_evo.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       28 2024-04-13 06:10:06.000000 vnpy_evo-0.2.0/vnpy_evo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-04-13 06:10:06.000000 vnpy_evo-0.2.0/vnpy_evo.egg-info/top_level.txt
```

### Comparing `vnpy_evo-0.1.0/LICENSE` & `vnpy_evo-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vnpy_evo-0.1.0/PKG-INFO` & `vnpy_evo-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy_evo
-Version: 0.1.0
+Version: 0.2.0
 Summary: Core module for using VeighNa project on crypto markets.
 Home-page: https://www.github.com/veighna-global
 Author: VeighNa Global
 Author-email: veighna@hotmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/veighna-global/vnpy_evo
 Keywords: quant,quantitative,investment,trading,algotrading,crypto,btc
@@ -26,17 +26,17 @@
 # By Traders, For Traders.
 
 <p align="center">
   <img src ="https://github.com/veighna-global/vnpy_evo/blob/dev/logo.png" width="300" height="300"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-0.1.0-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-0.2.0-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg"/>
     <img src ="https://img.shields.io/github/license/veighna-global/vnpy_evo.svg?color=orange"/>
 </p>
 
 VeighNa Evo (vnpy_evo) is the core module for using [VeighNa (vnpy)](https://github.com/vnpy/vnpy) quant trading platform on the crypto market. 
 
 ## Social
 
@@ -53,17 +53,19 @@
 
     * Crypto Market
 
         * Binance ([binance](https://www.github.com/veighna-global/vnpy_binance)): Spot/Perpetual/Futures/Option
 
         * OKX ([okx](https://www.github.com/veighna-global/vnpy_okx)): Spot/Perpetual/Futures/Option
 
-        * Bybit ([bybit](https://www.github.com/veighna-global/vnpy_bybit)): Spot/Perpetual/Futures
+        * Bybit ([bybit](https://www.github.com/veighna-global/vnpy_bybit)): Spot/Perpetual/Futures/Option
 
-        * Deribit ([deribit](https://www.github.com/veighna-global/vnpy_deribit)): Perpetual/Futures/Option
+    * Forex Market
+
+        * MT5 ([mt5](https://www.github.com/veighna-global/vnpy_mt5)): Forex/Gold/Commodity/Crypto
 
     * Special Applications
 
         * RPC service ([rpc](https://www.github.com/vnpy/vnpy_rpcservice)): inter-process communication interface for distributed architecture
 
 3. Applications for various quantitative strategies (vnpy_evo.app).
```

### Comparing `vnpy_evo-0.1.0/README.md` & `vnpy_evo-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # By Traders, For Traders.
 
 <p align="center">
   <img src ="https://github.com/veighna-global/vnpy_evo/blob/dev/logo.png" width="300" height="300"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-0.1.0-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-0.2.0-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg"/>
     <img src ="https://img.shields.io/github/license/veighna-global/vnpy_evo.svg?color=orange"/>
 </p>
 
 VeighNa Evo (vnpy_evo) is the core module for using [VeighNa (vnpy)](https://github.com/vnpy/vnpy) quant trading platform on the crypto market. 
 
 ## Social
 
@@ -28,17 +28,19 @@
 
     * Crypto Market
 
         * Binance ([binance](https://www.github.com/veighna-global/vnpy_binance)): Spot/Perpetual/Futures/Option
 
         * OKX ([okx](https://www.github.com/veighna-global/vnpy_okx)): Spot/Perpetual/Futures/Option
 
-        * Bybit ([bybit](https://www.github.com/veighna-global/vnpy_bybit)): Spot/Perpetual/Futures
+        * Bybit ([bybit](https://www.github.com/veighna-global/vnpy_bybit)): Spot/Perpetual/Futures/Option
 
-        * Deribit ([deribit](https://www.github.com/veighna-global/vnpy_deribit)): Perpetual/Futures/Option
+    * Forex Market
+
+        * MT5 ([mt5](https://www.github.com/veighna-global/vnpy_mt5)): Forex/Gold/Commodity/Crypto
 
     * Special Applications
 
         * RPC service ([rpc](https://www.github.com/vnpy/vnpy_rpcservice)): inter-process communication interface for distributed architecture
 
 3. Applications for various quantitative strategies (vnpy_evo.app).
```

### Comparing `vnpy_evo-0.1.0/setup.cfg` & `vnpy_evo-0.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `vnpy_evo-0.1.0/vnpy_evo/__init__.py` & `vnpy_evo-0.2.0/vnpy_evo/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,9 +16,12 @@
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 
+import os
+os.environ["LANG"] = "en"       # Only support English
 
-__version__ = "0.1.0"
+
+__version__ = "0.2.0"
```

### Comparing `vnpy_evo-0.1.0/vnpy_evo/trader/ui/ico/veighna.ico` & `vnpy_evo-0.2.0/vnpy_evo/trader/ui/ico/veighna.ico`

 * *Files identical despite different names*

### Comparing `vnpy_evo-0.1.0/vnpy_evo/trader/ui/mainwindow.py` & `vnpy_evo-0.2.0/vnpy_evo/trader/ui/mainwindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     FluentWindow, MessageBox,
     FluentIcon as FIF,
     PushButton, RoundMenu,
     Action, NavigationItemPosition,
 )
 
 from vnpy.event import EventEngine
-from vnpy.trader.locale import _
 
 import vnpy_evo
 from .qt import QtCore, QtGui, QtWidgets
 from .widget import (
     ConnectDialog,
     TradingWidget,
     AboutDialog,
@@ -187,27 +186,27 @@
         self.trade_monitor = TradeMonitor(self.main_engine, self.event_engine)
         self.position_monitor = PositionMonitor(self.main_engine, self.event_engine)
         self.account_monitor = AccountMonitor(self.main_engine, self.event_engine)
         self.log_monitor = LogMonitor(self.main_engine, self.event_engine)
 
         self.menu: RoundMenu = RoundMenu(parent=self)
 
-        self.menu_button: PushButton = PushButton("System")
+        self.menu_button: PushButton = PushButton("Connect Gateway")
         self.menu_button.clicked.connect(self.show_menu)
 
         # Set layout
         mid_pivot = PivotWidgdet(self)
-        mid_pivot.add_widget(self.active_monitor, "Active")
-        mid_pivot.add_widget(self.order_monitor, "Order")
+        mid_pivot.add_widget(self.active_monitor, "Open Orders")
+        mid_pivot.add_widget(self.order_monitor, "Order History")
 
         bottom_pivot = PivotWidgdet(self)
         bottom_pivot.add_widget(self.log_monitor, "Log")
-        bottom_pivot.add_widget(self.trade_monitor, "Trade")
-        bottom_pivot.add_widget(self.position_monitor, "Position")
-        bottom_pivot.add_widget(self.account_monitor, "Account")
+        bottom_pivot.add_widget(self.trade_monitor, "Trade History")
+        bottom_pivot.add_widget(self.position_monitor, "Positions")
+        bottom_pivot.add_widget(self.account_monitor, "Assets")
 
         vbox1 = QtWidgets.QVBoxLayout()
         vbox1.addWidget(self.tick_monitor)
         vbox1.addWidget(mid_pivot)
         vbox1.addWidget(bottom_pivot)
 
         vbox2 = QtWidgets.QVBoxLayout()
```

### Comparing `vnpy_evo-0.1.0/vnpy_evo/trader/ui/monitor.py` & `vnpy_evo-0.2.0/vnpy_evo/trader/ui/monitor.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         """
         self.setColumnCount(len(self.headers))
 
         labels: list = [d["display"] for d in self.headers.values()]
         self.setHorizontalHeaderLabels(labels)
 
         self.verticalHeader().setVisible(False)
-        self.setEditTriggers(self.NoEditTriggers)
+        self.setEditTriggers(self.EditTrigger.NoEditTriggers)
         self.setAlternatingRowColors(True)
         self.setSortingEnabled(self.sorting)
 
     def init_menu(self) -> None:
         """
         Create right click menu.
         """
@@ -641,15 +641,15 @@
             label: str = f"{display}\n{name}"
             labels.append(label)
 
         self.contract_table: TableWidget = TableWidget()
         self.contract_table.setColumnCount(len(self.headers))
         self.contract_table.setHorizontalHeaderLabels(labels)
         self.contract_table.verticalHeader().setVisible(False)
-        self.contract_table.setEditTriggers(self.contract_table.NoEditTriggers)
+        self.contract_table.setEditTriggers(self.contract_table.EditTrigger.NoEditTriggers)
         self.contract_table.setAlternatingRowColors(True)
 
         hbox: QtWidgets.QHBoxLayout = QtWidgets.QHBoxLayout()
         hbox.addWidget(self.filter_line)
         hbox.addWidget(self.button_show)
 
         vbox: QtWidgets.QVBoxLayout = QtWidgets.QVBoxLayout()
```

### Comparing `vnpy_evo-0.1.0/vnpy_evo/trader/ui/qt.py` & `vnpy_evo-0.2.0/vnpy_evo/trader/ui/qt.py`

 * *Files identical despite different names*

### Comparing `vnpy_evo-0.1.0/vnpy_evo/trader/ui/widget.py` & `vnpy_evo-0.2.0/vnpy_evo/trader/ui/widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -184,18 +184,18 @@
 
         self.gateway_combo: ComboBox = ComboBox()
         self.gateway_combo.addItems(self.main_engine.get_all_gateway_names())
 
         self.price_check: CheckBox = CheckBox()
         self.price_check.setToolTip(_("设置价格随行情更新"))
 
-        send_button: PushButton = PushButton(_("委托"))
+        send_button: PushButton = PushButton("Send Order")
         send_button.clicked.connect(self.send_order)
 
-        cancel_button: PushButton = PushButton(_("全撤"))
+        cancel_button: PushButton = PushButton("Cancel All")
         cancel_button.clicked.connect(self.cancel_all)
 
         grid: QtWidgets.QGridLayout = QtWidgets.QGridLayout()
         grid.addWidget(BodyLabel(_("交易所")), 0, 0)
         grid.addWidget(BodyLabel(_("代码")), 1, 0)
         grid.addWidget(BodyLabel(_("名称")), 2, 0)
         grid.addWidget(BodyLabel(_("方向")), 3, 0)
```

### Comparing `vnpy_evo-0.1.0/vnpy_evo.egg-info/PKG-INFO` & `vnpy_evo-0.2.0/vnpy_evo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnpy-evo
-Version: 0.1.0
+Version: 0.2.0
 Summary: Core module for using VeighNa project on crypto markets.
 Home-page: https://www.github.com/veighna-global
 Author: VeighNa Global
 Author-email: veighna@hotmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/veighna-global/vnpy_evo
 Keywords: quant,quantitative,investment,trading,algotrading,crypto,btc
@@ -26,17 +26,17 @@
 # By Traders, For Traders.
 
 <p align="center">
   <img src ="https://github.com/veighna-global/vnpy_evo/blob/dev/logo.png" width="300" height="300"/>
 </p>
 
 <p align="center">
-    <img src ="https://img.shields.io/badge/version-0.1.0-blueviolet.svg"/>
+    <img src ="https://img.shields.io/badge/version-0.2.0-blueviolet.svg"/>
     <img src ="https://img.shields.io/badge/platform-windows|linux|macos-yellow.svg"/>
-    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg" />
+    <img src ="https://img.shields.io/badge/python-3.10|3.11|3.12-blue.svg"/>
     <img src ="https://img.shields.io/github/license/veighna-global/vnpy_evo.svg?color=orange"/>
 </p>
 
 VeighNa Evo (vnpy_evo) is the core module for using [VeighNa (vnpy)](https://github.com/vnpy/vnpy) quant trading platform on the crypto market. 
 
 ## Social
 
@@ -53,17 +53,19 @@
 
     * Crypto Market
 
         * Binance ([binance](https://www.github.com/veighna-global/vnpy_binance)): Spot/Perpetual/Futures/Option
 
         * OKX ([okx](https://www.github.com/veighna-global/vnpy_okx)): Spot/Perpetual/Futures/Option
 
-        * Bybit ([bybit](https://www.github.com/veighna-global/vnpy_bybit)): Spot/Perpetual/Futures
+        * Bybit ([bybit](https://www.github.com/veighna-global/vnpy_bybit)): Spot/Perpetual/Futures/Option
 
-        * Deribit ([deribit](https://www.github.com/veighna-global/vnpy_deribit)): Perpetual/Futures/Option
+    * Forex Market
+
+        * MT5 ([mt5](https://www.github.com/veighna-global/vnpy_mt5)): Forex/Gold/Commodity/Crypto
 
     * Special Applications
 
         * RPC service ([rpc](https://www.github.com/vnpy/vnpy_rpcservice)): inter-process communication interface for distributed architecture
 
 3. Applications for various quantitative strategies (vnpy_evo.app).
```

### Comparing `vnpy_evo-0.1.0/vnpy_evo.egg-info/SOURCES.txt` & `vnpy_evo-0.2.0/vnpy_evo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

