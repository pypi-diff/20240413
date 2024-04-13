# Comparing `tmp/pubmed_parser-0.3.1.tar.gz` & `tmp/pubmed_parser-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pubmed_parser-0.3.1.tar", last modified: Mon Nov 22 12:19:38 2021, max compression
+gzip compressed data, was "pubmed_parser-0.4.0.tar", last modified: Sat Apr 13 12:19:02 2024, max compression
```

## Comparing `pubmed_parser-0.3.1.tar` & `pubmed_parser-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxr-xr-x   0 titipata   (501) staff       (20)        0 2021-11-22 12:19:38.000000 pubmed_parser-0.3.1/
--rw-r--r--   0 titipata   (501) staff       (20)     1101 2020-01-23 04:33:16.000000 pubmed_parser-0.3.1/LICENSE
--rw-r--r--   0 titipata   (501) staff       (20)     1363 2021-11-22 12:19:38.000000 pubmed_parser-0.3.1/PKG-INFO
--rw-r--r--   0 titipata   (501) staff       (20)    15165 2021-11-22 12:17:57.000000 pubmed_parser-0.3.1/README.md
-drwxr-xr-x   0 titipata   (501) staff       (20)        0 2021-11-22 12:19:38.000000 pubmed_parser-0.3.1/pubmed_parser/
--rw-r--r--   0 titipata   (501) staff       (20)      561 2021-11-22 12:19:06.000000 pubmed_parser-0.3.1/pubmed_parser/__init__.py
--rw-r--r--   0 titipata   (501) staff       (20)    23598 2021-11-22 12:17:57.000000 pubmed_parser-0.3.1/pubmed_parser/medline_parser.py
--rw-r--r--   0 titipata   (501) staff       (20)    18577 2021-11-22 12:17:57.000000 pubmed_parser-0.3.1/pubmed_parser/pubmed_oa_parser.py
--rw-r--r--   0 titipata   (501) staff       (20)    13543 2020-01-28 13:58:05.000000 pubmed_parser-0.3.1/pubmed_parser/pubmed_web_parser.py
--rw-r--r--   0 titipata   (501) staff       (20)     4118 2021-06-16 14:26:04.000000 pubmed_parser-0.3.1/pubmed_parser/utils.py
-drwxr-xr-x   0 titipata   (501) staff       (20)        0 2021-11-22 12:19:38.000000 pubmed_parser-0.3.1/pubmed_parser.egg-info/
--rw-r--r--   0 titipata   (501) staff       (20)     1363 2021-11-22 12:19:38.000000 pubmed_parser-0.3.1/pubmed_parser.egg-info/PKG-INFO
--rw-r--r--   0 titipata   (501) staff       (20)      360 2021-11-22 12:19:38.000000 pubmed_parser-0.3.1/pubmed_parser.egg-info/SOURCES.txt
--rw-r--r--   0 titipata   (501) staff       (20)        1 2021-11-22 12:19:38.000000 pubmed_parser-0.3.1/pubmed_parser.egg-info/dependency_links.txt
--rw-r--r--   0 titipata   (501) staff       (20)       52 2021-11-22 12:19:38.000000 pubmed_parser-0.3.1/pubmed_parser.egg-info/requires.txt
--rw-r--r--   0 titipata   (501) staff       (20)       14 2021-11-22 12:19:38.000000 pubmed_parser-0.3.1/pubmed_parser.egg-info/top_level.txt
--rw-r--r--   0 titipata   (501) staff       (20)       38 2021-11-22 12:19:38.000000 pubmed_parser-0.3.1/setup.cfg
--rw-r--r--   0 titipata   (501) staff       (20)     2020 2021-11-22 12:18:56.000000 pubmed_parser-0.3.1/setup.py
+drwxr-xr-x   0 titipata   (501) staff       (20)        0 2024-04-13 12:19:02.497761 pubmed_parser-0.4.0/
+-rw-r--r--   0 titipata   (501) staff       (20)     1101 2024-04-13 12:05:04.000000 pubmed_parser-0.4.0/LICENSE
+-rw-r--r--   0 titipata   (501) staff       (20)    16859 2024-04-13 12:19:02.497513 pubmed_parser-0.4.0/PKG-INFO
+-rw-r--r--   0 titipata   (501) staff       (20)    15308 2024-04-13 12:05:04.000000 pubmed_parser-0.4.0/README.md
+drwxr-xr-x   0 titipata   (501) staff       (20)        0 2024-04-13 12:19:02.495660 pubmed_parser-0.4.0/pubmed_parser/
+-rw-r--r--   0 titipata   (501) staff       (20)      549 2024-04-13 12:07:10.000000 pubmed_parser-0.4.0/pubmed_parser/__init__.py
+-rw-r--r--   0 titipata   (501) staff       (20)    25027 2024-04-13 12:05:04.000000 pubmed_parser-0.4.0/pubmed_parser/medline_parser.py
+-rw-r--r--   0 titipata   (501) staff       (20)    18736 2024-04-13 12:05:04.000000 pubmed_parser-0.4.0/pubmed_parser/pubmed_oa_parser.py
+-rw-r--r--   0 titipata   (501) staff       (20)    13709 2024-04-13 12:05:04.000000 pubmed_parser-0.4.0/pubmed_parser/pubmed_web_parser.py
+-rw-r--r--   0 titipata   (501) staff       (20)     4118 2024-04-13 12:05:04.000000 pubmed_parser-0.4.0/pubmed_parser/utils.py
+drwxr-xr-x   0 titipata   (501) staff       (20)        0 2024-04-13 12:19:02.497254 pubmed_parser-0.4.0/pubmed_parser.egg-info/
+-rw-r--r--   0 titipata   (501) staff       (20)    16859 2024-04-13 12:19:02.000000 pubmed_parser-0.4.0/pubmed_parser.egg-info/PKG-INFO
+-rw-r--r--   0 titipata   (501) staff       (20)      452 2024-04-13 12:19:02.000000 pubmed_parser-0.4.0/pubmed_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 titipata   (501) staff       (20)        1 2024-04-13 12:19:02.000000 pubmed_parser-0.4.0/pubmed_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 titipata   (501) staff       (20)       52 2024-04-13 12:19:02.000000 pubmed_parser-0.4.0/pubmed_parser.egg-info/requires.txt
+-rw-r--r--   0 titipata   (501) staff       (20)       14 2024-04-13 12:19:02.000000 pubmed_parser-0.4.0/pubmed_parser.egg-info/top_level.txt
+-rw-r--r--   0 titipata   (501) staff       (20)       38 2024-04-13 12:19:02.497823 pubmed_parser-0.4.0/setup.cfg
+-rw-r--r--   0 titipata   (501) staff       (20)     2205 2024-04-13 12:08:02.000000 pubmed_parser-0.4.0/setup.py
+drwxr-xr-x   0 titipata   (501) staff       (20)        0 2024-04-13 12:19:02.496984 pubmed_parser-0.4.0/tests/
+-rw-r--r--   0 titipata   (501) staff       (20)    14358 2024-04-13 12:05:04.000000 pubmed_parser-0.4.0/tests/test_medline_parser.py
+-rw-r--r--   0 titipata   (501) staff       (20)     2996 2024-04-13 12:05:04.000000 pubmed_parser-0.4.0/tests/test_pubmed_oa_parser.py
+-rw-r--r--   0 titipata   (501) staff       (20)     4562 2024-04-13 12:05:04.000000 pubmed_parser-0.4.0/tests/test_pubmed_web_parser.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pubmed_parser-0.3.1/LICENSE` & `pubmed_parser-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pubmed_parser-0.3.1/README.md` & `pubmed_parser-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,16 @@
 * `journal` : journal of the given paper
 * `medline_ta` : this is abbreviation of the journal name
 * `nlm_unique_id` : NLM unique identification
 * `issn_linking` : ISSN linkage, typically use to link with Web of Science dataset
 * `country` : Country extracted from journal information field
 * `reference` : string of PMID each separated by `;` or list of references made to the article
 * `delete` : boolean if `False` means paper got updated so you might have two
