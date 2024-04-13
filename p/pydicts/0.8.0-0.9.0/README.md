# Comparing `tmp/pydicts-0.8.0.tar.gz` & `tmp/pydicts-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydicts-0.8.0.tar", max compression
+gzip compressed data, was "pydicts-0.9.0.tar", max compression
```

## Comparing `pydicts-0.8.0.tar` & `pydicts-0.9.0.tar`

### file list

```diff
@@ -1,23 +1,27 @@
--rw-r--r--   0        0        0    35149 2023-04-10 16:27:20.112887 pydicts-0.8.0/LICENSE
--rw-r--r--   0        0        0     7799 2023-11-26 16:54:44.928656 pydicts-0.8.0/README.md
--rw-r--r--   0        0        0      145 2023-11-26 16:53:10.401653 pydicts-0.8.0/pydicts/__init__.py
--rw-r--r--   0        0        0    16783 2023-11-26 11:29:52.240032 pydicts-0.8.0/pydicts/casts.py
--rw-r--r--   0        0        0     2814 2023-04-11 05:44:25.702913 pydicts-0.8.0/pydicts/classes.py
--rw-r--r--   0        0        0      424 2023-11-26 16:54:51.900656 pydicts-0.8.0/pydicts/locale/en/LC_MESSAGES/pydicts.mo
--rw-r--r--   0        0        0      738 2022-04-25 13:52:57.304754 pydicts-0.8.0/pydicts/locale/en.po
--rw-r--r--   0        0        0      422 2023-11-26 16:54:51.898656 pydicts-0.8.0/pydicts/locale/es/LC_MESSAGES/pydicts.mo
--rw-r--r--   0        0        0     3006 2023-11-26 16:54:51.896656 pydicts-0.8.0/pydicts/locale/es.po
--rw-r--r--   0        0        0      827 2023-11-26 16:54:51.892656 pydicts-0.8.0/pydicts/locale/pydicts.pot
--rw-r--r--   0        0        0     7292 2023-11-04 08:57:19.417456 pydicts-0.8.0/pydicts/lod.py
--rw-r--r--   0        0        0     1052 2023-04-12 05:25:02.458349 pydicts-0.8.0/pydicts/lod_xyv.py
--rw-r--r--   0        0        0     9707 2023-07-02 08:06:04.240499 pydicts-0.8.0/pydicts/lod_ymv.py
--rw-r--r--   0        0        0     2918 2023-11-26 16:43:44.399636 pydicts-0.8.0/pydicts/lol.py
--rw-r--r--   0        0        0     3716 2023-05-04 17:10:10.584841 pydicts-0.8.0/pydicts/pylatex.py
--rw-r--r--   0        0        0        0 2023-04-10 16:27:20.112887 pydicts-0.8.0/pydicts/tests/__init__.py
--rw-r--r--   0        0        0    10327 2023-11-26 16:36:16.920622 pydicts-0.8.0/pydicts/tests/test_casts.py
--rw-r--r--   0        0        0     2118 2023-11-04 08:57:19.418455 pydicts-0.8.0/pydicts/tests/test_lod.py
--rw-r--r--   0        0        0     5973 2023-07-02 08:09:33.101505 pydicts-0.8.0/pydicts/tests/test_lod_ymv.py
--rw-r--r--   0        0        0     1135 2023-11-26 16:43:48.635636 pydicts-0.8.0/pydicts/tests/test_lol.py
--rw-r--r--   0        0        0     1038 2023-05-04 17:14:37.488849 pydicts-0.8.0/pydicts/tests/test_pylatex.py
--rw-r--r--   0        0        0      815 2023-11-26 16:52:34.616652 pydicts-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     8359 1970-01-01 00:00:00.000000 pydicts-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-10 16:27:20.112887 pydicts-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1707 2023-12-04 19:07:56.073587 pydicts-0.9.0/README.md
+-rw-r--r--   0        0        0      143 2023-12-04 19:07:56.073587 pydicts-0.9.0/pydicts/__init__.py
+-rw-r--r--   0        0        0    17499 2023-12-04 18:57:49.935774 pydicts-0.9.0/pydicts/casts.py
+-rw-r--r--   0        0        0     3001 2023-12-01 05:35:23.397345 pydicts-0.9.0/pydicts/classes.py
+-rw-r--r--   0        0        0      951 2023-04-19 18:07:44.800377 pydicts-0.9.0/pydicts/devscripts.py
+-rw-r--r--   0        0        0      227 2023-12-01 05:35:23.398345 pydicts-0.9.0/pydicts/exceptions.py
+-rw-r--r--   0        0        0      424 2023-12-04 19:05:09.652582 pydicts-0.9.0/pydicts/locale/en/LC_MESSAGES/pydicts.mo
+-rw-r--r--   0        0        0      738 2022-04-25 13:52:57.304754 pydicts-0.9.0/pydicts/locale/en.po
+-rw-r--r--   0        0        0     1063 2023-12-04 19:05:09.650582 pydicts-0.9.0/pydicts/locale/es/LC_MESSAGES/pydicts.mo
+-rw-r--r--   0        0        0     2117 2023-12-04 19:07:56.073587 pydicts-0.9.0/pydicts/locale/es.po
+-rw-r--r--   0        0        0     1698 2023-12-04 19:07:56.074587 pydicts-0.9.0/pydicts/locale/pydicts.pot
+-rw-r--r--   0        0        0     7495 2023-12-01 05:35:23.398345 pydicts-0.9.0/pydicts/lod.py
+-rw-r--r--   0        0        0     1222 2023-12-01 05:35:23.398345 pydicts-0.9.0/pydicts/lod_xyv.py
+-rw-r--r--   0        0        0     9878 2023-12-01 05:35:23.398345 pydicts-0.9.0/pydicts/lod_ymv.py
+-rw-r--r--   0        0        0     3828 2023-12-02 06:57:47.172483 pydicts-0.9.0/pydicts/lol.py
+-rw-r--r--   0        0        0     7772 2023-12-04 18:57:49.936774 pydicts-0.9.0/pydicts/myjsonencoder.py
+-rw-r--r--   0        0        0     3897 2023-12-01 05:35:23.399345 pydicts-0.9.0/pydicts/pylatex.py
+-rw-r--r--   0        0        0        0 2023-04-10 16:27:20.112887 pydicts-0.9.0/pydicts/tests/__init__.py
+-rw-r--r--   0        0        0    10475 2023-12-04 18:57:49.936774 pydicts-0.9.0/pydicts/tests/test_casts.py
+-rw-r--r--   0        0        0     2118 2023-11-04 08:57:19.418455 pydicts-0.9.0/pydicts/tests/test_lod.py
+-rw-r--r--   0        0        0     5973 2023-07-02 08:09:33.101505 pydicts-0.9.0/pydicts/tests/test_lod_ymv.py
+-rw-r--r--   0        0        0     1288 2023-12-02 06:57:47.172483 pydicts-0.9.0/pydicts/tests/test_lol.py
+-rw-r--r--   0        0        0     2265 2023-12-04 18:57:49.936774 pydicts-0.9.0/pydicts/tests/test_myjsonencoder.py
+-rw-r--r--   0        0        0     1194 2023-12-01 05:35:23.399345 pydicts-0.9.0/pydicts/tests/test_pylatex.py
+-rw-r--r--   0        0        0      778 2023-12-04 19:07:56.074587 pydicts-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pydicts-0.9.0/PKG-INFO
```

### Comparing `pydicts-0.8.0/LICENSE` & `pydicts-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydicts-0.8.0/pydicts/casts.py` & `pydicts-0.9.0/pydicts/casts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,48 @@
 ### If a function only can be used by dtaware or naive it will have its prefix dtaware_ or dtnaive_
 ### If a function can use both of them its prefix will be dt_
 from decimal import Decimal
 from datetime import timedelta, date, datetime, time
