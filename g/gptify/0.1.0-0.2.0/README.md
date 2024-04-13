# Comparing `tmp/gptify-0.1.0.tar.gz` & `tmp/gptify-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptify-0.1.0.tar", max compression
+gzip compressed data, was "gptify-0.2.0.tar", max compression
```

## Comparing `gptify-0.1.0.tar` & `gptify-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1234 2024-04-12 06:46:54.346346 gptify-0.1.0/README.md
--rw-r--r--   0        0        0        0 2024-04-12 06:46:54.346346 gptify-0.1.0/gptify/__init__.py
--rw-r--r--   0        0        0      201 2024-04-12 06:46:54.346346 gptify-0.1.0/gptify/cli.py
--rw-r--r--   0        0        0     4550 2024-04-12 06:46:54.346346 gptify-0.1.0/gptify/gpt_repository_loader.py
--rw-r--r--   0        0        0      458 2024-04-12 06:46:54.346346 gptify-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 gptify-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1234 2024-04-13 04:25:39.535155 gptify-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-13 04:25:39.535155 gptify-0.2.0/gptify/__init__.py
+-rw-r--r--   0        0        0      201 2024-04-13 04:25:39.535155 gptify-0.2.0/gptify/cli.py
+-rw-r--r--   0        0        0     4678 2024-04-13 04:25:39.535155 gptify-0.2.0/gptify/gpt_repository_loader.py
+-rw-r--r--   0        0        0      458 2024-04-13 04:25:39.535155 gptify-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 gptify-0.2.0/PKG-INFO
```

### Comparing `gptify-0.1.0/README.md` & `gptify-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `gptify-0.1.0/gptify/gpt_repository_loader.py` & `gptify-0.2.0/gptify/gpt_repository_loader.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,52 +55,55 @@
     parser.add_argument(
         "--clipboard", help="copy the output to the clipboard", action="store_true"
     )
     parser.add_argument(
         "--openfile", help="open output file after creation", action="store_true"
     )
     parser.add_argument(
+        "--output", help="path to save output file", type=str, default="gptify_output.txt", nargs="?"
+    )
+    parser.add_argument(
         "--write-config",
         help="Write a default config file to the target directory.",
         type=str,
         nargs="?",
     )
     args = parser.parse_args()
 
     repo_path = args.repo_path or os.getcwd()
     ignore_file_path = os.path.join(repo_path, ".gptignore")
     if sys.platform == "win32":
         ignore_file_path = ignore_file_path.replace("/", "\\")
 
-    if not os.path.exists(ignore_file_path):
+    # if not os.path.exists(ignore_file_path):
         # try and use the .gptignore file in the current directory as a fallback.
-        ignore_file_path = os.path.join(HERE, ".gptignore")
-        assert os.path.exists(ignore_file_path)
-        with open(ignore_file_path, "r") as ignore_file:
-            contents = ignore_file.read()
-        with open(ignore_file_path, "w") as ignore_file:
-            ignore_file.write(contents)
+        # ignore_file_path = os.path.join(HERE, ".gptignore")
+        #assert os.path.exists(ignore_file_path)
+        # with open(ignore_file_path, "r") as ignore_file:
+        #    contents = ignore_file.read()
+        # with open(ignore_file_path, "w") as ignore_file:
+        #    ignore_file.write(contents)
 
     preamble_file = args.preamble
     if os.path.exists(ignore_file_path):
         ignore_list = get_ignore_list(ignore_file_path)
     else:
         ignore_list = []
-    outfile = os.path.abspath("gptify_output.txt")
+    outfile = os.path.abspath(args.output)
     with open(outfile, "w") as output_file:
         if preamble_file:
             with open(preamble_file, "r") as pf:
                 preamble_text = pf.read()
                 output_file.write(f"{preamble_text}\n")
         else:
             output_file.write(
                 "The following text is a Git repository with code. The structure of the text are sections that begin with ----!@#$----, followed by a single line containing the file path and file name, followed by a variable amount of lines containing the file contents. The text representing the Git repository ends when the symbols --END-- are encounted. Any further text beyond --END-- are meant to be interpreted as instructions using the aforementioned Git repository as context.\n"
             )
         process_repository(repo_path, ignore_list, output_file)
-    outfile = os.path.abspath("gptify_output.txt")
+    outfile = os.path.abspath(args.output)
     with open(outfile, "a") as output_file:
         output_file.write("--END--")
     if not args.clipboard:
         print(f"Repository contents written to {outfile}")
         if args.openfile:
             if sys.platform == "win32":
                 os.startfile(outfile)
```

### Comparing `gptify-0.1.0/PKG-INFO` & `gptify-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptify
-Version: 0.1.0
+Version: 0.2.0
 Summary: Convert code repos into an LLM prompt-friendly format. Forked from https://github.com/zackees/gptrepo
 Author: Wilder Lopes
 Author-email: wilder@ogre.run
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

