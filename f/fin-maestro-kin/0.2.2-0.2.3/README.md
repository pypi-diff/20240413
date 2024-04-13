# Comparing `tmp/fin_maestro_kin-0.2.2.tar.gz` & `tmp/fin_maestro_kin-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fin_maestro_kin-0.2.2.tar", max compression
+gzip compressed data, was "fin_maestro_kin-0.2.3.tar", max compression
```

## Comparing `fin_maestro_kin-0.2.2.tar` & `fin_maestro_kin-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,21 @@
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.2/fin_maestro_kin/__init__.py
--rw-r--r--   0        0        0     1518 2024-04-07 12:51:01.798236 fin_maestro_kin-0.2.2/fin_maestro_kin/constants.py
--rw-r--r--   0        0        0      545 2024-03-09 11:03:03.068361 fin_maestro_kin-0.2.2/fin_maestro_kin/main.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/__init__.py
--rw-r--r--   0        0        0       18 2024-03-31 06:15:52.175723 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/__init__.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/nse/__init__.py
--rw-r--r--   0        0        0    12664 2024-04-07 13:52:02.139544 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/nse/helper.py
--rw-r--r--   0        0        0    18970 2024-04-07 12:51:02.233160 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py
--rw-r--r--   0        0        0     7634 2024-04-07 13:52:15.430589 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/sentiment_analysis/__init__.py
--rw-r--r--   0        0        0     1563 2024-02-10 16:25:56.398293 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py
--rw-r--r--   0        0        0     2109 2024-02-25 06:17:29.811861 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py
--rw-r--r--   0        0        0        0 2024-02-10 15:38:47.413185 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/trend_detector/__init__.py
--rw-r--r--   0        0        0     2074 2024-02-25 06:17:29.827487 fin_maestro_kin-0.2.2/fin_maestro_kin/modules/trend_detector/trend_detector.py
--rw-r--r--   0        0        0     1090 2024-02-10 16:19:33.663653 fin_maestro_kin-0.2.2/LICENSE
--rw-r--r--   0        0        0      614 2024-04-07 13:53:15.823782 fin_maestro_kin-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     5339 2024-03-31 06:18:04.202217 fin_maestro_kin-0.2.2/README.md
--rw-r--r--   0        0        0     6179 1970-01-01 00:00:00.000000 fin_maestro_kin-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.3/fin_maestro_kin/__init__.py
+-rw-r--r--   0        0        0     1606 2024-04-12 20:53:43.495343 fin_maestro_kin-0.2.3/fin_maestro_kin/constants.py
+-rw-r--r--   0        0        0      675 2024-04-12 19:12:33.740169 fin_maestro_kin-0.2.3/fin_maestro_kin/main.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/__init__.py
+-rw-r--r--   0        0        0       18 2024-03-31 06:15:52.175723 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/nse/__init__.py
+-rw-r--r--   0        0        0    12569 2024-04-12 20:19:01.630418 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/nse/helper.py
+-rw-r--r--   0        0        0    19034 2024-04-12 20:25:36.577477 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py
+-rw-r--r--   0        0        0     7634 2024-04-07 13:52:15.430589 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py
+-rw-r--r--   0        0        0        0 2024-04-12 15:03:25.791170 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/screener/__init__.py
+-rw-r--r--   0        0        0      514 2024-04-12 20:45:58.837209 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/screener/helper.py
+-rw-r--r--   0        0        0     1865 2024-04-12 20:45:18.468552 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/screener/screener_equities.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.381919 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/sentiment_analysis/__init__.py
+-rw-r--r--   0        0        0     1563 2024-02-10 16:25:56.398293 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py
+-rw-r--r--   0        0        0     2109 2024-02-25 06:17:29.811861 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py
+-rw-r--r--   0        0        0        0 2024-02-10 15:38:47.413185 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/trend_detector/__init__.py
+-rw-r--r--   0        0        0     2074 2024-02-25 06:17:29.827487 fin_maestro_kin-0.2.3/fin_maestro_kin/modules/trend_detector/trend_detector.py
+-rw-r--r--   0        0        0     1090 2024-02-10 16:19:33.663653 fin_maestro_kin-0.2.3/LICENSE
+-rw-r--r--   0        0        0      642 2024-04-13 06:33:03.660401 fin_maestro_kin-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     5339 2024-03-31 06:18:04.202217 fin_maestro_kin-0.2.3/README.md
+-rw-r--r--   0        0        0     6227 1970-01-01 00:00:00.000000 fin_maestro_kin-0.2.3/PKG-INFO
```

### Comparing `fin_maestro_kin-0.2.2/fin_maestro_kin/constants.py` & `fin_maestro_kin-0.2.3/fin_maestro_kin/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 ENDPOINTS = [
-    '/equities/security-archives?symbol=TCS&start_date=04-01-2024&end_date=14-01-2024&series=ALL',
-    '/equities/bulk-deals-archives?start_date=28-01-2024&end_date=04-02-2024',
-    '/equities/block-deals-archives?start_date=28-01-2024&end_date=04-02-2024',
-    '/equities/short-selling-archives?start_date=28-01-2024&end_date=04-02-2024',
-    '/equities/corporate-actions?start_date=28-01-2024&end_date=04-02-2024',
+    '/equities/security-archives?symbol=TCS&start_date=04-01-2024&end_date=07-01-2024&series=ALL',
+    '/equities/bulk-deals-archives?start_date=28-01-2024&end_date=01-02-2024',
+    '/equities/block-deals-archives?start_date=28-01-2024&end_date=01-02-2024',
+    '/equities/short-selling-archives?start_date=28-01-2024&end_date=01-02-2024',
+    '/equities/corporate-actions?start_date=28-01-2024&end_date=01-02-2024',
     '/equities/most-active-securities',
     '/equities/advances-declines?year=2024',
     '/equities/monthly-settlement-stats/capital-market?financial_year=2022-2023',
     '/equities/monthly-settlement-stats/fno?financial_year=2022-2023',
     '/equities/stock-pcr?symbol=RELIANCE',
     '/equities/equity-tickers',
-    '/nseindices/history?symbol=NIFTY 50&start_date=10-Jan-2024&end_date=12-Jan-2024',
+    '/equities/annual-reports?symbol=BAJAJCON',
+    '/equities/shareholding-patterns?symbol=BAJAJCON',
+    '/equities/insider-trading?start_date=28-01-2024&end_date=01-02-2024',
+    '/equities/board-meetings?start_date=28-01-2024&end_date=01-02-2024',
+    '/nseindices/history?symbol=NIFTY 50&start_date=10-01-2024&end_date=12-01-2024',
     '/nseindices/ratios?symbol=NIFTY 50&start_date=10-Jan-2024&end_date=12-Jan-2024',
     '/nseindices/returns?symbol=NIFTY 50&start_date=10-Jan-2024&end_date=12-Jan-2024',
     '/nseindices/indice-pcr?symbol=NIFTY',
-    '/nseindices/india-vix?start_date=28-01-2024&end_date=04-02-2024',
+    '/nseindices/india-vix?start_date=28-01-2024&end_date=01-02-2024',
+    '/nseindices/index-symbols',
     '/sentiment/pcr-indice-analysis',
     '/sentiment/pcr-stocks-analysis?symbol=INFY',
     '/generate_plot?ticker=BSE.NS',
-    '/equities/annual-reports?symbol=BAJAJCON',
-    '/equities/shareholding-patterns?symbol=BAJAJCON',
-    '/equities/insider-trading?start_date=28-01-2024&end_date=04-02-2024',
-    '/equities/board-meetings?start_date=28-01-2024&end_date=04-02-2024'
+    '/screener-equities/quarterly-result?symbol=vedl'
 ]