+from gettext import translation
+from importlib.resources import files
+from pydicts import exceptions
 from zoneinfo import ZoneInfo
+        
+try:
+    t=translation('pydicts', files("pydicts") / 'locale')
+    _=t.gettext
+except:
+    _=str
 
-_=str
 
 def object_or_empty(v):
     """
         Returns and empty string if None, else return value
     """
     return "" if v is None else v
 
 ## Converts a string  to a decimal
 def str2decimal(s, type):
+    if s is None:
+        return None
     if type==1: #2.123,25
         try:
             return Decimal(s.replace(".","").replace(",", "."))
         except:
-            return None
+            raise exceptions.CastException(_("Method str2decimal couln't convert {0} ({1}) to a Decimal"))
 
 
 def str2bool(value):
     """
         Converts strings True or False to boolean
         @param s String
         @return Boolean
     """
     def exception():
-        raise Exception(f"Method str2bool couldn't convert {value} ({value.__class__} to a boolean")
+        raise exceptions.CastException(_("Method str2bool couldn't convert {0} ({1}) to a boolean").format(value, value.__class__))
     if not value.__class__ is str:
         exception()
         
     if value=="0" or value.lower()=="false":
         return False
     elif value=="1" or value.lower()=="true":
         return True
@@ -172,24 +182,24 @@
     return dtaware_day_end_from_date(date(year, 12, 31), tz_name)
     
 def dtaware_day_end(dt, tz_name):
     """
         Returns the last  datetime (microsecond  level) of the  day in tz_name zone
     """
     if is_naive():