+* `languages` : list of languages, separated by `;`
+* `vernacular_title`: vernacular title. Defaults to empty string whenever non-available.
 
 XMLs for the same paper. You can delete the record of deleted paper because it got updated.
 
 ``` python
 dicts_out = pp.parse_medline_xml('data/medline16n0902.xml.gz',
                                  year_info_only=False,
                                  nlm_category=False,
@@ -220,15 +222,15 @@
 Identifiers should be passed as strings. PubMed Central ID's are default, and should be passed as strings *without* the `'PMC'` prefix. If no citations are found, or if no article is found matching `doc_id` in the indicated database, it will return `None`.
 
 ## Installation
 
 You can install the most update version of the package directly from the repository
 
 ``` bash
-pip install git+git://github.com/titipata/pubmed_parser.git
+pip install git+https://github.com/titipata/pubmed_parser.git
 ```
 
 or install recent release with [PyPI](https://pypi.org/project/pubmed-parser/) using
 
 ``` bash
 pip install pubmed-parser
 ```
```

### Comparing `pubmed_parser-0.3.1/pubmed_parser/__init__.py` & `pubmed_parser-0.4.0/pubmed_parser/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """
 Pubmed Parser: A Python Parser for PubMed Open-Access XML Subset and MEDLINE XML Dataset
 
 Author: Titipat Achakulvisut, Daniel E. Acuna
 """
-__version__ = "0.3.1"
+__version__ = "0.4.0"
 from .pubmed_oa_parser import (
     list_xml_path,
     parse_pubmed_xml,
     parse_pubmed_references,
     parse_pubmed_paragraph,
     parse_pubmed_caption,
     parse_pubmed_table,
 )
-from .medline_parser import parse_medline_xml, parse_medline_grant_id
+from .medline_parser import parse_medline_xml, split_mesh
 from .pubmed_web_parser import (
     parse_xml_web,
     parse_citation_web,
     parse_outgoing_citation_web,
 )
 from .utils import pretty_print
```

### Comparing `pubmed_parser-0.3.1/pubmed_parser/medline_parser.py` & `pubmed_parser-0.4.0/pubmed_parser/medline_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 """
 Parsers for MEDLINE XML
 """
 import re
 import numpy as np
+import gzip
 from itertools import chain
+from lxml import etree
 from collections import defaultdict
 from pubmed_parser.utils import read_xml, stringify_children, month_or_day_formater
 
-__all__ = ["parse_medline_xml", "parse_medline_grant_id"]
+__all__ = ["parse_medline_xml",  "split_mesh"]
 
 
 def parse_pmid(pubmed_article):
     """
     A function to parse PMID from a given Pubmed Article tree
 
     Parameters
