# Comparing `tmp/haunts-0.7.0.tar.gz` & `tmp/haunts-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haunts-0.7.0.tar", last modified: Tue Apr  9 16:36:12 2024, max compression
+gzip compressed data, was "haunts-0.7.1.tar", last modified: Sat Apr 13 12:22:48 2024, max compression
```

## Comparing `haunts-0.7.0.tar` & `haunts-0.7.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-09 16:36:12.199000 haunts-0.7.0/
--rw-r--r--   0 keul       (501) staff       (20)      154 2024-04-09 16:36:11.000000 haunts-0.7.0/AUTHORS.rst
--rw-r--r--   0 keul       (501) staff       (20)     3512 2024-04-09 16:36:11.000000 haunts-0.7.0/CONTRIBUTING.rst
--rw-r--r--   0 keul       (501) staff       (20)     1529 2024-04-09 16:36:11.000000 haunts-0.7.0/HISTORY.rst
--rw-r--r--   0 keul       (501) staff       (20)     1520 2024-04-09 16:36:11.000000 haunts-0.7.0/LICENSE
--rw-r--r--   0 keul       (501) staff       (20)      262 2024-04-09 16:36:11.000000 haunts-0.7.0/MANIFEST.in
--rw-r--r--   0 keul       (501) staff       (20)    13213 2024-04-09 16:36:12.198907 haunts-0.7.0/PKG-INFO
--rw-r--r--   0 keul       (501) staff       (20)    10653 2024-04-09 16:36:11.000000 haunts-0.7.0/README.rst
-drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-09 16:36:12.196448 haunts-0.7.0/docs/
--rw-r--r--   0 keul       (501) staff       (20)      607 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/Makefile
--rw-r--r--   0 keul       (501) staff       (20)       28 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/authors.rst
--rwxr-xr-x   0 keul       (501) staff       (20)     4786 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/conf.py
--rw-r--r--   0 keul       (501) staff       (20)       33 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/contributing.rst
--rw-r--r--   0 keul       (501) staff       (20)    61680 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/fear-of-the-worklog.jpg
--rw-r--r--   0 keul       (501) staff       (20)       28 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/history.rst
--rw-r--r--   0 keul       (501) staff       (20)      309 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/index.rst
--rw-r--r--   0 keul       (501) staff       (20)     1108 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/installation.rst
--rw-r--r--   0 keul       (501) staff       (20)      768 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/make.bat
--rw-r--r--   0 keul       (501) staff       (20)    88743 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/pm.gif
--rw-r--r--   0 keul       (501) staff       (20)       27 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/readme.rst
--rw-r--r--   0 keul       (501) staff       (20)       73 2024-04-09 16:36:11.000000 haunts-0.7.0/docs/usage.rst
-drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-09 16:36:12.197543 haunts-0.7.0/haunts/
--rw-r--r--   0 keul       (501) staff       (20)      226 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/__init__.py
--rw-r--r--   0 keul       (501) staff       (20)      155 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/actions.py
--rw-r--r--   0 keul       (501) staff       (20)     4795 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/calendars.py
--rw-r--r--   0 keul       (501) staff       (20)     4017 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/cli.py
--rw-r--r--   0 keul       (501) staff       (20)     1664 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/credentials.py
--rw-r--r--   0 keul       (501) staff       (20)     4137 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/download.py
--rw-r--r--   0 keul       (501) staff       (20)     1268 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/ini.py
--rw-r--r--   0 keul       (501) staff       (20)     6873 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/report.py
--rw-r--r--   0 keul       (501) staff       (20)    13851 2024-04-09 16:36:11.000000 haunts-0.7.0/haunts/spreadsheet.py
-drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-09 16:36:12.198702 haunts-0.7.0/haunts.egg-info/
--rw-r--r--   0 keul       (501) staff       (20)    13213 2024-04-09 16:36:12.000000 haunts-0.7.0/haunts.egg-info/PKG-INFO
--rw-r--r--   0 keul       (501) staff       (20)      726 2024-04-09 16:36:12.000000 haunts-0.7.0/haunts.egg-info/SOURCES.txt
--rw-r--r--   0 keul       (501) staff       (20)        1 2024-04-09 16:36:12.000000 haunts-0.7.0/haunts.egg-info/dependency_links.txt
--rw-r--r--   0 keul       (501) staff       (20)       43 2024-04-09 16:36:12.000000 haunts-0.7.0/haunts.egg-info/entry_points.txt
--rw-r--r--   0 keul       (501) staff       (20)        1 2024-04-09 16:36:12.000000 haunts-0.7.0/haunts.egg-info/not-zip-safe
--rw-r--r--   0 keul       (501) staff       (20)      140 2024-04-09 16:36:12.000000 haunts-0.7.0/haunts.egg-info/requires.txt
--rw-r--r--   0 keul       (501) staff       (20)        7 2024-04-09 16:36:12.000000 haunts-0.7.0/haunts.egg-info/top_level.txt
--rw-r--r--   0 keul       (501) staff       (20)      863 2024-04-09 16:36:11.000000 haunts-0.7.0/pyproject.toml
--rw-r--r--   0 keul       (501) staff       (20)      378 2024-04-09 16:36:12.199267 haunts-0.7.0/setup.cfg
--rw-r--r--   0 keul       (501) staff       (20)     1588 2024-04-09 16:36:11.000000 haunts-0.7.0/setup.py
-drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-09 16:36:12.198536 haunts-0.7.0/tests/
--rw-r--r--   0 keul       (501) staff       (20)       36 2024-04-09 16:36:11.000000 haunts-0.7.0/tests/__init__.py
--rw-r--r--   0 keul       (501) staff       (20)      819 2024-04-09 16:36:11.000000 haunts-0.7.0/tests/test_haunts.py
+drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-13 12:22:48.120260 haunts-0.7.1/
+-rw-r--r--   0 keul       (501) staff       (20)      154 2024-04-13 12:22:47.000000 haunts-0.7.1/AUTHORS.rst
+-rw-r--r--   0 keul       (501) staff       (20)     3512 2024-04-13 12:22:47.000000 haunts-0.7.1/CONTRIBUTING.rst
+-rw-r--r--   0 keul       (501) staff       (20)     1766 2024-04-13 12:22:47.000000 haunts-0.7.1/HISTORY.rst
+-rw-r--r--   0 keul       (501) staff       (20)     1520 2024-04-13 12:22:47.000000 haunts-0.7.1/LICENSE
+-rw-r--r--   0 keul       (501) staff       (20)      262 2024-04-13 12:22:47.000000 haunts-0.7.1/MANIFEST.in
+-rw-r--r--   0 keul       (501) staff       (20)    13450 2024-04-13 12:22:48.120184 haunts-0.7.1/PKG-INFO
+-rw-r--r--   0 keul       (501) staff       (20)    10653 2024-04-13 12:22:47.000000 haunts-0.7.1/README.rst
+drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-13 12:22:48.117748 haunts-0.7.1/docs/
+-rw-r--r--   0 keul       (501) staff       (20)      607 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/Makefile
+-rw-r--r--   0 keul       (501) staff       (20)       28 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/authors.rst
+-rwxr-xr-x   0 keul       (501) staff       (20)     4786 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/conf.py
+-rw-r--r--   0 keul       (501) staff       (20)       33 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/contributing.rst
+-rw-r--r--   0 keul       (501) staff       (20)    61680 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/fear-of-the-worklog.jpg
+-rw-r--r--   0 keul       (501) staff       (20)       28 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/history.rst
+-rw-r--r--   0 keul       (501) staff       (20)      309 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/index.rst
+-rw-r--r--   0 keul       (501) staff       (20)     1108 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/installation.rst
+-rw-r--r--   0 keul       (501) staff       (20)      768 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/make.bat
+-rw-r--r--   0 keul       (501) staff       (20)    88743 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/pm.gif
+-rw-r--r--   0 keul       (501) staff       (20)       27 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/readme.rst
+-rw-r--r--   0 keul       (501) staff       (20)       73 2024-04-13 12:22:47.000000 haunts-0.7.1/docs/usage.rst
+drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-13 12:22:48.118788 haunts-0.7.1/haunts/
+-rw-r--r--   0 keul       (501) staff       (20)      226 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/__init__.py
+-rw-r--r--   0 keul       (501) staff       (20)      155 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/actions.py
+-rw-r--r--   0 keul       (501) staff       (20)     4746 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/calendars.py
+-rw-r--r--   0 keul       (501) staff       (20)     4017 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/cli.py
+-rw-r--r--   0 keul       (501) staff       (20)     1664 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/credentials.py
+-rw-r--r--   0 keul       (501) staff       (20)     4367 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/download.py
+-rw-r--r--   0 keul       (501) staff       (20)     1268 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/ini.py
+-rw-r--r--   0 keul       (501) staff       (20)     6877 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/report.py
+-rw-r--r--   0 keul       (501) staff       (20)    13955 2024-04-13 12:22:47.000000 haunts-0.7.1/haunts/spreadsheet.py
+drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-13 12:22:48.119990 haunts-0.7.1/haunts.egg-info/
+-rw-r--r--   0 keul       (501) staff       (20)    13450 2024-04-13 12:22:48.000000 haunts-0.7.1/haunts.egg-info/PKG-INFO
+-rw-r--r--   0 keul       (501) staff       (20)      726 2024-04-13 12:22:48.000000 haunts-0.7.1/haunts.egg-info/SOURCES.txt
+-rw-r--r--   0 keul       (501) staff       (20)        1 2024-04-13 12:22:48.000000 haunts-0.7.1/haunts.egg-info/dependency_links.txt
+-rw-r--r--   0 keul       (501) staff       (20)       43 2024-04-13 12:22:48.000000 haunts-0.7.1/haunts.egg-info/entry_points.txt
+-rw-r--r--   0 keul       (501) staff       (20)        1 2024-04-13 12:22:48.000000 haunts-0.7.1/haunts.egg-info/not-zip-safe
+-rw-r--r--   0 keul       (501) staff       (20)      140 2024-04-13 12:22:48.000000 haunts-0.7.1/haunts.egg-info/requires.txt
+-rw-r--r--   0 keul       (501) staff       (20)        7 2024-04-13 12:22:48.000000 haunts-0.7.1/haunts.egg-info/top_level.txt
+-rw-r--r--   0 keul       (501) staff       (20)      863 2024-04-13 12:22:47.000000 haunts-0.7.1/pyproject.toml
+-rw-r--r--   0 keul       (501) staff       (20)      378 2024-04-13 12:22:48.120514 haunts-0.7.1/setup.cfg
+-rw-r--r--   0 keul       (501) staff       (20)     1588 2024-04-13 12:22:47.000000 haunts-0.7.1/setup.py
+drwxr-xr-x   0 keul       (501) staff       (20)        0 2024-04-13 12:22:48.119824 haunts-0.7.1/tests/
+-rw-r--r--   0 keul       (501) staff       (20)       36 2024-04-13 12:22:47.000000 haunts-0.7.1/tests/__init__.py
+-rw-r--r--   0 keul       (501) staff       (20)      819 2024-04-13 12:22:47.000000 haunts-0.7.1/tests/test_haunts.py
```

### Comparing `haunts-0.7.0/CONTRIBUTING.rst` & `haunts-0.7.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `haunts-0.7.0/HISTORY.rst` & `haunts-0.7.1/HISTORY.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 History
 =======
 
+0.7.1 (2024-04-13)
+------------------
+
+- read event selection: if user is in invited list, add the event only if she/he accepted or not answered
+- read events: do not put event id (I action flag) when event cames from a linked calendar
+
+
 0.7.0 (2024-04-09)
 ------------------
 
 - Added ``read`` option to ``--execute``
 
-
 0.6.0 (2023-03-31)
 ------------------
 
 - Added ``II`` action
 
 0.5.0 (2022-12-04)
 ------------------
```

