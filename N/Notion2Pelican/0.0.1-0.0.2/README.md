# Comparing `tmp/Notion2Pelican-0.0.1-py3-none-any.whl.zip` & `tmp/Notion2Pelican-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 8219 bytes, number of entries: 8
--rw-rw-rw-  2.0 fat     6724 b- defN 24-Mar-26 20:28 Notion2Pelican/Notion2Pelican.py
--rw-rw-rw-  2.0 fat       23 b- defN 24-Mar-26 19:27 Notion2Pelican/__init__.py
+Zip file size: 8763 bytes, number of entries: 8
+-rw-rw-rw-  2.0 fat     8640 b- defN 24-Apr-13 12:56 Notion2Pelican/Notion2Pelican.py
+-rw-rw-rw-  2.0 fat       23 b- defN 24-Apr-13 13:07 Notion2Pelican/__init__.py
 -rw-rw-rw-  2.0 fat     7242 b- defN 24-Mar-26 18:59 Notion2Pelican/notion2md.py
--rw-rw-rw-  2.0 fat     1085 b- defN 24-Mar-29 07:14 Notion2Pelican-0.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3969 b- defN 24-Mar-29 07:14 Notion2Pelican-0.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Mar-29 07:14 Notion2Pelican-0.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       15 b- defN 24-Mar-29 07:14 Notion2Pelican-0.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      675 b- defN 24-Mar-29 07:14 Notion2Pelican-0.0.1.dist-info/RECORD
-8 files, 19825 bytes uncompressed, 7031 bytes compressed:  64.5%
+-rw-rw-rw-  2.0 fat     1085 b- defN 24-Apr-13 13:12 Notion2Pelican-0.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     4279 b- defN 24-Apr-13 13:12 Notion2Pelican-0.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-13 13:12 Notion2Pelican-0.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       15 b- defN 24-Apr-13 13:12 Notion2Pelican-0.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      675 b- defN 24-Apr-13 13:12 Notion2Pelican-0.0.2.dist-info/RECORD
+8 files, 22051 bytes uncompressed, 7575 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: Notion2Pelican/__init__.py
 Comment: 
 
 Filename: Notion2Pelican/notion2md.py
 Comment: 
 
-Filename: Notion2Pelican-0.0.1.dist-info/LICENSE
+Filename: Notion2Pelican-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: Notion2Pelican-0.0.1.dist-info/METADATA
+Filename: Notion2Pelican-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: Notion2Pelican-0.0.1.dist-info/WHEEL
+Filename: Notion2Pelican-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: Notion2Pelican-0.0.1.dist-info/top_level.txt
+Filename: Notion2Pelican-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: Notion2Pelican-0.0.1.dist-info/RECORD
+Filename: Notion2Pelican-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Notion2Pelican/Notion2Pelican.py