```

### Comparing `fin_maestro_kin-0.2.2/fin_maestro_kin/main.py` & `fin_maestro_kin-0.2.3/fin_maestro_kin/main.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from fastapi import FastAPI
 from modules.sentiment_analysis.sentiment_analysis import router as sentiment_analysis_router
 from modules.trend_detector.trend_detector import router as trend_detector_router
 from modules.data_toolkit.nse.nse_indices import router as nse_indices_router
 from modules.data_toolkit.nse.nse_equities import router as nse_eq_router
+from modules.data_toolkit.screener.screener_equities import router as screener_eq_router
 
 app = FastAPI()
 
 app.include_router(sentiment_analysis_router)
 app.include_router(trend_detector_router)
 app.include_router(nse_indices_router)
-app.include_router(nse_eq_router)
+app.include_router(nse_eq_router)
+app.include_router(screener_eq_router)
```

### Comparing `fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/nse/helper.py` & `fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/nse/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import requests
 import pandas as pd
+import json
 import math
 from datetime import datetime
 
 headers = {
     'Connection': 'keep-alive',
     'Cache-Control': 'max-age=0',
     'DNT': '1',
@@ -41,15 +42,14 @@
     except ValueError:
         session = requests.Session()
         result = session.get("http://nseindia.com", headers=headers)
         result = session.get(payload, headers=headers).json()
     return result
 
 
-# Convert DataFrame to dictionary with special handling for float values
 def convert_dataframe_to_dict(df):
     df_dict = df.to_dict(orient='records')
     for record in df_dict:
         for key, value in record.items():
             if isinstance(value, float):
                 if pd.notna(value) and math.isfinite(value):
                     record[key] = round(value, 2)
@@ -296,18 +296,14 @@
             "to_year": entry["toYr"],
             "attachment": entry["fileName"],
         }
         processed_data.append(processed_entry)
     return processed_data
 
 