@@ -75,43 +77,112 @@
                 else ""
             )
         else:
             doi = ""
     return doi
 
 
-def parse_mesh_terms(medline):
+def parse_mesh_terms(medline, parse_subs=False):
     """
     A function to parse MESH terms from article
 
     Parameters
     ----------
     medline: Element
         The lxml node pointing to a medline document
-
+    parse_subs: bool
+        If True, parse mesh subterms as well.
     Returns
     -------
     mesh_terms: str
         String of semi-colon ``;`` spearated MeSH (Medical Subject Headings)
         terms contained in the document.
     """
+    if parse_subs:
+        return parse_mesh_terms_with_subs(medline)
     if medline.find("MeshHeadingList") is not None:
         mesh = medline.find("MeshHeadingList")
         mesh_terms_list = [
             m.find("DescriptorName").attrib.get("UI", "")
             + ":"
             + m.find("DescriptorName").text
             for m in mesh.getchildren()
         ]
         mesh_terms = "; ".join(mesh_terms_list)
     else:
         mesh_terms = ""
     return mesh_terms
 
 
+def parse_mesh_terms_with_subs(medline):
+    """
+    A function to parse MESH terms and subterms from article
+
+    Parameters
+    ----------
+    medline: Element
+        The lxml node pointing to a medline document
+
+    Returns
+    -------
+    mesh_terms: str
+        String of semi-colon ``;`` spearated MeSH (Medical Subject Headings) terms contained in the document
+        and mesh subterms concatenated " / "
+        and appended with * if the subterm is a major topic.
+    """
+    if medline.find("MeshHeadingList") is not None:
+        mesh = medline.find("MeshHeadingList")
+        mesh_terms_list = []
+        for m in mesh.getchildren():
+            term = m.find("DescriptorName").attrib.get("UI", "") + ":" + \
+                   m.find("DescriptorName").text
+            if m.attrib.get("MajorTopicYN", "") == "Y":
+                term += "*"
+            for q in m.findall("QualifierName"):
+                term += " / " + q.attrib.get("UI", "") + ":" + \
+                        q.text
+                if q.attrib.get("MajorTopicYN", "") == "Y":
+                    term += "*"
+            mesh_terms_list.append(term)
+        mesh_terms = "; ".join(mesh_terms_list)
+    else:
+        mesh_terms = ""
+    return mesh_terms
+
+
+def split_mesh(mesh):
+    """String split a string from parse_mesh_terms_with_subs()
+
+    Parameters
+    ----------
+    mesh: str
+        A string returned from parse_mesh_terms_with_subs()
+
+    Returns
+    -------
+    mesh_list: List of List of 2-tuples of strings
+        A list representation of the mesh headings
+
+    Example
+    --------
+    # >>> pubmed_parser.split_mesh('D001249:Asthma / Q000188:drug therapy*; D001993:Bronchodilator Agents / Q000008:administration & dosage* / Q000009:adverse effects
+')
+    [[('D001249', 'Asthma'), ('Q000188', 'drug therapy*')],
+     [('D001993', 'Bronchodilator Agents'), ('Q000008', 'administration & dosage*'), ('Q000009', 'adverse effects')]]
+    """
+    mesh_list = []
+    for term in mesh.split("; "):
+        subs = []
+        for subterm in term.split(" / "):
+            ui, descriptor = subterm.split(":")
+            subs.append((ui, descriptor))
+        mesh_list.append(subs)
+    return mesh_list
+
+
 def parse_publication_types(medline):
     """Parse Publication types from article
 
     Parameters
     ----------
     medline: Element
         The lxml node pointing to a medline document
@@ -276,15 +347,14 @@
     grant_list: list
         List of grants acknowledged in the publications. Each
         entry in the dictionary contains the PubMed ID,
         grant ID, grant acronym, country, and agency.
     """
     medline = pubmed_article.find("MedlineCitation")
     article = medline.find("Article")