### Comparing `haunts-0.7.0/LICENSE` & `haunts-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `haunts-0.7.0/PKG-INFO` & `haunts-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haunts
-Version: 0.7.0
+Version: 0.7.1
 Summary: Fill and sync Google Calendars with events taken from a Google spreadsheet
 Home-page: https://github.com/keul/haunts
 Author: Luca Fabbri
 Author-email: l.fabbri@bopen.eu
 License: GNU General Public License v3
 Keywords: google-calendar spreadsheet reports worklog
 Classifier: Development Status :: 4 - Beta
@@ -360,20 +360,26 @@
 * gcammarota (reporting-tool-guy)
 
 
 
 History
 =======
 
+0.7.1 (2024-04-13)
+------------------
+
+- read event selection: if user is in invited list, add the event only if she/he accepted or not answered
+- read events: do not put event id (I action flag) when event cames from a linked calendar
+
+
 0.7.0 (2024-04-09)
 ------------------
 
 - Added ``read`` option to ``--execute``
 
-
 0.6.0 (2023-03-31)
 ------------------
 
 - Added ``II`` action
 
 0.5.0 (2022-12-04)
 ------------------
```

### Comparing `haunts-0.7.0/README.rst` & `haunts-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `haunts-0.7.0/docs/Makefile` & `haunts-0.7.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `haunts-0.7.0/docs/conf.py` & `haunts-0.7.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `haunts-0.7.0/docs/fear-of-the-worklog.jpg` & `haunts-0.7.1/docs/fear-of-the-worklog.jpg`

 * *Files identical despite different names*