-import json
-
-import json
-
 def process_index_data(data):
     data_json = data.to_json(orient="records")
 
     try:
         data = json.loads(data_json)
     except json.JSONDecodeError:
         return {"error": "Invalid JSON data"}
@@ -322,9 +318,7 @@
             "low_value": entry["indexCloseOnlineRecords"]["EOD_LOW_INDEX_VAL"],
             "timestamp": entry["indexCloseOnlineRecords"]["EOD_TIMESTAMP"],
             "traded_quantity": entry["indexTurnoverRecords"]["HIT_TRADED_QTY"],
             "turnover": entry["indexTurnoverRecords"]["HIT_TURN_OVER"]
         }
         processed_data.append(processed_entry)
     return processed_data
-
-
```

### Comparing `fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py` & `fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/nse/nse_equities.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from modules.data_toolkit.nse.helper import *
 from fastapi.responses import JSONResponse
 import requests
 import pandas as pd
 import re
 import json
 
-router = APIRouter(tags=["Equities"])
+router = APIRouter(tags=["NSE Equities"])
 
     
 def security_wise_archive(symbol, start_date, end_date, series="ALL"):   
     base_url = "https://www.nseindia.com/api/historical/securityArchives"
     customized_request_url = f"{base_url}?from={start_date}&to={end_date}&symbol={symbol.upper()}&dataType=priceVolumeDeliverable&series={series.upper()}"
     response = fetch_data_from_nse(customized_request_url)
     
@@ -19,15 +19,15 @@
     if not payload:
         raise HTTPException(status_code=404, detail=f"No data found for the specified parameters.")
     
     return pd.DataFrame(payload)
 
 
 # Example usage - http://localhost:8000/equities/security-archives?symbol=TCS&start_date=04-01-2024&end_date=14-01-2024&series=ALL
-@router.get("/equities/security-archives",tags=["Equities"])
+@router.get("/equities/security-archives",tags=["NSE Equities"])
 def get_security_wise_archive(
     symbol: str = Query(..., title="Symbol", description="Stock symbol"),
     start_date: str = Query(..., title="From Date", description="Start date for historical data in dd-mm-yyyy format"),
     end_date: str = Query(..., title="To Date", description="End date for historical data in dd-mm-yyyy format"),
     series: str = Query("ALL", title="Series", description="Stock series")
 ):
     try:
@@ -48,15 +48,15 @@
     if not payload:
         raise HTTPException(status_code=404, detail=f"No data found for the specified parameters.")
     
     return pd.DataFrame(payload)
 
 
 # Example usage - http://localhost:8000/equities/bulk-deals-archives?start_date=28-01-2024&end_date=04-02-2024
-@router.get("/equities/bulk-deals-archives",tags=["Equities"])
+@router.get("/equities/bulk-deals-archives",tags=["NSE Equities"])
 def get_bulk_deals_archives(
     start_date: str = Query(..., title="From Date", description="Start date for historical data in dd-mm-yyyy format"),
     end_date: str = Query(..., title="To Date", description="End date for historical data in dd-mm-yyyy format"),  
 ):
     try:
         historical_data = bulk_deals_archives(start_date, end_date)
         processed_data = process_bulk_block_deal_archive_data(historical_data)
@@ -75,15 +75,15 @@
     if not payload:
         raise HTTPException(status_code=404, detail=f"No data found for the specified parameters.")
     
     return pd.DataFrame(payload)
 
 
 # Example usage - http://localhost:8000/equities/block-deals-archives?start_date=28-01-2024&end_date=04-02-2024
-@router.get("/equities/block-deals-archives",tags=["Equities"])
+@router.get("/equities/block-deals-archives",tags=["NSE Equities"])
 def get_block_deals_archives(
     start_date: str = Query(..., title="From Date", description="Start date for historical data in dd-mm-yyyy format"),
     end_date: str = Query(..., title="To Date", description="End date for historical data in dd-mm-yyyy format"),  
 ):
     try:
         historical_data = block_deals_archives(start_date, end_date)
         processed_data = process_bulk_block_deal_archive_data(historical_data)
@@ -102,15 +102,15 @@
     if not payload:
         raise HTTPException(status_code=404, detail=f"No data found for the specified parameters.")
     
     return pd.DataFrame(payload)
 
 
 #Example usage - http://localhost:8000/equities/short-selling-archives?start_date=28-01-2024&end_date=04-02-2024
-@router.get("/equities/short-selling-archives",tags=["Equities"])
+@router.get("/equities/short-selling-archives",tags=["NSE Equities"])
 def get_short_selling_archives(
     start_date: str = Query(..., title="From Date", description="Start date for historical data in dd-mm-yyyy format"),
     end_date: str = Query(..., title="To Date", description="End date for historical data in dd-mm-yyyy format"),  
 ):
     try:
         historical_data = short_selling_archives(start_date, end_date)
         processed_data = process_short_selling_archives_data(historical_data)
@@ -133,15 +133,15 @@
     else:
         payload = response.get('data', [])
     
     return pd.DataFrame(payload)
     
 
 # Example usage - http://localhost:8000/equities/corporate-actions?start_date=28-01-2024&end_date=04-02-2024
-@router.get("/equities/corporate-actions",tags=["Equities"])
+@router.get("/equities/corporate-actions",tags=["NSE Equities"])
 def get_corporate_actions(
     start_date: str = Query(..., title="From Date", description="Start date for data in dd-mm-yyyy format"),
     end_date: str = Query(..., title="To Date", description="End date for data in dd-mm-yyyy format"),  
 ):
     try:
         data = corporate_actions(start_date, end_date)
         processed_data = process_corporate_actions_data(data)
@@ -158,15 +158,15 @@
     if not payload:
         raise HTTPException(status_code=404, detail=f"No data found for the specified parameters.")
     
     return pd.DataFrame(payload)
     
 
 # Example usage - http://localhost:8000/equities/most-active-securities