-        raise Exception(_("Datetime parameter should be aware"))
+        raise exceptions.CastException(_("A datetime with timezone is needed"))
     dt=dtaware_changes_tz(dt, tz_name)
     return dt.replace(hour=23, minute=59, second=59, microsecond=999999)
     
 def dtnaive_day_end(dt):
     """
         Returns the last  datetime (microsecond  level) of the  day in naive format
     """
     if is_aware(dt):
-        raise Exception(_("Datetime parameter should be naive"))
+        raise exceptions.CastException(_("A datetime without timezone is needed"))
     return dt.replace(hour=23, minute=59, second=59, microsecond=999999)
 
 ## Returns the end of the day dtnaive from a date
 def dtnaive_day_end_from_date(date_):
     dt=datetime(date_.year, date_.month, date_.day)
     return dtnaive_day_end(dt)
 
@@ -200,15 +210,15 @@
 ## Returns a dtnaive or dtawre (as parameter) with the end of the day
 def dtnaive_day_start(dt):
     return dt.replace(hour=0, minute=0, second=0, microsecond=0)
 
 ## Returns a dtnaive or dtawre (as parameter) with the end of the day in zone tz_name
 def dtaware_day_start(dt, tz_name):
     if is_naive():
-        raise Exception(_("Datetime parameter should be aware"))
+        raise exceptions.CastException(_("A datetime with timezone is needed"))
     dt=dtaware_changes_tz(dt, tz_name)
     return dt.replace(hour=0, minute=0, second=0, microsecond=0)
 
 ## Returns the end of the day dtnaive from a date
 def dtnaive_day_start_from_date(date_):
     dt=datetime(date_.year, date_.month, date_.day)
     return dtnaive_day_start(dt)
@@ -266,15 +276,15 @@
                 s=s.replace("PM", "")
                 points=s.split(":")
                 return time(int(points[0])+12, int(points[1]))
             else:#AM
                 points=s.split(":")
                 return time(int(points[0]), int(points[1]))
     else:
-        raise Exception(_("I can't convert this format '{}'. I only support this {}".format(format, allowed)))
+        raise exceptions.CastException(_("I can't convert this format '{}'. I only support this {}").format(format, allowed))
 
 ## Converts a time to a string
 def time2str(ti, format="HH:MM" ):
     allowed=["HH:MM", "HH:MM:SS","Xulpymoney"]
     if format in allowed:
         if ti==None:
             return None
@@ -304,18 +314,18 @@
                 return date(int(d[2]), int(d[1]),  int(d[0]))
             if format=="DD/MM": #DD/MM
                 d=iso.split("/")
                 return date(date.today().year, int(d[1]),  int(d[0]))
         except:
             return None
     else:
-        raise Exception("I can't convert this format '{}'. I only support this {}".format(format, allowed))
+        raise exceptions.CastException(_("I can't convert this format '{}'. I only support this {}").format(format, allowed))
 
 def str2dtnaive(s, format):
-    allowed=["%Y%m%d%H%M","%Y-%m-%d %H:%M:%S","%d/%m/%Y %H:%M","%d %m %H:%M %Y","%Y-%m-%d %H:%M:%S.","%H:%M:%S", '%b %d %H:%M:%S']
+    allowed=["%Y%m%d%H%M","%Y-%m-%d %H:%M:%S","%d/%m/%Y %H:%M","%d %m %H:%M %Y","%Y-%m-%d %H:%M:%S.","%H:%M:%S", '%b %d %H:%M:%S', "JsIso"]
     if format in allowed:
         if format=="%Y%m%d%H%M":
             dat=datetime.strptime( s, format )
             return dat
         if format=="%Y-%m-%d %H:%M:%S":#2017-11-20 23:00:00
             return datetime.strptime( s, format )
         if format=="%d/%m/%Y %H:%M":#20/11/2017 23:00