-    pmid = parse_pmid(pubmed_article)
 
     grants = article.find("GrantList")
     grant_list = list()
     if grants is not None:
         grants_list = grants.getchildren()
         for grant in grants_list:
             grant_country = grant.find("Country")
@@ -304,15 +374,14 @@
                 acronym = ""
             grant_id = grant.find("GrantID")
             if grant_id is not None:
                 gid = grant_id.text
             else:
                 gid = ""
             grant_dict = {
-                "pmid": pmid,
                 "grant_id": gid,
                 "grant_acronym": acronym,
                 "country": country,
                 "agency": agency,
             }
             grant_list.append(grant_dict)
     return grant_list
@@ -474,15 +543,15 @@
         references = ";".join(
             [ref["pmid"] for ref in references if ref["pmid"] != ""]
         )
         return references
 
 
 def parse_article_info(
-    pubmed_article, year_info_only, nlm_category, author_list, reference_list
+    pubmed_article, year_info_only, nlm_category, author_list, reference_list, parse_subs=False
 ):
     """Parse article nodes from Medline dataset
 
     Parameters
     ----------
     pubmed_article: Element
         The lxml element pointing to a medline document
@@ -490,15 +559,16 @@
         see more details in date_extractor()
     nlm_category: bool
         see more details in parse_medline_xml()
     author_list: bool
         if True, return output as list, else
     reference_list: bool
         if True, parse reference list as an output
-
+    parse_subs: bool
+        if True, parse mesh terms with subterms
     Returns
     -------
     article: dict
         Dictionary containing information about the article, including
         `title`, `abstract`, `journal`, `authors`, `affiliations`, `pubdate`,
         `pmid`, `other_id`, `mesh_terms`, `pages`, `issue`, and `keywords`. The field
         `delete` is always `False` because this function parses
@@ -513,14 +583,24 @@
         title = ""
 
     if article.find("Journal/JournalIssue/Volume") is not None:
         volume = article.find("Journal/JournalIssue/Volume").text or ""
     else:
         volume = ""
 
+    if article.find("Language") is not None:
+        languages = ";".join([language.text for language in article.findall("Language")])
+    else:
+        languages = ""
+
+    if article.find("VernacularTitle") is not None:
+        vernacular_title = stringify_children(article.find("VernacularTitle")).strip() or ""
+    else:
+        vernacular_title = ""
+
     if article.find("Journal/JournalIssue/Issue") is not None:
         issue = article.find("Journal/JournalIssue/Issue").text or ""
     else:
         issue = ""
 
     if volume == "":
         issue = ""
@@ -561,29 +641,29 @@
                 author.get("affiliation", "")
                 for author in authors_dict
                 if author.get("affiliation", "") != ""
             ]
         )
         authors = ";".join(
             [
-                author.get("lastname", "") + "|" + author.get("forename",   "") + "|" +
-                author.get("initials",  "") + "|" + author.get("identifier", "")
+                author.get("lastname", "") + "|" + author.get("forename", "") + "|" +
+                author.get("initials", "") + "|" + author.get("identifier", "")
                 for author in authors_dict
             ]
         )
     else:
         authors = authors_dict
     journal = article.find("Journal")
     journal_name = " ".join(journal.xpath("Title/text()"))
 
     pmid = parse_pmid(pubmed_article)
     doi = parse_doi(pubmed_article)
     references = parse_references(pubmed_article, reference_list)
     pubdate = date_extractor(journal, year_info_only)
-    mesh_terms = parse_mesh_terms(medline)
+    mesh_terms = parse_mesh_terms(medline, parse_subs=parse_subs)
     publication_types = parse_publication_types(medline)
     chemical_list = parse_chemical_list(medline)
     keywords = parse_keywords(medline)
     other_id_dict = parse_other_id(medline)
     journal_info_dict = parse_journal_info(medline)
     dict_out = {
         "title": title,
@@ -597,32 +677,36 @@
         "mesh_terms": mesh_terms,
         "publication_types": publication_types,
         "chemical_list": chemical_list,
         "keywords": keywords,
         "doi": doi,
         "references": references,
         "delete": False,
+        "languages": languages,
+        "vernacular_title": vernacular_title
     }
     if not author_list:
         dict_out.update({"affiliations": affiliations})
     dict_out.update(other_id_dict)
     dict_out.update(journal_info_dict)
     return dict_out
 
 
 def parse_medline_xml(
     path,
     year_info_only=True,
     nlm_category=False,
     author_list=False,
     reference_list=False,
+    parse_downto_mesh_subterms=False
 ):
     """Parse XML file from Medline XML format available at