-@router.get("/equities/most-active-securities",tags=["Equities"])
+@router.get("/equities/most-active-securities",tags=["NSE Equities"])
 def get_nse_monthly_most_active_securities():
     try:
         historical_data = nse_monthly_most_active_securities()
         processed_data = process_most_active_securities_data(historical_data)
         return JSONResponse(content={"most_active_securities_data": processed_data})
     except Exception as e:
         raise HTTPException(status_code=500, detail=f"Error fetching monthly most active securities data: {e}")
@@ -182,15 +182,15 @@
     if not payload:
         raise HTTPException(status_code=404, detail=f"No data found for the specified parameters.")
     
     return pd.DataFrame(payload)
 
 
 #Example usage - http://localhost:8000/equities/advances-declines?year=2024
-@router.get("/equities/advances-declines",tags=["Equities"])
+@router.get("/equities/advances-declines",tags=["NSE Equities"])
 def get_nse_monthly_advances_and_declines(
     year: str = Query(..., title="Year", description="Year for historical data in format YYYY"), 
 ):
     if not re.match(r"\d{4}", year):
         raise HTTPException(status_code=422, detail="Invalid year format. Please use 'YYYY' format.")
     
     try:
@@ -210,15 +210,15 @@
     if not payload:
         raise HTTPException(status_code=404, detail=f"No capital market settlement statistics found.")
     
     return pd.DataFrame(payload)
 
 
 #Example usage - http://localhost:8000/equities/monthly-settlement-stats/capital-market?financial_year=2022-2023
-@router.get("/equities/monthly-settlement-stats/capital-market",tags=["Equities"])
+@router.get("/equities/monthly-settlement-stats/capital-market",tags=["NSE Equities"])
 def get_nse_capital_market_monthly_settlement_stats(
     financial_year: str = Query(..., title="Year", description="Financial Year for historical data in format YYYY-YYYY"), 
 ):
     if not re.match(r"\d{4}-\d{4}", financial_year):
         raise HTTPException(status_code=422, detail="Invalid financial year format. Please use 'YYYY-YYYY' format.")
     
     try:
@@ -239,15 +239,15 @@
     if not payload:
         raise HTTPException(status_code=404, detail="No monthly settlement statistics found.")
     
     return pd.DataFrame(payload)
 
 
 #Example usage - http://localhost:8000/equities/monthly-settlement-stats/fno?financial_year=2022-2023
-@router.get("/equities/monthly-settlement-stats/fno",tags=["Equities"])
+@router.get("/equities/monthly-settlement-stats/fno",tags=["NSE Equities"])
 def get_nse_fno_monthly_settlement_stats(
     financial_year: str = Query(..., title="Year", description="Financial Year for historical data in format YYYY-YYYY"), 
 ):
     if not re.match(r"\d{4}-\d{4}", financial_year):
         raise HTTPException(status_code=422, detail="Invalid financial year format. Please use 'YYYY-YYYY' format.")
     
     try:
@@ -278,15 +278,15 @@
     totPE = data['filtered']['PE']['totOI']
 
     pcr= totPE/totCE
     return round(pcr,3)
 
 
 #Example usage - http://127.0.0.1:8000/equities/stock-pcr?symbol=RELIANCE
-@router.get("/equities/stock-pcr",tags=["Equities"])
+@router.get("/equities/stock-pcr",tags=["NSE Equities"])
 def get_pcr(symbol: str = Query(..., title="Symbol", description="Stock symbol")):
     pcr_value = pcr_stocks_scraper(symbol)
     return {"symbol": symbol, "pcr_value": pcr_value}
 
 
 def nse_equity_tickers():
     try:
@@ -294,15 +294,15 @@
         tickers = symbols['SYMBOL'].tolist()
         return tickers
     except Exception as e:
         return f"Error fetching equity tickers: {e}"
 
 
 #Example usage - http://localhost:8000/equities/equity-tickers
-@router.get("/equities/equity-tickers", tags=["Equities"])
+@router.get("/equities/equity-tickers", tags=["NSE Equities"])
 def get_nse_equity_tickers():
     return {"equity_tickers": nse_equity_tickers()}
 
 
 def board_meetings(start_date, end_date):
     base_url = "https://www.nseindia.com/api/corporate-board-meetings"
     
