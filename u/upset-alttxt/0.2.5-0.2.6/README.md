# Comparing `tmp/upset-alttxt-0.2.5.tar.gz` & `tmp/upset-alttxt-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upset-alttxt-0.2.5.tar", last modified: Mon Mar 25 16:45:57 2024, max compression
+gzip compressed data, was "upset-alttxt-0.2.6.tar", last modified: Fri Apr 12 22:27:55 2024, max compression
```

## Comparing `upset-alttxt-0.2.5.tar` & `upset-alttxt-0.2.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:45:57.497267 upset-alttxt-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-03-25 16:45:50.000000 upset-alttxt-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-03-25 16:45:57.497267 upset-alttxt-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-03-25 16:45:50.000000 upset-alttxt-0.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      648 2024-03-25 16:45:50.000000 upset-alttxt-0.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-03-25 16:45:57.497267 upset-alttxt-0.2.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-25 16:45:50.000000 upset-alttxt-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:45:57.493267 upset-alttxt-0.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:45:57.493267 upset-alttxt-0.2.5/src/alttxt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 16:45:50.000000 upset-alttxt-0.2.5/src/alttxt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-03-25 16:45:50.000000 upset-alttxt-0.2.5/src/alttxt/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-03-25 16:45:50.000000 upset-alttxt-0.2.5/src/alttxt/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-03-25 16:45:50.000000 upset-alttxt-0.2.5/src/alttxt/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-25 16:45:50.000000 upset-alttxt-0.2.5/src/alttxt/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12302 2024-03-25 16:45:50.000000 upset-alttxt-0.2.5/src/alttxt/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     6901 2024-03-25 16:45:50.000000 upset-alttxt-0.2.5/src/alttxt/phrases.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-03-25 16:45:50.000000 upset-alttxt-0.2.5/src/alttxt/regionclass.py
--rw-r--r--   0 runner    (1001) docker     (127)    40310 2024-03-25 16:45:50.000000 upset-alttxt-0.2.5/src/alttxt/tokenmap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:45:57.497267 upset-alttxt-0.2.5/src/upset_alttxt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-03-25 16:45:57.000000 upset-alttxt-0.2.5/src/upset_alttxt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-03-25 16:45:57.000000 upset-alttxt-0.2.5/src/upset_alttxt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 16:45:57.000000 upset-alttxt-0.2.5/src/upset_alttxt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 16:45:57.000000 upset-alttxt-0.2.5/src/upset_alttxt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-25 16:45:57.000000 upset-alttxt-0.2.5/src/upset_alttxt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-25 16:45:57.000000 upset-alttxt-0.2.5/src/upset_alttxt.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 16:45:57.497267 upset-alttxt-0.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-03-25 16:45:50.000000 upset-alttxt-0.2.5/tests/test_alttxt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:27:55.219862 upset-alttxt-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-12 22:27:55.219862 upset-alttxt-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      648 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-12 22:27:55.219862 upset-alttxt-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:27:55.215862 upset-alttxt-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:27:55.215862 upset-alttxt-0.2.6/src/alttxt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2407 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6689 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13128 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6945 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/phrases.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/regionclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43919 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/src/alttxt/tokenmap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:27:55.219862 upset-alttxt-0.2.6/src/upset_alttxt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-12 22:27:55.000000 upset-alttxt-0.2.6/src/upset_alttxt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-12 22:27:55.000000 upset-alttxt-0.2.6/src/upset_alttxt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:27:55.000000 upset-alttxt-0.2.6/src/upset_alttxt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 22:27:54.000000 upset-alttxt-0.2.6/src/upset_alttxt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-12 22:27:55.000000 upset-alttxt-0.2.6/src/upset_alttxt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-12 22:27:55.000000 upset-alttxt-0.2.6/src/upset_alttxt.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 22:27:55.219862 upset-alttxt-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-12 22:27:51.000000 upset-alttxt-0.2.6/tests/test_alttxt.py
```

### Comparing `upset-alttxt-0.2.5/LICENSE` & `upset-alttxt-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.5/PKG-INFO` & `upset-alttxt-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upset-alttxt
-Version: 0.2.5
+Version: 0.2.6
 Summary: Generates alt text for UpSet plots
 Author: Visualization Design Lab
 License: BSD3
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `upset-alttxt-0.2.5/README.md` & `upset-alttxt-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.5/pyproject.toml` & `upset-alttxt-0.2.6/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -20,11 +20,11 @@
 warn_return_any = true
 warn_unreachable = false
 warn_unused_configs = true
 no_implicit_reexport = true
 
 [project]
 name = "upset-alttxt"
-version = "0.2.5"
+version = "0.2.6"
 description = "Generates alt text for UpSet plots"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `upset-alttxt-0.2.5/setup.cfg` & `upset-alttxt-0.2.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.5/src/alttxt/__main__.py` & `upset-alttxt-0.2.6/src/alttxt/__main__.py`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.5/src/alttxt/enums.py` & `upset-alttxt-0.2.6/src/alttxt/enums.py`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.5/src/alttxt/generator.py` & `upset-alttxt-0.2.6/src/alttxt/generator.py`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.5/src/alttxt/models.py` & `upset-alttxt-0.2.6/src/alttxt/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     """
 
     name: str
     size: int # size
     dev: float # Deviation
     degree: int # Set to -1 if parser fails to find degree
     classification: IntersectionType
+    setMembership: set
 
 class DataModel(BaseModel):
     """
     For holding data from the "rawData" and "processedData" fields
     of the JSON data file.
     """
```