@@ -332,16 +342,20 @@
         if format=="%H:%M:%S": 
             tod=date.today()
             a=s.split(":")
             return datetime(tod.year, tod.month, tod.day, int(a[0]), int(a[1]), int(a[2]))
         if format=='%b %d %H:%M:%S': #Apr 26 07:50:44. Year is missing so I set to current
             s=f"{date.today().year} {s}"
             return datetime.strptime(s, '%Y %b %d %H:%M:%S')
+        if format=="JsIso": #2021-08-21T06:27:38.294
+            s=s.replace("T"," ")
+            dtnaive=str2dtnaive(s,"%Y-%m-%d %H:%M:%S.")
+            return dtnaive
     else:
-        raise Exception("I can't convert this format '{}'. I only support this {}".format(format, allowed))
+        raise exceptions.CastException(_("I can't convert this format '{}'. I only support this {}").format(format, allowed))
 
 def str2dtaware(s, format, tz_name='UTC'):
     allowed=["%Y-%m-%d %H:%M:%S%z","%Y-%m-%d %H:%M:%S.%z", "JsUtcIso"]
     if format in allowed:
         if format=="%Y-%m-%d %H:%M:%S%z":#2017-11-20 23:00:00+00:00
             s=s[:-3]+s[-2:]
             dt=datetime.strptime( s, format )
@@ -386,15 +400,15 @@
 
 
 ## Returns a formated string of a dtaware string formatting with a zone name
 ## @param dt datetime aware object
 ## @return String
 def dtaware2str(dt, format):
     if is_naive(dt)==True:
-        raise Exception("A dtaware is needed for {}".format(dt))
+        raise exceptions.CastException("A datetime with timezone is needed for {}").format(dt)
     else:
         return dtnaive2str(dt, format)
 
 ## Returns a formated string of a dtaware string formatting with a zone name
 ## @param dt datetime aware object
 ## @param format String in ["%Y-%m-%d", "%Y-%m-%d %H:%M:%S", "%Y%m%d %H%M", "%Y%m%d%H%M"]
 ## @return String
@@ -410,15 +424,15 @@
         elif format=="%Y%m%d %H%M": 
             return dt.strftime("%Y%m%d %H%M")
         elif format=="%Y%m%d%H%M":
             return dt.strftime("%Y%m%d%H%M")
         elif format=="JsUtcIso":
             return dt.strftime("%Y-%m-%dT%H:%M:%SZ")
     else:
-        raise Exception("I can't convert this format '{}'. I only support this {}".format(format, allowed))
+        raise exceptions.CastException(_("I can't convert this format '{}'. I only support this {}").format(format, allowed))
 
 ## Changes zoneinfo from a dtaware object
 ## For example:
 ## - datetime.datetime(2018, 5, 18, 8, 12, tzinfo=<DstTzInfo 'Europe/Madrid' CEST+2:00:00 DST>)
 ## - libcaloriestrackerfunctions.dtaware_changes_tz(a,"Europe/London")
 ## - datetime.datetime(2018, 5, 18, 7, 12, tzinfo=<DstTzInfo 'Europe/London' BST+1:00:00 DST>)
 ## @param dt datetime aware object
@@ -426,15 +440,15 @@
 ## @return datetime aware object
 def dtaware_changes_tz(dt,  tzname):
     if dt==None:
         return None
     if is_aware(dt):
         return dt.astimezone(ZoneInfo(tzname))
     else:
-        raise Exception("Dtaware needed")
+        raise exceptions.CastException(_("A datetime with timezone is needed"))
 
 ## Returns a list of tuples (year, month) from a month to another month, both included
 ## @param year_from Integer
 ## @param month_from Integer
 ## @param year_to Integer If none uses current year
 ## @param month_to Integer If none uses current month
 def months(year_from, month_from, year_to=None, month_to=None):
```

### Comparing `pydicts-0.8.0/pydicts/classes.py` & `pydicts-0.9.0/pydicts/classes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,16 @@
 from pydicts.lod import lod_has_key, lod_print, lod_print_first, lod_sum, lod2list, lod_average_ponderated