@@ -317,15 +317,15 @@
     else:
         payload = response.get('data', [])
     
     return pd.DataFrame(payload)
     
 
 # Example usage - http://localhost:8000/equities/board-meetings?start_date=28-01-2024&end_date=04-02-2024
-@router.get("/equities/board-meetings",tags=["Equities"])
+@router.get("/equities/board-meetings",tags=["NSE Equities"])
 def get_board_meetings(
     start_date: str = Query(..., title="From Date", description="Start date for data in dd-mm-yyyy format"),
     end_date: str = Query(..., title="To Date", description="End date for data in dd-mm-yyyy format"),  
 ):
     try:
         data = board_meetings(start_date, end_date)
         processed_data = process_board_meetings_data(data)
@@ -348,15 +348,15 @@
     else:
         payload = response.get('data', [])
     
     return pd.DataFrame(payload)
     
 
 # Example usage - http://localhost:8000/equities/insider-trading?start_date=28-01-2024&end_date=04-02-2024
-@router.get("/equities/insider-trading",tags=["Equities"])
+@router.get("/equities/insider-trading",tags=["NSE Equities"])
 def get_insider_trading(
     start_date: str = Query(..., title="From Date", description="Start date for data in dd-mm-yyyy format"),
     end_date: str = Query(..., title="To Date", description="End date for data in dd-mm-yyyy format"),  
 ):
     try:
         data = insider_trading(start_date, end_date)
         processed_data = process_insider_trading_data(data)
@@ -378,15 +378,15 @@
         payload = response
     else:
         payload = response.get('data', [])
     return pd.DataFrame(payload)
     
 
 # Example usage - http://localhost:8000/equities/shareholding-patterns?symbol=BAJAJCON
-@router.get("/equities/shareholding-patterns",tags=["Equities"])
+@router.get("/equities/shareholding-patterns",tags=["NSE Equities"])
 def get_shareholding_patterns(
     symbol: str = Query(..., title="Symbol", description="Stock Symbol")
 ):
     try:
         data = shareholding_patterns(symbol)
         processed_data = process_shareholding_patterns_data(data)
         return JSONResponse(content={"shareholding_patterns_data": processed_data})
@@ -407,15 +407,15 @@
         payload = response
     else:
         payload = response.get('data', [])
     return pd.DataFrame(payload)
     
 
 # Example usage - http://localhost:8000/equities/annual-reports?symbol=BAJAJCON
-@router.get("/equities/annual-reports",tags=["Equities"])
+@router.get("/equities/annual-reports",tags=["NSE Equities"])
 def get_annual_reports(
     symbol: str = Query(..., title="Symbol", description="Stock Symbol")
 ):
     try:
         data = annual_reports(symbol)
         processed_data = process_annual_reports_data(data)
         return JSONResponse(content={"annual_reports_data": processed_data})
