# Comparing `tmp/kgr-0.1.5.tar.gz` & `tmp/kgr-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgr-0.1.5.tar", last modified: Wed Apr 10 16:09:37 2024, max compression
+gzip compressed data, was "kgr-0.1.6.tar", last modified: Fri Apr 12 23:28:02 2024, max compression
```

## Comparing `kgr-0.1.5.tar` & `kgr-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1074 2024-04-10 14:38:49.000000 kgr-0.1.5/LICENSE
--rw-r--r--   0        0        0        0 2024-04-10 14:34:29.000000 kgr-0.1.5/README.md
--rw-r--r--   0        0        0      692 2024-04-10 16:09:37.135089 kgr-0.1.5/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-10 14:21:46.000000 kgr-0.1.5/src/kgr/__init__.py
--rw-r--r--   0        0        0       30 2024-04-10 16:04:38.945223 kgr-0.1.5/src/kgr/__main__.py
--rw-r--r--   0        0        0     8943 2024-04-10 16:09:11.599821 kgr-0.1.5/src/kgr/lib.py
--rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 kgr-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-10 14:38:49.000000 kgr-0.1.6/LICENSE
+-rw-r--r--   0        0        0        0 2024-04-10 14:34:29.000000 kgr-0.1.6/README.md
+-rw-r--r--   0        0        0      692 2024-04-12 23:28:02.843710 kgr-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0   205566 2024-04-12 23:26:08.681521 kgr-0.1.6/src/kgr/KGR - Potential victims.csv
+-rw-r--r--   0        0        0        0 2024-04-10 14:21:46.000000 kgr-0.1.6/src/kgr/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-12 23:27:35.713698 kgr-0.1.6/src/kgr/__main__.py
+-rw-r--r--   0        0        0     8952 2024-04-12 23:19:33.588135 kgr-0.1.6/src/kgr/lib.py
+-rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 kgr-0.1.6/PKG-INFO
```

### Comparing `kgr-0.1.5/LICENSE` & `kgr-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kgr-0.1.5/pyproject.toml` & `kgr-0.1.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "kgr"
-version = "0.1.5"
+version = "0.1.6"
 dependencies = [
     "requests",
     "geopy",
     "bs4",
 ]
 authors = [
     { name = "Dmitry Luschan", email = "dluschan@gmail.com" },
```

### Comparing `kgr-0.1.5/src/kgr/lib.py` & `kgr-0.1.6/src/kgr/lib.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,20 +19,21 @@
 	description = description_tag.text.strip().replace("""
 """, "").replace("""\r""", " ").replace("  ", " ").replace("  ", " ")
 	img = soup.select_one('div.human-dossier-card__img > img').get("src")
 	return description, img
 
 
 def parse_raw_data(data: list, args):
+	width = len(str(len(data)))
 	for i, row in enumerate(data, 1):
 		try:
 			row["city"] = ""
 			row["description"], row["img_src"] = get_description_and_img(row["Полная информация"])
 			if args.verbosity > 0 and i % 10 == 0 or args.verbosity > 1:
-				print(f"Done. {i}/{len(data)}")
+				print(f"Done: {i:>{width}d}/{len(data)}")
 		except AssertionError:
 			row["city"], row["description"], row["img_src"] = "", "", ""
 			if not args.quiet:
 				print(*row, file=args.error)
 
 
 def get_geocode(city: str, app) -> str:
@@ -56,15 +57,15 @@
 			row["lon"], row["lat"] = 0, 0
 			if not args.quiet:
 				print(f"""{row["ФИО"]}""", file=args.error)
 			errors += 1
 		finally:
 			row["WKT"] = f"""POINT ({row["lon"]} {row["lat"]})"""
 			if args.verbosity > 0 and i % 10 == 0 or args.verbosity > 1:
-				print(f"Done:{i: {width}d}/{len(data)}")
+				print(f"Done: {i:>{width}d}/{len(data)}")
 	return errors
 
 
 def read_data(args):
 	return list(DictReader(open(args.input, newline=''), delimiter=args.delimiter))
 
 
@@ -158,16 +159,16 @@
 	convert_parser.add_argument("-s", "--suffix", help="the phrase added to the description of each person")
 	convert_parser.add_argument("-l", "--layout", help="the internal name of the xml document and the name of the layer on the map")
 
 	return parser
 
 
 def prepare(args):
-	if args.output is None:
-		args.output = args.input.replace(".csv", ".kml")
+	if args.replace:
+		args.output = args.input
 	data = read_data(args)
 	assert len(data), "Empty data"
 	assert "ФИО" in data[0].keys(), """Error: Missing column "ФИО"! """
 	assert "Полная информация" in data[0].keys(), """Error: Missing column "Полная информация"! """
 	parse_raw_data(data, args)
 	write_data(data, args)
```

### Comparing `kgr-0.1.5/PKG-INFO` & `kgr-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kgr
-Version: 0.1.5
+Version: 0.1.6
 Summary: Miltitool for convert data from https://memopzk.org to Google Maps
 Author-Email: Dmitry Luschan <dluschan@gmail.com>
 Maintainer-Email: Dmitry Luschan <dluschan@gmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