```diff
@@ -1,8 +1,9 @@
 import json
+from os.path import abspath, join, pardir
 import requests
 import re
 
 
 def get_notion_headers(token):
     """ gives the headers as needed by Notion API
 
@@ -19,63 +20,68 @@
         "Authorization": "Bearer " + token,
         "Content-Type": "application/json",
         "Notion-Version": "2022-06-28"
         }
     return headers
 
 
-def readDatabase(databaseId, notion_header, print_res=False):
+def readDatabase(databaseId, notion_header, print_res=False, fp=None):
     """ reads the database (identified by Notion with databaseId) and returns the structure as a json
 
     Parameters
     -----------
     databaseId: str
         notion id
     notion_header: json
         header sent via REST url
     print_res: bool
         if True prints debug messages
+    fp: str
+        file path where the json result should be saved, defaults to "db.json"
 
     Returns
     -------
     data: json
         Data structure returned by the Notion API
 
     Documentation:
     --------------
     curl https://api.notion.com/v1/blocks/16d8004e-5f6a-42a6-9811-51c22ddada12/children?page_size=100 \  # noqa E501
     -H 'Authorization: Bearer '"$NOTION_API_KEY"'' \
     -H "Notion-Version: 2022-06-28"
     """
     read_url = f"https://api.notion.com/v1/blocks/{databaseId}/children?page_size=100"  # noqa E501
+    if fp is None:
+        fp = abspath(join(__file__, pardir, "db.json"))
 
     res = requests.request("GET", read_url, headers=notion_header)
     data = res.json()
     html_response = res.status_code
 
     if html_response == 200:  # res.status_code
-        with open('./db.json', 'w', encoding='utf8') as f:
+        with open(fp, 'w', encoding='utf8') as f:
             f.write(json.dumps(data, indent=4))
         if print_res:
             print("print res >>>>>>>>>>>>>")
             print(json.dumps(data, indent=4))
             print("print res <<<<<<<<<<<<<<")
     return data
 
 
-def page_tree_ids(res, headers):
+def page_tree_ids(res, headers, fp=None):
     """ parses the Notion DB json into a tree
 
     Parameters
     ----------
     res: json
         json returned by NOTION API
     headers: json
         headers used for parameters in REST API
-
+    fp: str
+        file path where the json result should be saved, defaults to "db.json"
     Returns
     -------
     children_ids : list of dict
         each dict is a page title, page id and list of children
     """
 
     children_ids = []
@@ -88,14 +94,18 @@
                 page_title = b["child_page"]["title"]
                 res1 = readDatabase(id1, headers, print_res=False)
                 children = page_tree_ids(res1, headers)
                 children_page = {"title": page_title, "id": id1,
                                  "children": children}
                 children_ids.append(children_page)
 
+    if fp is None:
+        fp = abspath(join(__file__, pardir, "page_id.json"))
+    with open(fp, "w", encoding="utf-8") as fo:
+        fo.write(json.dumps(children_ids, indent=4))
     return children_ids
 
 
 def para_2_md(paragraph):
     """ Convets Notion Paragraph to markdown string
 
     Parameters
@@ -104,49 +114,64 @@
         dict of various values from notion paragraph definition
 
     Returns
     -------
     md: str
         markdown encoded in string version of the paragrap
     """
-    md = "\n"
+    md = ""
 
     for para in paragraph:
         if para == "rich_text":
             for para_block in paragraph[para]:
                 if "text" in para_block:
                     content = para_block["text"]["content"]
                     if para_block["text"]["link"] is not None:
                         link = para_block["text"]["link"]["url"]
                         md += f"[{content}]({link})"
                     else:
-                        md += f"{content}"
+                        # md += f"{content}"
+                        raw_content = content
+                        for annotation in para_block["annotations"]:
+                            if para_block["annotations"][annotation]:
+                                if annotation == "bold":
+                                    raw_content = f"**{raw_content}**"
+                                elif annotation == "italic":
+                                    raw_content = f"*{raw_content}*"
+                                elif annotation == "strikethrough":
+                                    raw_content = f"~~{raw_content}~~"
+                                elif annotation == "underline":
+                                    raw_content = f"__{raw_content}__"
+                        md += raw_content
                 if "mention" in para_block:
                     plain_text = para_block["plain_text"]
                     url = para_block["href"]
                     md += f"[{plain_text}]({url})"
-    md += "\n"
+    # md += "\n"
     return md
 
 
-def pageid_2_md(front_matter, res):
+def pageid_2_md(front_matter, res, debug=False):
     """ generates markdown with front matter from notion json
 
     Parameters
     ----------
     front_matter: json
         the page title as the title is not in the json object
     res: json
         json returned by the NOTION API
 
     Returns
     --------
     md: str
         Markdown formatted page
     """
+
+    known_btype = ["heading_1", "heading_2", "paragraph", "bulleted_list_item", "numbered_list_item", "image"]
+
     # FIXME: 56c2ac88fa7c49d8859c44ce68eca68b
 
     if "status" not in front_matter:
         front_matter["status"] = "published"
 
     md = f"""---
 title: {front_matter['title']}
@@ -159,44 +184,56 @@
 
 """
 
     md += f"# {front_matter['title']}\n\n"
     prev_btype = ""
 
     for block in res["results"]:
-        # print(block["type"])
         btype = block["type"]
-        bullet_index = 0
+        if debug:
+            print("btype", btype)
+        md_txt = para_2_md(block[btype])
+
+        if btype != "numbered_list_item":
+            bullet_index = 0
+        
         if btype == "paragraph":  # in block:
-            md += para_2_md(block[btype])
+            md += f"\n{md_txt}\n"
+        elif btype == "heading_1":
+            md += f"\n# {md_txt}\n\n"
         elif btype == "heading_2":  # in block:
             """ "heading_2": {
                     "rich_text": [
                         {
                             "type": "text",
                             "text": {
                                 "content": """
-            head2 = block["heading_2"]["rich_text"][0]["text"]["content"]
+            head2 = md_txt # block["heading_2"]["rich_text"][0]["text"]["content"]
             # print("head2",head2)
             md += f"\n## {head2}\n\n"
         elif btype == "heading_3":  # in block:
-            head3 = block["heading_3"]["rich_text"][0]["text"]["content"]
+            head3 = md_txt # block["heading_3"]["rich_text"][0]["text"]["content"]
             # print("head2",head2)
             md += f"\n### {head3}\n\n"
         elif btype == "bulleted_list_item":
             # bull = block[btype]["rich_text"]
-            bulletpoint = block[btype]["rich_text"][0]["text"]["content"]
+            bulletpoint = md_txt #block[btype]["rich_text"][0]["text"]["content"]
             md += f"* {bulletpoint}\n"
         elif btype == "numbered_list_item":
-            bulletpoint = block[btype]["rich_text"][0]["text"]["content"]
+            bulletpoint = md_txt #block[btype]["rich_text"][0]["text"]["content"]
+            # print("!!!!!!!!!!!!!", prev_btype, btype, bullet_index)
             if prev_btype == btype:
                 bullet_index += 1
+                md += f"{bullet_index}. {bulletpoint}\n"
             else:
                 bullet_index = 1
-            md += f"{bullet_index}. {bulletpoint}\n"
+                md += f"\n{bullet_index}. {bulletpoint}\n"
+        elif btype == "quote":
+            quote_text = md_txt  # block[btype]["rich_text"][0]["text"]["content"]
+            md += f"\n> {quote_text}\n"
         elif btype == "image":
             caption = ""
             for c in block["image"]["caption"]:
                 caption += c["plain_text"]
             url = block["image"][block["image"]["type"]]["url"]
             img = f"![{caption}]({url})\n\n"
             md += img
```