-    ftp://ftp.nlm.nih.gov/nlmdata/.medleasebaseline/gz/
-
+    https://ftp.ncbi.nlm.nih.gov/pubmed/
+    
+    
     Parameters
     ----------
     path: str
         The path
     year_info_only: bool
         if True, this tool will only attempt to extract year information from PubDate.
         if False, an attempt will be made to harvest all available PubDate information.
@@ -633,102 +717,47 @@
         between articles.
         default: True
     nlm_category: bool
         if True, this will parse structured abstract where each section if original Label
         if False, this will parse structured abstract where each section will be assigned to
         NLM category of each sections
         default: False
-     author_list: bool
+    author_list: bool
         if True, return parsed author output as a list of authors
         if False, return parsed author output as a string of authors concatenated with ``;``
         default: False
     reference_list: bool
         if True, parse reference list as an output
         if False, return string of PMIDs concatenated with ;
         default: False
+    parse_downto_mesh_subterms: bool
+        if True, return mesh terms concatenated with "; " and mesh subterms concatenated " / "
+                and appended with * if the subterm is major
+        if False, return mesh_terms concatenated with "; "
+        default: False
 
     Return
     ------
-    article_list: list
-        A list of dictionary containing information about articles in NLM format (see
-        `parse_article_info`). Articles that have been deleted will be
+    An iterator of dictionary containing information about articles in NLM format.
+        see `parse_article_info`). Articles that have been deleted will be
         added with no information other than the field `delete` being `True`
 
     Examples
     --------