+from gettext import translation
+from importlib.resources import files
+        
+try:
+    t=translation('pydicts', files("pydicts") / 'locale')
+    _=t.gettext
+except:
+    _=str
 ## El objetivo es crear un objeto list_dict que se almacenera en self.ld con funciones set
 ## set_from_db #Todo se carga desde base de datos con el minimo parametro posible
 ## set_from_db_and_variables #Preguntara a base datos aquellas variables que falten. Aunque no estén en los parámetros p.e. money_convert
 ## set_from_variables #Solo con variables
 ## set #El lod ya está hecho pero se necesita el objeto para operar con el
 ##class Do:
 ##    def __init__(self,d):
@@ -62,15 +70,15 @@
         del self.ld
         self.ld=ld
         return self
 
     def is_set(self):
         if hasattr(self, "ld"):
             return True
-        print(f"You must set your lod in {self.name}")
+        print(_("You must set your lod in {}").format(self.name))
         return False
 
     def append(self,o):
         self.ld.append(o)
 
     def first(self):
         return self.ld[0] if self.length()>0 else None
```

### Comparing `pydicts-0.8.0/pydicts/locale/en.po` & `pydicts-0.9.0/pydicts/locale/en.po`

 * *Files identical despite different names*

### Comparing `pydicts-0.8.0/pydicts/lod.py` & `pydicts-0.9.0/pydicts/lod.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 from collections import OrderedDict
 from tabulate import tabulate
+from gettext import translation
+from importlib.resources import files
+        
+try:
+    t=translation('pydicts', files("pydicts") / 'locale')
+    _=t.gettext
+except:
+    _=str
 
 def lod_has_key(lod, key):
     if len(lod)==0:
         return False
     return key in lod[0]
 
 ## Order data columns. None values are set at the beginning
@@ -29,15 +37,15 @@
     @param lod
     @type List of dictionaries
     @param number Number of dictionaries in the list to print. If None prints all lod. (defaults to None)
     @type Integer
     """
     number=len(lod) if number is None else number
     if len(lod)==0:
-        print("No data to print_batch")
+        print(_("This list of dictionaries hasn't data to print"))
     print(tabulate(lod[0:number], headers="keys", tablefmt="psql"))
 
 def lod_sum(lod, key, ignore_nones=True):
     r=0
     for d in lod:
         if ignore_nones is True and d[key] is None:
             continue
```

### Comparing `pydicts-0.8.0/pydicts/lod_xyv.py` & `pydicts-0.9.0/pydicts/lod_xyv.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+from gettext import translation
+from importlib.resources import files
 
+try:
+    t=translation('pydicts', files("pydicts") / 'locale')
+    _=t.gettext
+except:
+    _=str
 
 
 ## Converts a tipical groyp by lor with A, B, value, value into an other lod with A as rows, B as columns and value as AxB list of dic
 ## columns order can be defined in order
 def lod_xyv_transformation(ld, key_x, key_y, key_value, order=None):
     if len(ld)==0:
        return []
 
     if not key_x in ld[0] or not key_y in ld[0] or not key_value in ld[0]:
-        print("Keys names are not correct in dictionary in lod_year_month_value_transposition function")
+        print(_("Keys names are not correct in dictionary in lod_year_month_value_transposition function"))
         return None
 
     #Searches for all diferent keys
     columns=set()
     rows=set()
     for d in ld:
         columns.add(d[key_y])
```

### Comparing `pydicts-0.8.0/pydicts/lod_ymv.py` & `pydicts-0.9.0/pydicts/lod_ymv.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 from datetime import date
 from pydicts import lod
+from gettext import translation
+from importlib.resources import files
+
+try:
+    t=translation('pydicts', files("pydicts") / 'locale')
+    _=t.gettext
+except:
+    _=str
 """
     lod_ymv example:
     +------------------+-------------------+---------+
 |   datetime__year |   datetime__month |   quote |
 |------------------+-------------------+---------|
 |             2020 |                 1 |   82.92 |
 |             2020 |                 2 |   67.41 |