## Notion2Pelican/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "0.0.1"
+__version__ = "0.0.2"
```

## Comparing `Notion2Pelican-0.0.1.dist-info/LICENSE` & `Notion2Pelican-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `Notion2Pelican-0.0.1.dist-info/METADATA` & `Notion2Pelican-0.0.2.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Notion2Pelican
-Version: 0.0.1
+Version: 0.0.2
 Summary: Import notion pages in pelican blogging format
 Home-page: https://github.com/oberron/Notion2Pelican
 Author: oberron
 Author-email: one.annum@gmail.com
 License: LICENSE
 Project-URL: Bug Tracker, https://github.com/oberron/Notion2Pelican/issues
 Keywords: Notion Pelican
@@ -68,15 +68,23 @@
 
 > cd docs
 > python example.py
 
 
 ## Release Notes and Roadmap
 
-### v0.0.1 (first release)
+v0.0.2 - adding support for
+
+* add support for H1 (which was not present)
+* numbered list (which was not working)
+* italic and bold (which was not available)
+* non regression for images (though it was working)
+* add support for quotes
+
+v0.0.1 (first release)
 
 Supports:
 
 * Titles (H1, H2, )
 * Bulleted items
 * images 
 
@@ -129,15 +137,15 @@
 
 > twine upload -r testpypi dist\*
 
 10. check updates on read_the_docs
 
 11. check on google colab it works
 
-12. release on pypi
-> twine upload -r pypi dist\*
+12. release on pypi (assumes your pypirc is local to the project)
+> twine upload -r pypi --config-file=.\.pypirc dist\*
 
 13. check on colab that pypi package works:
 
 >!python -m pip install Notion2Pelican
 from Notion2Pelican import __version__
 print(__version__)
```

## Comparing `Notion2Pelican-0.0.1.dist-info/RECORD` & `Notion2Pelican-0.0.2.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Notion2Pelican/Notion2Pelican.py,sha256=kdY01dPn7c474S8w5BLps_bLOKpwU-1qo6tTkglxXSM,6724
-Notion2Pelican/__init__.py,sha256=ry5O5SW74ugwOUMKSV2_LbWjYa8B0IEvUm7S-lHPA2c,23
+Notion2Pelican/Notion2Pelican.py,sha256=WZKB0M1mggAdLYq6S5mPscQJw-YeOF_TNB-h-QaeMKo,8640
+Notion2Pelican/__init__.py,sha256=j7895T8JfsWQAOvxm8SAdESs5iFmIuAqKpyfjSAfKZ4,23
 Notion2Pelican/notion2md.py,sha256=0doPGW6-qflmBNoemZ-wjL0r4ZsJqjQY21BN50dUwUM,7242
-Notion2Pelican-0.0.1.dist-info/LICENSE,sha256=Fn3cwvKKiiE3szx4MfhsP3Onsx25i8Fr2a7iJ7yMZBg,1085
-Notion2Pelican-0.0.1.dist-info/METADATA,sha256=wjRL8Y1iMm5D_rnIlId2Dg0hpO9LtcONCwdmsOFhFeI,3969
-Notion2Pelican-0.0.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-Notion2Pelican-0.0.1.dist-info/top_level.txt,sha256=ajK76CzagnB5dN-ombUkwmeUPuH0dRY9LlTmMzaTqlY,15
-Notion2Pelican-0.0.1.dist-info/RECORD,,
+Notion2Pelican-0.0.2.dist-info/LICENSE,sha256=Fn3cwvKKiiE3szx4MfhsP3Onsx25i8Fr2a7iJ7yMZBg,1085
+Notion2Pelican-0.0.2.dist-info/METADATA,sha256=8uA_NEYN-xkdC2EkIzZjsbl9DygyL9DxXtzGowWu0dw,4279
+Notion2Pelican-0.0.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+Notion2Pelican-0.0.2.dist-info/top_level.txt,sha256=ajK76CzagnB5dN-ombUkwmeUPuH0dRY9LlTmMzaTqlY,15
+Notion2Pelican-0.0.2.dist-info/RECORD,,
```