### Comparing `haunts-0.7.0/docs/installation.rst` & `haunts-0.7.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `haunts-0.7.0/docs/make.bat` & `haunts-0.7.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `haunts-0.7.0/docs/pm.gif` & `haunts-0.7.1/docs/pm.gif`

 * *Files identical despite different names*

### Comparing `haunts-0.7.0/haunts/calendars.py` & `haunts-0.7.1/haunts/calendars.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,29 +33,26 @@
     service = build("calendar", "v3", credentials=creds)
 
     from_time = from_time or get("START_TIME", "09:00")
     start = datetime.datetime.strptime(
         f"{date.strftime('%Y-%m-%d')}T{from_time}:00Z",
         "%Y-%m-%dT%H:%M:%SZ",
     )
-    print(start)
 
     startParams = None
     endParams = None
-    haveLength = length is not None and type(length) is not str
+    haveLength = length is not None and not isinstance(length, str)
     duration = None
     if haveLength:
         duration = float(length)
         delta = datetime.timedelta(hours=duration)
     else:
         delta = datetime.timedelta(hours=0)
     end = start + delta
 
-    print(start.isoformat() + "Z")
-
     if haveLength:
         # Event with a duration
         startParams = {
             "dateTime": start.isoformat(),
             "timeZone": get("TIMEZONE", "Etc/GMT"),
         }
         endParams = {
```

### Comparing `haunts-0.7.0/haunts/cli.py` & `haunts-0.7.1/haunts/cli.py`

 * *Files identical despite different names*

### Comparing `haunts-0.7.0/haunts/credentials.py` & `haunts-0.7.1/haunts/credentials.py`

 * *Files identical despite different names*

### Comparing `haunts-0.7.0/haunts/download.py` & `haunts-0.7.1/haunts/download.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,15 +21,17 @@
     USER_EMAIL = get("USER_EMAIL")
     if USER_EMAIL is None:
         raise KeyError("USER_EMAIL not set in configuration")
     for event in events:
         if event.get("creator", {}).get("email") == USER_EMAIL:
             yield event
         elif USER_EMAIL in [
-            attendee.get("email") for attendee in event.get("attendees", [])
+            attendee.get("email")
+            for attendee in event.get("attendees", [])
+            if attendee.get("responseStatus") in ["accepted", "needsAction"]
         ]:
             yield event
 
 
 def get_events_at(events_service, calendar_id, date):
     """Get all events from a calendar in a specific date."""
     start_datetime = datetime.combine(date, datetime.min.time()).isoformat() + "Z"
@@ -83,33 +85,34 @@
         new_events = [
             e for e in filter_my_event(events) if e["id"] not in already_added_events
         ]
         already_added_events.update([e["id"] for e in new_events])
         all_events.extend(new_events)
 
     # Get calendar configurations
-    calendar_names = get_calendars_names(sheet_service)
+    calendar_names = get_calendars_names(sheet_service, flat=False)
 
     # Main operation loop
     for event in all_events:
         event_summary = event.get("summary", "No summary")
         start = event["start"].get("dateTime", event["start"].get("date"))
         end = event["end"].get("dateTime", event["end"].get("date"))
-        project = calendar_names[event["calendar_id"]]
+        project = calendar_names[event["calendar_id"]]["alias"]
+        is_linked = calendar_names[event["calendar_id"]]["is_linked"]
 
         start_date = datetime.fromisoformat(start).date()
         start_time = datetime.fromisoformat(start).time()
         duration = datetime.fromisoformat(end) - datetime.fromisoformat(start)
         click.echo(f"Adding new event {event_summary} ({project}) to selected sheet")
         append_line(
             sheet_service,
             sheet,
             date_col=start_date,
             time_col=start_time,
             duration_col=duration,
             project_col=project,
             activity_col=event_summary,
             details_col=event.get("description", ""),
-            event_id_col=event["id"],
+            event_id_col=event["id"] if not is_linked else "",
             link_col=event.get("htmlLink", ""),
-            action_col="I",
+            action_col="I" if not is_linked else "",
         )
```

### Comparing `haunts-0.7.0/haunts/ini.py` & `haunts-0.7.1/haunts/ini.py`

 * *Files identical despite different names*

### Comparing `haunts-0.7.0/haunts/report.py` & `haunts-0.7.1/haunts/report.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         spent = get_col(row, headers_id["Spent"])
 
         # We have a value of spent hours in this event
         if isinstance(spent, numbers.Number):
             prog_stats["total"] += spent
             if in_overtime:
                 prog_stats["overtime"] += spent
-        elif type(spent) == str and not spent:
+        elif isinstance(spent, str) and not spent:
             # Check: we have multiple full days in the same day! haunts is not supporting this
             if date_stats["have_full_day"]:
                 click.echo(
                     Back.YELLOW
                     + Fore.BLACK
                     + f"There are multiple full days in the same day: {str(date)}"
                     + Style.RESET_ALL
```

### Comparing `haunts-0.7.0/haunts/spreadsheet.py` & `haunts-0.7.1/haunts/spreadsheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -259,18 +259,18 @@
             id in configured_calendars or read_from in configured_calendars
         ):
             continue
         configured_calendars[alias] = read_from or id
     return configured_calendars
 
 
-def get_calendars_names(sheet):
+def get_calendars_names(sheet, flat=True):
     """Get all calendars names, giving precedence to alias defined in column "linked_calendar".
 
-    If aliases are found, the first one will be used
+    If multiple aliases are found, the first one will be used
     """
     RANGE = f"{get('CONTROLLER_SHEET_NAME', 'config')}!A2:C"
     calendars = (
         sheet.values()
         .get(spreadsheetId=get("CONTROLLER_SHEET_DOCUMENT_ID"), range=RANGE)
         .execute()
     )
@@ -281,15 +281,17 @@
             id, alias, linked_id = cols
         except ValueError:
             # no linked_id
             id, alias = cols
             linked_id = None
         if names.get(linked_id) or (names.get(id) and not linked_id):
             continue
-        names[linked_id or id] = alias
+        names[linked_id or id] = (
+            alias if flat else {"alias": alias, "is_linked": bool(linked_id)}
+        )
     return names
 
 
 def get_first_empty_line(sheet, month):
     """Get the first empty line in a month."""
     RANGE = f"{month}!A1:A"
     lines = (
```

### Comparing `haunts-0.7.0/haunts.egg-info/PKG-INFO` & `haunts-0.7.1/haunts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: haunts
-Version: 0.7.0
+Version: 0.7.1
 Summary: Fill and sync Google Calendars with events taken from a Google spreadsheet
 Home-page: https://github.com/keul/haunts
 Author: Luca Fabbri
 Author-email: l.fabbri@bopen.eu
 License: GNU General Public License v3
 Keywords: google-calendar spreadsheet reports worklog
 Classifier: Development Status :: 4 - Beta
@@ -360,20 +360,26 @@
 * gcammarota (reporting-tool-guy)
 
 
 
 History
 =======
 
+0.7.1 (2024-04-13)
+------------------
+
+- read event selection: if user is in invited list, add the event only if she/he accepted or not answered
+- read events: do not put event id (I action flag) when event cames from a linked calendar
+
+
 0.7.0 (2024-04-09)
 ------------------
 
 - Added ``read`` option to ``--execute``
 
-
 0.6.0 (2023-03-31)
 ------------------
 
 - Added ``II`` action
 
 0.5.0 (2022-12-04)
 ------------------
```

### Comparing `haunts-0.7.0/haunts.egg-info/SOURCES.txt` & `haunts-0.7.1/haunts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `haunts-0.7.0/pyproject.toml` & `haunts-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `haunts-0.7.0/setup.py` & `haunts-0.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,10 +47,10 @@
     include_package_data=True,
     keywords="google-calendar spreadsheet reports worklog",
     name="haunts",
     packages=find_packages(include=["haunts", "haunts.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/keul/haunts",
-    version="0.7.0",
+    version="0.7.1",
     zip_safe=False,
 )
```

### Comparing `haunts-0.7.0/tests/test_haunts.py` & `haunts-0.7.1/tests/test_haunts.py`

 * *Files identical despite different names*