@@ -63,15 +71,15 @@
         |   2023 | 111.62 | 110.42 | 112.76 | 113.96 |   0    |   0    |   0    |   0    |   0    |   0    |   0    |   0    |  448.76 |
         +--------+--------+--------+--------+--------+--------+--------+--------+--------+--------+--------+--------+--------+---------+
     """
     if len(ld)==0:
        return []
 
     if not key_year in ld[0] or not key_month in ld[0] or not key_value in ld[0]:
-        print("Keys names are not correct in dictionary in lod_ymv_transposition function")
+        print(_("Keys names are not correct in dictionary in lod_ymv_transposition function"))
         return None
 
     min_year=lod.lod_min_value(ld, key_year)
     max_year=lod.lod_max_value(ld, key_year)
     #Initialize result
     r=[]
     for year in range(min_year,max_year+1):
```

### Comparing `pydicts-0.8.0/pydicts/pylatex.py` & `pydicts-0.9.0/pydicts/pylatex.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,28 @@
 """
 
 
 from pylatex import LongTabularx, MultiColumn
 from pylatex.basic import NewLine
 from pylatex.utils import NoEscape, bold, escape_latex
 from pydicts import lod
+from gettext import translation
+from importlib.resources import files
+        
+try:
+    t=translation('pydicts', files("pydicts") / 'locale')
+    _=t.gettext
+except:
+    _=str
+
 def pylatex_table(
     doc, 
     lod_, 
     code_=None, 
-    text_no_results="No data to show", 
+    text_no_results=_("No data to show"), 
 ):
     """
     Creates a table in a pylatex document
 
     @param doc pylatex document object
     @param lod 
     @param code_ |c|r|l|
@@ -39,15 +48,15 @@
         
     with doc.create(LongTabularx(code_)) as data_table:
         data_table.add_hline()
         data_table.add_row(headers)
         data_table.add_hline()
         data_table.end_table_header()
         data_table.add_hline()
-        data_table.add_row((MultiColumn(len(headers), align='r', data='La tabla continúa en la siguiente página'),))
+        data_table.add_row((MultiColumn(len(headers), align='r', data=_('This table continues in the next page')),))
         data_table.end_table_footer()
         data_table.end_table_last_footer()
 
         escaped_list=[]
         for list_ in lod.lod2lol(lod_):
             row=[]
             for column in range(len(headers)):
@@ -60,28 +69,28 @@
 
     
 def pylatex_table_with_matched_values(
     doc, 
     values_to_match, 
     lod_, 
     code_=None, 
-    text_no_results="No data to show", 
+    text_no_results=_("No data to show" ), 
     match_color="teal", 
     unmatch_color="red"
 ):
     """
     Creates a table in a pylatex document
     
     This function needs to have xcolor package loaded in document with
     doc.packages.append(Package('xcolor'))
 
     @param doc pylatex document object
     @param values_to_match Values to match is a list
     @param lod 
