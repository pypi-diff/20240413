# Comparing `tmp/socx-0.0.8.tar.gz` & `tmp/socx-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socx-0.0.8.tar", last modified: Fri Mar  1 00:51:10 2024, max compression
+gzip compressed data, was "socx-0.0.9.tar", last modified: Sat Apr 13 14:03:03 2024, max compression
```

## Comparing `socx-0.0.8.tar` & `socx-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-01 00:51:10.478701 socx-0.0.8/
--rw-rw-rw-   0        0        0      717 2024-03-01 00:51:10.475702 socx-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      389 2024-02-18 18:52:10.000000 socx-0.0.8/README.md
--rw-rw-rw-   0        0        0      469 2024-03-01 00:50:54.000000 socx-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-01 00:51:10.478701 socx-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-01 00:51:10.399166 socx-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-03-01 00:51:10.416175 socx-0.0.8/src/socx/
--rw-rw-rw-   0        0        0       70 2024-02-18 18:56:09.000000 socx-0.0.8/src/socx/__init__.py
--rw-rw-rw-   0        0        0    19450 2024-03-01 00:35:10.000000 socx-0.0.8/src/socx/socx.py
--rw-rw-rw-   0        0        0     9451 2024-02-18 21:14:56.000000 socx-0.0.8/src/socx/util.py
-drwxrwxrwx   0        0        0        0 2024-03-01 00:51:10.471703 socx-0.0.8/src/socx.egg-info/
--rw-rw-rw-   0        0        0      717 2024-03-01 00:51:10.000000 socx-0.0.8/src/socx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-03-01 00:51:10.000000 socx-0.0.8/src/socx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-01 00:51:10.000000 socx-0.0.8/src/socx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2024-03-01 00:51:10.000000 socx-0.0.8/src/socx.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        5 2024-03-01 00:51:10.000000 socx-0.0.8/src/socx.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 14:03:03.689442 socx-0.0.9/
+-rw-rw-rw-   0        0        0      993 2024-04-13 14:03:03.687440 socx-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      665 2024-04-12 22:11:13.000000 socx-0.0.9/README.md
+-rw-rw-rw-   0        0        0      469 2024-04-13 14:02:45.000000 socx-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-13 14:03:03.690440 socx-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-13 14:03:03.641912 socx-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-04-13 14:03:03.651930 socx-0.0.9/src/socx/
+-rw-rw-rw-   0        0        0       70 2024-02-18 18:56:09.000000 socx-0.0.9/src/socx/__init__.py
+-rw-rw-rw-   0        0        0    21667 2024-04-13 13:58:52.000000 socx-0.0.9/src/socx/socx.py
+-rw-rw-rw-   0        0        0     9451 2024-02-18 21:14:56.000000 socx-0.0.9/src/socx/util.py
+drwxrwxrwx   0        0        0        0 2024-04-13 14:03:03.685439 socx-0.0.9/src/socx.egg-info/
+-rw-rw-rw-   0        0        0      993 2024-04-13 14:03:03.000000 socx-0.0.9/src/socx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-04-13 14:03:03.000000 socx-0.0.9/src/socx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 14:03:03.000000 socx-0.0.9/src/socx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2024-04-13 14:03:03.000000 socx-0.0.9/src/socx.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        5 2024-04-13 14:03:03.000000 socx-0.0.9/src/socx.egg-info/top_level.txt
```

### Comparing `socx-0.0.8/src/socx/socx.py` & `socx-0.0.9/src/socx/socx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 #!/usr/bin/env python3
-import time
-
 
 try:
     import argparse
     import os
+    import time
     import re
     import socket
     import hashlib
     import requests
     import sqlite3 as sql
     import pandas as pd
     import keyring
@@ -27,23 +26,31 @@
     python -m pip install {e.name} --trusted-host pypi.org --trusted-host pypi.python.org --trusted-host files.pythonhosted.org"""
     )
     exit(1)
 
 program_name = "socx"
 VERSION = 1.0
 about = f"""
+   _____ ____  _______  __
+  / ___// __ \/ ____/ |/ /
+  \__ \/ / / / /    |   / 
+ ___/ / /_/ / /___ /   |  
+/____/\____/\____//_/|_|  
+
 Version: {VERSION}
 A tool to assist with day to day activites in a security operations center (pronounced "socks")
 """
 
 usage = f"""Usage:
     {program_name} [universal options] [function] [options]
     python {program_name}.py [universal options] [function] [options]
-    
+        
 Examples:
+    {program_name} --help
+    {program_name} info -h
     {program_name} info -ip 1.2.3.4
     {program_name} -v 3 info -d google.com
     {program_name} search -f filename.txt -i
     {program_name} search -f fold.*name -r
     {program_name} tools --url_unwrap "https://urldefense.com/v3/__https:/..."
     
 """
@@ -66,19 +73,18 @@
     parser.add_argument(
         "-v",
         "--verbosity",
         type=int,
         default=1,
         help="The verbosity, 0 for quiet, 5 for very verbose",
     )
-    parser.add_argument(
-        "-c",
-        "--config",
-        action="store_true",
-        help="Edit the settings, keys, and variables",
+
+    # Config - Edit stored settings
+    config = subparsers.add_parser(
+        "config", help="Edit the settings, keys, and variables"
     )
 
     # Information - Online
     info = subparsers.add_parser(
         "info", help="Gather information on the specified topic"
     )
     info.add_argument("-ip", "--ip", type=str, help="An IP address")
@@ -131,14 +137,20 @@
     tools.add_argument(
         "-u",
         "--user",
         type=str,
         default="~",
         help="The user's name to use. Default is current user.",
     )
+    tools.add_argument(
+        "-r",
+        "--regex",
+        action="store_true",
+        help="Launch a regex testing environment.",
+    )
 
     args = parser.parse_args()
 
     ##########
     ## Util ##
     ##########
 
@@ -158,15 +170,15 @@
 
     def get_enironmental_variable(name):
         value = keyring.get_password("system", "_socX__" + name)
         if value is None:
             value = environmental_variables[name]
         return value
 
-    if args.config:
+    if args.function == "config":
         while True:
             p("Settings, keys, variables", v=1)
             for index, var in enumerate(environmental_variables.keys()):
                 print(f"\t{index} - {var}")
             index = input(
                 "Enter the index of the variable you want to edit (Nothing to stop): "
             )
@@ -288,21 +300,27 @@
                 vt_report_url = response.json()["data"]["links"]["self"]
 
             p(f"Getting information on {url} (unwrapped)", v=1)
 
             # Virus total get url
             if vt_api_key != "":
                 p("Waiting for Virustotal to process..", v=3)
-                time.sleep(10)
-                report_response = requests.request(
-                    "GET", url=vt_report_url, headers={"x-apikey": vt_api_key}
-                ).json()
-                print("Virustotal:", report_response["data"]["links"]["item"])
-                print("Virustotal:", report_response["data"]["attributes"]["stats"])
-                p("P.S. Run again if stats are incomplete now.", v=3)
+                for seconds in [5, 7, 10, 15]:
+                    time.sleep(seconds)
+                    report_response = requests.request(
+                        "GET", url=vt_report_url, headers={"x-apikey": vt_api_key}
+                    ).json()
+                    if report_response["data"]["attributes"]["status"] != "queued":
+                        print("Virustotal:", report_response["data"]["links"]["item"])
+                        print(
+                            "Virustotal:",
+                            report_response["data"]["attributes"]["stats"],
+                        )
+                        p("P.S. Run again if stats are incomplete now.", v=3)
+                        break
 
     ############
     ## Search ##
     ############
 
     def search(pattern, string):
         if args.insensitive:
@@ -505,10 +523,54 @@
             )
             with open(cmd_history_path, "r") as file:
                 with open(cwd + "\\powershell_history.txt", "w") as output_file:
                     for line in file:
                         output_file.write(line)
             p("Command history gathered", v=3)
 
+        elif args.regex:
+            to_match_list = []
+
+            def append_matches():
+                while True:
+                    to_match = input("Enter text to match (nothing to stop):")
+                    if to_match == "":
+                        break
+                    to_match_list.append(to_match)
+
+            to_fail_list = []
+
+            def append_failures():
+                while True:
+                    to_fail = input("Enter text to fail (nothing to stop):")
+                    if to_fail == "":
+                        break
+                    to_fail_list.append(to_fail)
+
+            def run_tests():
+                while True:
+                    success = True
+                    regex = input("Enter regex to test (nothing to stop):")
+                    if regex == "":
+                        break
+                    for to_match in to_match_list:
+                        if not re.search(regex, to_match):
+                            p(f"Failed to match: {to_match}")
+                            success = False
+                    for to_fail in to_fail_list:
+                        if re.search(regex, to_fail):
+                            p(f"Failed by matching: {to_fail}")
+                            success = False
+                    if success:
+                        p("SUCCESS")
+
+            append_matches()
+            append_failures()
+            run_tests()
+
+    if not args.function:
+        print(f"You must provide a function.")
+        print(usage)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `socx-0.0.8/src/socx/util.py` & `socx-0.0.9/src/socx/util.py`

 * *Files identical despite different names*