-    >>> pubmed_parser.parse_medline_xml('data/pubmed20n0014.xml.gz')
-    """
-    tree = read_xml(path)
-    medline_citations = tree.findall(".//MedlineCitationSet/MedlineCitation")
-    if len(medline_citations) == 0:
-        medline_citations = tree.findall(".//PubmedArticle")
-    article_list = list(
-        map(
-            lambda m: parse_article_info(
-                m, year_info_only, nlm_category, author_list, reference_list
-            ),
-            medline_citations,
-        )
-    )
-    delete_citations = tree.findall(".//DeleteCitation/PMID")
-    dict_delete = [
-        {
-            "title": np.nan,
-            "abstract": np.nan,
-            "journal": np.nan,
-            "authors": np.nan,
-            "affiliations": np.nan,
-            "pubdate": np.nan,
-            "pmid": p.text.strip(),
-            "doi": np.nan,
-            "other_id": np.nan,
-            "pmc": np.nan,
-            "mesh_terms": np.nan,
-            "keywords": np.nan,
-            "publication_types": np.nan,
-            "chemical_list": np.nan,
-            "delete": True,
-            "medline_ta": np.nan,
-            "nlm_unique_id": np.nan,
-            "issn_linking": np.nan,
-            "country": np.nan,
-            "references": np.nan,
-            "issue": np.nan,
-            "pages": np.nan,
-        }
-        for p in delete_citations
-    ]
-    article_list.extend(dict_delete)
-    return article_list
-
-
-def parse_medline_grant_id(path):
-    """Parse grant id from Medline XML file
-
-    Parameters
-    ----------
-    path: str
-        The path to the XML with the information
-
-    Return
-    ------
-    grant_id_list: list
-        A list of dictionaries contains the grants in a given path. Each dictionary
-        has the keys of 'pmid', 'grant_id', 'grant_acronym', 'country', and 'agency'
-
-    >>> pubmed_parser.parse_medline_grant_id('data/pubmed20n0014.xml.gz')
-    [{
-        'pmid': '399300',
-        'grant_id': 'HL17731',
-        'grant_acronym': 'HL',
-        'country': 'United States',
-        'agency': 'NHLBI NIH HHS'
-    }, ...
-    ]
-    """
-    tree = read_xml(path)
-    medline_citations = tree.findall(".//MedlineCitationSet/MedlineCitation")
-    if len(medline_citations) == 0:
-        medline_citations = tree.findall(".//PubmedArticle")
-    grant_id_list = list(map(parse_grant_id, medline_citations))
-    grant_id_list = list(chain(*grant_id_list))  # flatten list
-    return grant_id_list
+    >>> article_iterator = pubmed_parser.parse_medline_xml('data/pubmed20n0014.xml.gz')
+    >>> for article in article_iterator:
+    ...     print(article['title'])
+    """
+    with gzip.open(path, "rb") as f:
+        for event, element in etree.iterparse(f, events=("end",)):
+            if element.tag == "PubmedArticle":
+                res = parse_article_info(
+                    element,
+                    year_info_only,
+                    nlm_category,
+                    author_list,
+                    reference_list,
+                    parse_subs=parse_downto_mesh_subterms
+                )
+                res['grant_ids'] = parse_grant_id(element)
+                element.clear()
+                yield res
```

### Comparing `pubmed_parser-0.3.1/pubmed_parser/pubmed_oa_parser.py` & `pubmed_parser-0.4.0/pubmed_parser/pubmed_oa_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,18 +62,24 @@
 
 
 def parse_article_meta(tree):
     """
     Parse PMID, PMC and DOI from given article tree
     """
     article_meta = tree.find(".//article-meta")