### Comparing `upset-alttxt-0.2.5/src/alttxt/parser.py` & `upset-alttxt-0.2.6/src/alttxt/parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -151,15 +151,22 @@
             size: int = int(item.get("size", self.default_field))
             # Deviation - rounded to 2 decimals
             dev: float = round(item.get("deviation", self.default_field), 2)
             # Degree
             degree: int = int(item.get("degree", self.default_field))
             # Classification
             classification = self.classify_subset(degree, len(data["visibleSets"]))
-            subsets.append(Subset(name=name, size=size, dev=dev, degree=degree, classification=classification))
+
+               # Process setMembership to store only the names of sets with "Yes" membership
+            setMembership = {key[4:] if key.startswith("Set_") else key: value for key, value in item.get("setMembership", {}).items() if value == "Yes"}
+        
+            # Only store the keys (set names) that have "Yes" as their value
+            yes_sets = {key for key, value in setMembership.items() if value == "Yes"}
+
+            subsets.append(Subset(name=name, size=size, dev=dev, degree=degree, classification=classification, setMembership=yes_sets))
         
         lowercase_data_visible_subsets = {k.lower(): k for k in data_visible_subsets.keys()}
 
         all_subsets: list[Subset] = []
         data_all_subsets = data["processedData"]["values"]
         count: list[int] = []
         for key, item in data_all_subsets.items():
@@ -186,17 +193,22 @@
                 degree = int(degree)
             else:
                 degree = 0  # or some default value
 
             all_sets_length = len(data["allSets"])
 
             classification = self.classify_subset(degree, all_sets_length)
+
+            setMembership = {key[4:] if key.startswith("Set_") else key: value for key, value in item.get("setMembership", {}).items() if value == "Yes"}
+        
+            # Only store the keys (set names) that have "Yes" as their value
+            yes_sets = {key for key, value in setMembership.items() if value == "Yes"}
             
             count.append(size)
-            all_subsets.append(Subset(name=name, size=size, dev=dev, degree=degree, classification=classification))
+            all_subsets.append(Subset(name=name, size=size, dev=dev, degree=degree, classification=classification, setMembership=yes_sets))
 
         # List of set names
         sets_: list[str] = []
         for set_ in data["allSets"]:
             set_name: str = set_["name"]
             sizes[set_name] = set_["size"]
 