-    @param code_ |c|r|l|   Para usar wrapping |p{.20\\linewidth\p{.80\\linewidth}|
+    @param code_ |c|r|l|   Para usar wrapping |p{.20\\linewidth\\p{.80\\linewidth}|
     """
     keys= lod.lod_keys(lod_)
     if keys is None:
         doc.append(text_no_results)
         doc.append(NewLine())
         return
         
@@ -96,15 +105,15 @@
         
     with doc.create(LongTabularx(code_)) as data_table:
         data_table.add_hline()
         data_table.add_row(headers)
         data_table.add_hline()
         data_table.end_table_header()
         data_table.add_hline()
-        data_table.add_row((MultiColumn(len(headers), align='r', data='La tabla continúa en la siguiente página'),))
+        data_table.add_row((MultiColumn(len(headers), align='r', data=_('This table continues in the next page')),))
         data_table.end_table_footer()
         data_table.end_table_last_footer()
 
         #Prepare cells
         matched_list=[]
         for list_ in lod.lod2lol(lod_):
             row=[]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pydicts-0.8.0/pydicts/tests/test_casts.py` & `pydicts-0.9.0/pydicts/tests/test_casts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import date, time, datetime
 from decimal import Decimal
-from pydicts import casts
+from pydicts import casts, exceptions
 from pytest import raises
 from zoneinfo import ZoneInfo
 
 zonename_madrid="Europe/Madrid"
 zoneinfo_utc=ZoneInfo("UTC")
 dtnaive=casts.dtnaive_now()
 dtaware_utc=casts.dtaware_now()
@@ -15,19 +15,19 @@
     assert casts.object_or_empty(1)==1
     
 def test_str2decimal():
     assert casts.str2decimal(None, 1)==None
     assert casts.str2decimal("2.123,25", 1)==Decimal("2123.25")
 
 def test_str2bool():
-    with raises(Exception):
+    with raises(exceptions.CastException):
         casts.str2bool(None)==None
-    with raises(Exception):
+    with raises(exceptions.CastException):
         assert casts.str2bool(1)==True
-    with raises(Exception):
+    with raises(exceptions.CastException):
         assert casts.str2bool(0)==False
     assert casts.str2bool("true")==True
     assert casts.str2bool("True")==True
     assert casts.str2bool("false")==False
     assert casts.str2bool("False")==False
     
 
@@ -192,15 +192,16 @@
 def test_str2dtnaive():
 #    allowed=["%Y%m%d%H%M","%Y-%m-%d %H:%M:%S","%d/%m/%Y %H:%M","%d %m %H:%M %Y","%Y-%m-%d %H:%M:%S.","%H:%M:%S", '%b %d %H:%M:%S']
 
 #    assert casts.str2dtnaive("2023-11-26", "%Y-%m-%d")==datetime(2023, 11, 26)
 #    assert casts.str2dtnaive("2023-11-26 17:05:05", "%Y-%m-%d %H:%M:%S")==datetime(2023, 11, 26, 17, 5, 5)
 #    assert casts.str2dtnaive("20231126 1705", "%Y%m%d %H%M")==datetime(2023, 11, 26, 17, 5, 5)
     assert casts.str2dtnaive("202311261705", "%Y%m%d%H%M")==datetime(2023, 11, 26, 17, 5)
-#    assert casts.str2dtnaive("2023-11-26T17:05:05Z", "JsUtcIso")==datetime(2023, 11, 26, 17, 5, 5)
+    assert casts.str2dtnaive("2023-11-26T17:05:05.123456", "JsIso")==datetime(2023, 11, 26, 17, 5, 5, 123456)
+    assert casts.str2dtnaive("2023-11-26T17:05:05", "JsIso")==datetime(2023, 11, 26, 17, 5, 5)
 
 
 def test_str2dtaware():
 #    allowed=["%Y-%m-%d %H:%M:%S%z","%Y-%m-%d %H:%M:%S.%z", "JsUtcIso"]
     #assert casts.str2dtaware("2023-11-26", "%Y-%m-%d")==datetime(2023, 11, 26, tzinfo=ZoneInfo('UTC'))
     #assert casts.str2dtaware("202311261705", "%Y%m%d%H%M")==datetime(2023, 11, 26, 17, 5)
     assert casts.str2dtaware("2023-11-26T17:05:05Z", "JsUtcIso")==datetime(2023, 11, 26, 17, 5, 5, tzinfo=ZoneInfo('UTC'))
@@ -251,9 +252,9 @@
     dt_utc=datetime(2023, 11, 26, 11, 0,  tzinfo=ZoneInfo("UTC"))
     
     assert casts.dtaware_changes_tz(dt_madrid, "UTC")==dt_utc
     assert casts.dtaware_changes_tz(dt_utc, "Europe/Madrid")==dt_madrid
 
 def test_months():
     assert casts.months(2023, 11, 2024, 1)== [(2023, 11), (2023, 12), (2024, 1)]
-    assert casts.months(2023, 9)== [(2023, 9), (2023, 10), (2023, 11)]
+    assert casts.months(2023, 9,  2023, 9)== [(2023, 9)]
```

### Comparing `pydicts-0.8.0/pydicts/tests/test_lod.py` & `pydicts-0.9.0/pydicts/tests/test_lod.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.8.0/pydicts/tests/test_lod_ymv.py` & `pydicts-0.9.0/pydicts/tests/test_lod_ymv.py`

 * *Files identical despite different names*

### Comparing `pydicts-0.8.0/pydicts/tests/test_lol.py` & `pydicts-0.9.0/pydicts/tests/test_lol.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 #from datetime import datetime, date
 #from decimal import Decimal
-from pydicts import lol
-#from pytest import raises, fixture
+from pydicts import lol, exceptions
+from pytest import raises
 
 
 lol_=[]
 for i in range(10):
     lol_.append([1*i,2*i,3*i])
-    
-print(lol_)
-
 
 def test_lol_add_column():
     lol.lol_add_column(lol_, 2,  [1, 2, 3, 4, 5, 6, 7, 8, 9, 0])
+
+def test_lol_print():
+    lol.lol_print(lol_)
+    lol.lol_print(lol_,0)
+    lol.lol_print(lol_,-1)
     
-#
-#if __name__ == "__main__":
-#    def print_lor(lor):
-#        print("")
-#        for row in lor:
-#            print(row)
+def test_lol_transposed():
+    transposed=lol.lol_transposed(lol_)
+    transposed=lol.lol_transposed([])
+    with raises(exceptions.LolException):
+        transposed=lol.lol_transposed(None)
+
 #
 #    lor=[]
 #    column_to_add=[]
 #    for i in range(10):
 #        lor.append([1*i,2*i,3*i])
 #        column_to_add.append(-i)
 #    print_lor(lor)
```

### Comparing `pydicts-0.8.0/pydicts/tests/test_pylatex.py` & `pydicts-0.9.0/pydicts/tests/test_pylatex.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,30 @@
-from pydicts import pylatex
-from pylatex import Document, Section, Subsection
-from pylatex.package import Package
-from pylatex.utils import italic, NoEscape
-lod=[
-        {"year": 2022, "month": 1, "my_sum": 12},
-        {"year": 2021, "month": 2, "my_sum": 123},
-        {"year": 2019, "month": 5, "my_sum": 1},
-        {"year": 2022, "month": 12, "my_sum": 12},
-]
-def tests_pylatex_table_header():
+from shutil import which
 
-    doc = Document()
-    doc.packages.append(Package('xcolor'))
+if which("pdflatex") is not None:
+    from pydicts import pylatex
+    from pylatex import Document, Section, Subsection
+    from pylatex.package import Package
+    from pylatex.utils import italic, NoEscape
+    lod=[
+            {"year": 2022, "month": 1, "my_sum": 12},
+            {"year": 2021, "month": 2, "my_sum": 123},
+            {"year": 2019, "month": 5, "my_sum": 1},
+            {"year": 2022, "month": 12, "my_sum": 12},
+    ]
+    def tests_pylatex_table_header():
 
-    with doc.create(Section('A section')):
-        doc.append('Some regular text and some ')
-        doc.append(italic('italic text. '))
+        doc = Document()
+        doc.packages.append(Package('xcolor'))
 
-        with doc.create(Subsection('A subsection')):
-            doc.append('Also some crazy characters: $&#{}')
-            
-    doc.append(NoEscape("\\centering"))
-    pylatex.pylatex_table(doc, lod)
-    pylatex.pylatex_table(doc, [])
-    pylatex.pylatex_table_with_matched_values(doc,  [2022, 2, 12], lod, code_="|l|c|r|", match_color="teal", unmatch_color="red")
-    doc.generate_pdf('test_pylatex_table_header', clean_tex=False)
+        with doc.create(Section('A section')):
+            doc.append('Some regular text and some ')
+            doc.append(italic('italic text. '))
+
+            with doc.create(Subsection('A subsection')):
+                doc.append('Also some crazy characters: $&#{}')
+                
+        doc.append(NoEscape("\\centering"))
+        pylatex.pylatex_table(doc, lod)
+        pylatex.pylatex_table(doc, [])
+        pylatex.pylatex_table_with_matched_values(doc,  [2022, 2, 12], lod, code_="|l|c|r|", match_color="teal", unmatch_color="red")
+        doc.generate_pdf('test_pylatex_table_header', clean_tex=False)
```

### Comparing `pydicts-0.8.0/pyproject.toml` & `pydicts-0.9.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,23 @@
 [tool.poetry]
 name = "pydicts"
-version = "0.8.0"
+version = "0.9.0"
 description = "Module to use dictionaries in various situations"
 authors = ["turulomio <turulomio@yahoo.es>"]
 license = "GPL-3.0"
 readme = "README.md"
-exclude = [
-    "pydicts/devscripts.py"
-]
 
 [tool.poetry.dependencies]
-python = ">3.8"
-tabulate = "^0.9.0"
+python = ">=3.8"
+tabulate = ">=0.9.0"
+pylatex = ">=1.4.1"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.3.0"
-poethepoet = "^0.24.1"
-pylatex = "^1.4.1"
+pytest = ">=7.3.0"
+poethepoet = ">=0.24.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poe.tasks]
 release = { script = "pydicts.devscripts:release" }
```