-    pmid_node = article_meta.find('article-id[@pub-id-type="pmid"]')
-    pmc_node = article_meta.find('article-id[@pub-id-type="pmc"]')
-    pub_id_node = article_meta.find('article-id[@pub-id-type="publisher-id"]')
-    doi_node = article_meta.find('article-id[@pub-id-type="doi"]')
+    if article_meta is not None:
+        pmid_node = article_meta.find('article-id[@pub-id-type="pmid"]')
+        pmc_node = article_meta.find('article-id[@pub-id-type="pmc"]')
+        pub_id_node = article_meta.find('article-id[@pub-id-type="publisher-id"]')
+        doi_node = article_meta.find('article-id[@pub-id-type="doi"]')
+    else:
+        pmid_node = None
+        pmc_node = None
+        pub_id_node = None
+        doi_node = None
 
     pmid = pmid_node.text if pmid_node is not None else ""
     pmc = pmc_node.text if pmc_node is not None else ""
     pub_id = pub_id_node.text if pub_id_node is not None else ""
     doi = doi_node.text if doi_node is not None else ""
 
     dict_article_meta = {"pmid": pmid, "pmc": pmc, "doi": doi, "publisher_id": pub_id}
```

### Comparing `pubmed_parser-0.3.1/pubmed_parser/pubmed_web_parser.py` & `pubmed_parser-0.4.0/pubmed_parser/pubmed_web_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,24 +134,31 @@
 
     doi = ""
     article_ids = tree.xpath("//articleidlist//articleid")
     if len(article_ids) >= 1:
         for article_id in article_ids:
             if article_id.attrib.get("idtype") == "doi":
                 doi = article_id.text
+    
+    language = tree.xpath("//language")
+    try:
+        language = language[0].text
+    except IndexError:
+        language = None
 
     dict_out = {
         "title": title,
         "abstract": abstract,
         "journal": journal,
         "affiliation": affiliations_text,
         "authors": authors_text,
         "keywords": keywords,
         "doi": doi,
         "year": year,
+        "language": language
     }
     return dict_out
 
 
 def parse_xml_web(pmid, sleep=None, save_xml=False):
     """
     Give an input PMID, load and parse XML using PubMed eutils
```

### Comparing `pubmed_parser-0.3.1/pubmed_parser/utils.py` & `pubmed_parser-0.4.0/pubmed_parser/utils.py`

 * *Files identical despite different names*

### Comparing `pubmed_parser-0.3.1/setup.py` & `pubmed_parser-0.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 #! /usr/bin/env python
 from setuptools import setup
 
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
 if __name__ == "__main__":
     setup(
         name="pubmed_parser",
-        version="0.3.1",
+        version="0.4.0",
         description="A python parser for Pubmed Open-Access Subset and MEDLINE XML repository",
+        long_description=long_description,
+        long_description_content_type='text/markdown',
         url="https://github.com/titipata/pubmed_parser",
         download_url="https://github.com/titipata/pubmed_parser.git",
         author="Titipat Achakulvisut",
         author_email="my.titipat@gmail.com",
         license="MIT (c) 2015 - 2019 Titipat Achakulvisut, Daniel E. Acuna",
         install_requires=[
             "lxml",
```