@@ -244,19 +256,19 @@
         )
 
         plots = PlotModel(
             scatterplots=grammar["plots"]["scatterplots"],
             histograms=grammar["plots"]["histograms"],
         )
 
-        if "metaData" in grammar:
+        if "plotInformation" in grammar:
             metaData = MetaDataModel(
-                description=grammar["metaData"]["description"],
-                sets=grammar["metaData"]["sets"],
-                items=grammar["metaData"]["items"],
+                description=grammar["plotInformation"]["description"],
+                sets=grammar["plotInformation"]["sets"],
+                items=grammar["plotInformation"]["items"],
             )
         else:
             metaData = MetaDataModel(
                 description="",
                 sets="",
                 items="",
             )
```

### Comparing `upset-alttxt-0.2.5/src/alttxt/phrases.py` & `upset-alttxt-0.2.6/src/alttxt/phrases.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,16 +33,20 @@
         "statistical_information": "[[size_percs]]. [[maxmin_set_percentages_info]].",
     },
     "level_3": {
         "trend_analysis": "[[intersection_trend_change]][[factor_analysis]][[categorization_of_subsets]]",
 
     },
     # L3 note: observe which sets are not present in many large intersections
-    "AltText": "This is an UpSet plot which shows set intersection of {{visible_set_count}} sets out of {{set_count}} sets"
-    " and the largest intersection is {{max_intersection_name}} ({{max_intersection_size}}). The plot is sorted by {{sort_type}} and {{visible_non_empty_intersect_count}} non-empty intersections are shown.",
+    "AltText": "This is an UpSet plot which shows the intersections of {{visible_set_count}} sets."
+    " All major intersections involve the set {{highest_dominant_set}}."
+    " The largest intersection is {{max_intersection_name}}, with {{max_intersection_size}} {{set_description}}."
+    " Other large intersections also involve {{large_sets}}."
+    " {{all_set_index}}",
+
     # These are all of the non-terminal symbols that are used in the grammar
     "symbols": {
         # "This is an UpSet plot"
         "UpSet": "This is an UpSet plot that visualizes set intersection",
         # Another title for an UpSet plot
         "InUpSet": "in this UpSet plot",
         # Learn more about UpSet plots
```

### Comparing `upset-alttxt-0.2.5/src/alttxt/regionclass.py` & `upset-alttxt-0.2.6/src/alttxt/regionclass.py`

 * *Files identical despite different names*

### Comparing `upset-alttxt-0.2.5/src/alttxt/tokenmap.py` & `upset-alttxt-0.2.6/src/alttxt/tokenmap.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,20 +43,20 @@
         # Since functions are only executed on run, they can be used to
         # optimize by moving expensive tokens into fuctions.
         self.map: dict[str, Union[str, float, int, Callable[[], str]]] = {
             # Title of the plot as a phrase (with verb), with null check
             "title": f"is titled: {self.title}" if self.title else "has no title",
             # Dataset description as attribute name
             "dataset_description": (
-                f"The dataset shows attributes of {self.grammar.metaData.description}. "
+                f"The dataset shows attributes of {self.grammar.metaData.description.lower()}. "
                 if self.grammar.metaData.description
                 else ""
             ),
             # Set description as set name
-            "set_description": f"{self.grammar.metaData.items}" if self.grammar.metaData.items else "elements",
+            "set_description": f"{self.grammar.metaData.items.lower()}" if self.grammar.metaData.items else "elements",
             # largest by what factor
             "largest_factor": f" {self.sort_subsets_by_key(SubsetField.SIZE, True)[0].name} is the largest by a factor of {self.calculate_largest_factor()}." if self.calculate_largest_factor() >= 2 else "",
             # set intersection categorization text based on intersection type and size
             "empty_set_presence": f" The empty intersection is present with a size of {self.get_empty_intersection_size()}." if (self.categorize_subsets().get('the empty intersection') and self.categorize_subsets().get('the empty intersection')!='largest_data_region') else "",
             "all_set_presence": f" An all set intersection is present with a size of {self.get_all_set_intersection_size()}." if self.get_all_set_intersection_size()!= None else f" An all set intersection is not present.",
             "intersection_trend_analysis":f"{self.calculate_intersection_trend()}" if self.grammar.sort_by == SortBy.SIZE else "",
             "individual_set_presence": f"{self.individual_set_presence()}",
@@ -169,15 +169,18 @@
             "avg_neg_dev": self.dev_info()["neg_avg"],
             # Sizes of visible sets, listed
             "list_set_sizes": self.set_sizes,
             # 10 largest deviations, listed
             "list10_dev_outliers": self.dev_outliers(10) if len(self.data.subsets)>=10 else self.dev_outliers(len(self.data.subsets)),
             # 5 largest deviations, listed
             "list5_dev_outliers": self.dev_outliers(5) if len(self.data.subsets)>=5 else self.dev_outliers(len(self.data.subsets)),
-            "category_of_subsets": self.categorize_subsets
+            "category_of_subsets": self.categorize_subsets,
+            "highest_dominant_set": self.find_dominant_sets(),
+            "large_sets": self.find_sets_in_large_subsets(),
+            "all_set_index": self.get_all_set_position(),
         }
 
     ###############################
     #       Public methods        #
     ###############################
 
     def get_token(self, token: str) -> str:
@@ -733,20 +736,16 @@
             # Initialize dictionary to store sizes for special classifications
             special_sizes = {}
             # Initialize Counter for other classifications
             classification_sizes = Counter()
 
             for subset in subsets:
                 # Handle 'the empty set' and 'all set' by directly logging their sizes
-                # if subset.classification in ['the empty set', 'all set']:
-                #     special_sizes[subset.classification] = subset.size
                 if subset.classification in ['the empty set']:
                     special_sizes[subset.classification] = subset.size
-                # elif subset.degree == self.data.all_sets_length:
-                #     special_sizes[IntersectionType.ALL_SET] = subset.size
                 else:
                     classification_sizes[subset.classification] += subset.size
 
                     
 
             # Calculate percentages based on sizes for other classifications
             percentages = {cls: (size / total_sizes[region_name] * 100) for cls, size in classification_sizes.items()}
@@ -785,27 +784,25 @@
                     # Include all regions that meet the threshold
                     classification_to_regions[classification] = set(above_threshold_regions.keys())
             else:
                 # If the classification is present in only one region, include it regardless of the percentage
                 classification_to_regions[classification] = set(regions_percentages.keys())
 
         # Handle special cases such as 'the empty set' and 'all set'
-        # Assuming they should be directly mapped without considering the threshold
+        # They should be directly mapped without considering the threshold
         for special_case in ['the empty set', 'all set']:
             if special_case in results:
                 for region in results[special_case]:
                     classification_to_regions[special_case] = {region}
 
 
         final_output = {cls: {regions} if isinstance(regions, str) else set(regions) for cls, regions in classification_to_regions.items()}
         
         return final_output
 
-    
-
     def get_empty_intersection_size(self):
     # Iterate through subsets to find 'the empty intersection'
         for subset in self.data.subsets:
             if subset.classification.value == 'the empty intersection':
                 return subset.size
         # Return 0 or None if 'the empty intersection' is not found
         return None
@@ -890,8 +887,91 @@
         if self.grammar.sort_order == SortOrder.DESCENDING:
             return f" The intersection sizes peak at a value of {max_int_size} and then {intersection_trend} flatten down to {min_int_size}."
             
         else:
             return f" The intersection sizes start from a value of {min_int_size} and then {intersection_trend} rise up to {max_int_size}."
         
     
+    def find_dominant_sets(self):
+        # Initialize a counter for all visible sets
+        set_occurrences = Counter()
+
+        # Go through each subset and count the occurrences of each visible set in subset names
+        for subset in self.data.subsets:
+            for set_name in self.grammar.visible_sets:
+                if set_name in subset.name:
+                    set_occurrences[set_name] += 1
+        # Find the most common sets, which returns a list of tuples (set_name, occurrences)
+        most_common_sets = set_occurrences.most_common(2)
+
+        # Extract only the names of the most and second most dominant sets
+        most_dominant_set = most_common_sets[0][0]
+        second_most_dominant_set = most_common_sets[1][0] if len(most_common_sets) > 1 else None
+
+        return f"{most_dominant_set}, and {second_most_dominant_set}"
+
+    def find_sets_in_large_subsets(self):
+        # Sort subsets by size in descending order
+        sorted_subsets = sorted(self.data.subsets, key=lambda subset: subset.size, reverse=True)
+        
+        # Extract set names from the 2nd largest subset
+        second_largest_sets = sorted_subsets[1].setMembership
+        sets = []
+
+        if len(second_largest_sets) == 1:
+            # Extract set names from the 3rd largest subset
+            third_largest_sets = sorted_subsets[2].setMembership
+            # Find the intersection of sets between the 2nd and 3rd largest subsets
+            common_sets = second_largest_sets.union(third_largest_sets)
+
+            for cs in common_sets:
+                sets.append(cs)
+        
+        else:
+            for sm in second_largest_sets:
+                sets.append(sm)
+    
+         # Formatting the return value based on the size of the sets list
+        if len(sets) == 2:
+            return f"{sets[0]} and {sets[1]}"
+        elif len(sets) > 2:
+            return ', '.join(sets[:-1]) + ', and ' + sets[-1]
+        else:
+            return sets
+    
+
+    def get_all_set_position(self):
+    # Sort subsets by size in descending order
+        sorted_subsets = sorted(self.data.subsets, key=lambda subset: subset.size, reverse=True)
+
+        # Find the "all set" intersection if it exists
+        all_set_index = None
+        for index, subset in enumerate(sorted_subsets):
+            if subset.degree == len(self.grammar.visible_sets): # all_sets_length is equal to the number of visible sets
+                all_set_size =  subset.size
+                all_set_index = index
+                break
+
+        if all_set_index is not None:
+            # Determine the position of the "all set" intersection
+            total_subsets = len(sorted_subsets)
+            if all_set_index == 0:
+                return f"The intersection of all sets is the largest with {all_set_size} elements."
+            elif all_set_index == 1:
+                return f"The intersection of all sets is the second largest with {all_set_size} elements."
+            elif all_set_index == 2:
+                return f"The intersection of all sets is the third largest with {all_set_size} elements."
+            elif all_set_index == total_subsets - 1:
+                return f"The intersection of all sets is the smallest with {all_set_size} elements."
+            elif all_set_index == total_subsets - 2:
+                return f"The intersection of all sets is the second smallest with {all_set_size} elements."
+            elif all_set_index == total_subsets - 3:
+                return f"The intersection of all sets is the third smallest with {all_set_size} elements."
+            else:
+                return f"The intersection of all sets is present with {all_set_size} elements."
+        else:
+            return ""
+
+
+
+
```

### Comparing `upset-alttxt-0.2.5/src/upset_alttxt.egg-info/PKG-INFO` & `upset-alttxt-0.2.6/src/upset_alttxt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: upset-alttxt
-Version: 0.2.5
+Version: 0.2.6
 Summary: Generates alt text for UpSet plots
 Author: Visualization Design Lab
 License: BSD3
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `upset-alttxt-0.2.5/src/upset_alttxt.egg-info/SOURCES.txt` & `upset-alttxt-0.2.6/src/upset_alttxt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