```

### Comparing `fin_maestro_kin-0.2.2/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py` & `fin_maestro_kin-0.2.3/fin_maestro_kin/modules/data_toolkit/nse/nse_indices.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.2/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py` & `fin_maestro_kin-0.2.3/fin_maestro_kin/modules/sentiment_analysis/pcr_data.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.2/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py` & `fin_maestro_kin-0.2.3/fin_maestro_kin/modules/sentiment_analysis/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.2/fin_maestro_kin/modules/trend_detector/trend_detector.py` & `fin_maestro_kin-0.2.3/fin_maestro_kin/modules/trend_detector/trend_detector.py`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.2/LICENSE` & `fin_maestro_kin-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.2/pyproject.toml` & `fin_maestro_kin-0.2.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fin-maestro-kin"
-version = "0.2.2"
+version = "0.2.3"
 description = "Where Data Meets FastAPI Brilliance with Fin-Maestro-Kin – Your All-in-One Finance API."
 authors = ["DEV_FINWIZ <devjuneja43@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
@@ -12,14 +12,15 @@
 uvicorn = "^0.25.0"
 pydantic = "^2.5.3"
 requests = "^2.31.0"
 yfinance = "^0.2.35"
 matplotlib = "^3.8.2"
 pandas = "^2.1.4"
 numpy = "^1.26.3"
+beautifulsoup4 = "^4.12.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^8.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `fin_maestro_kin-0.2.2/README.md` & `fin_maestro_kin-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `fin_maestro_kin-0.2.2/PKG-INFO` & `fin_maestro_kin-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: fin-maestro-kin
-Version: 0.2.2
+Version: 0.2.3
 Summary: Where Data Meets FastAPI Brilliance with Fin-Maestro-Kin – Your All-in-One Finance API.
 License: MIT
 Author: DEV_FINWIZ
 Author-email: devjuneja43@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
 Requires-Dist: fastapi (>=0.109.0,<0.110.0)
 Requires-Dist: matplotlib (>=3.8.2,<4.0.0)
 Requires-Dist: numpy (>=1.26.3,<2.0.0)
 Requires-Dist: pandas (>=2.1.4,<3.0.0)
 Requires-Dist: pydantic (>=2.5.3,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: uvicorn (>=0.25.0,<0.26.0)
```

#### html2text {}

```diff
@@ -1,20 +1,20 @@
-Metadata-Version: 2.1 Name: fin-maestro-kin Version: 0.2.2 Summary: Where Data
+Metadata-Version: 2.1 Name: fin-maestro-kin Version: 0.2.3 Summary: Where Data
 Meets FastAPI Brilliance with Fin-Maestro-Kin â Your All-in-One Finance API.
 License: MIT Author: DEV_FINWIZ Author-email: devjuneja43@gmail.com Requires-
 Python: >=3.9,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
-Language :: Python :: 3.12 Requires-Dist: fastapi (>=0.109.0,<0.110.0)
-Requires-Dist: matplotlib (>=3.8.2,<4.0.0) Requires-Dist: numpy
-(>=1.26.3,<2.0.0) Requires-Dist: pandas (>=2.1.4,<3.0.0) Requires-Dist:
-pydantic (>=2.5.3,<3.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-
-Dist: uvicorn (>=0.25.0,<0.26.0) Requires-Dist: yfinance (>=0.2.35,<0.3.0)
-Description-Content-Type: text/markdown
+Language :: Python :: 3.12 Requires-Dist: beautifulsoup4 (>=4.12.3,<5.0.0)
+Requires-Dist: fastapi (>=0.109.0,<0.110.0) Requires-Dist: matplotlib
+(>=3.8.2,<4.0.0) Requires-Dist: numpy (>=1.26.3,<2.0.0) Requires-Dist: pandas
+(>=2.1.4,<3.0.0) Requires-Dist: pydantic (>=2.5.3,<3.0.0) Requires-Dist:
+requests (>=2.31.0,<3.0.0) Requires-Dist: uvicorn (>=0.25.0,<0.26.0) Requires-
+Dist: yfinance (>=0.2.35,<0.3.0) Description-Content-Type: text/markdown
                                     [image]
                          ************ FFiinn--MMaaeessttrroo--KKiinn ************
         _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_C_o_d_e_F_a_c_t_o_r_-_A_-_b_l_u_e_&_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-
  _b_a_d_g_e_&_c_o_l_o_r_=_b_l_u_e_][https://img.shields.io/badge/Python-3.9.1-blue&?style=for-
   the-badge&color=blue]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_d_e_v_f_i_n_w_i_z_/_F_i_n_-
  _M_a_e_s_t_r_o_-_K_i_n_?_c_o_l_o_r_=_p_u_r_p_l_e_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/
 _l_a_s_t_-_c_o_m_m_i_t_/_d_e_v_f_i_n_w_i_z_/_F_i_n_-_M_a_e_s_t_r_o_-_K_i_n_?_c_o_l_o_r_=_y_e_l_l_o_w_&_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]_[_h_t_t_p_s_:_/
```

