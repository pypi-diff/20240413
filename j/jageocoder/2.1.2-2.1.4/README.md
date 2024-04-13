# Comparing `tmp/jageocoder-2.1.2.tar.gz` & `tmp/jageocoder-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jageocoder-2.1.2.tar", max compression
+gzip compressed data, was "jageocoder-2.1.4.tar", max compression
```

## Comparing `jageocoder-2.1.2.tar` & `jageocoder-2.1.4.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0      113 2023-08-27 01:55:39.074598 jageocoder-2.1.2/LICENSE
--rw-r--r--   0        0        0     8253 2023-08-27 01:55:39.084598 jageocoder-2.1.2/README.md
--rw-r--r--   0        0        0     1364 2023-10-31 00:27:03.834263 jageocoder-2.1.2/jageocoder/__init__.py
--rw-r--r--   0        0        0     5605 2023-09-27 11:32:59.648181 jageocoder-2.1.2/jageocoder/__main__.py
--rw-r--r--   0        0        0     2574 2023-08-27 01:55:39.114598 jageocoder-2.1.2/jageocoder/address.py
--rw-r--r--   0        0        0     1421 2023-08-27 01:55:39.124598 jageocoder-2.1.2/jageocoder/aliases.json
--rw-r--r--   0        0        0    12147 2023-08-27 01:55:39.124598 jageocoder-2.1.2/jageocoder/aza_master.py
--rw-r--r--   0        0        0     1171 2023-08-27 01:55:39.124598 jageocoder-2.1.2/jageocoder/dataset.py
--rw-r--r--   0        0        0      691 2023-08-27 01:55:39.124598 jageocoder-2.1.2/jageocoder/exceptions.py
--rw-r--r--   0        0        0    19342 2023-10-04 11:58:20.470010 jageocoder-2.1.2/jageocoder/itaiji.py
--rw-r--r--   0        0        0    14220 2023-08-27 01:55:39.124598 jageocoder-2.1.2/jageocoder/itaiji_dic.json
--rw-r--r--   0        0        0    11718 2023-10-30 23:33:00.865378 jageocoder-2.1.2/jageocoder/module.py
--rw-r--r--   0        0        0    53107 2023-10-30 23:26:55.555507 jageocoder-2.1.2/jageocoder/node.py
--rw-r--r--   0        0        0     2631 2023-08-27 01:55:39.134598 jageocoder-2.1.2/jageocoder/result.py
--rw-r--r--   0        0        0    15475 2023-10-30 23:56:52.864900 jageocoder-2.1.2/jageocoder/rtree.py
--rw-r--r--   0        0        0     7795 2023-09-23 12:39:12.511418 jageocoder-2.1.2/jageocoder/strlib.py
--rw-r--r--   0        0        0    52507 2023-10-04 11:58:20.470010 jageocoder-2.1.2/jageocoder/tree.py
--rw-r--r--   0        0        0     4995 2023-08-27 01:55:39.134598 jageocoder-2.1.2/jageocoder/trie.py
--rw-r--r--   0        0        0     1285 2023-10-31 00:27:14.464261 jageocoder-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     9814 1970-01-01 00:00:00.000000 jageocoder-2.1.2/setup.py
--rw-r--r--   0        0        0     9793 1970-01-01 00:00:00.000000 jageocoder-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0      113 2023-08-03 02:25:59.197434 jageocoder-2.1.4/LICENSE
+-rw-r--r--   0        0        0     8253 2023-08-03 02:25:59.197434 jageocoder-2.1.4/README.md
+-rw-r--r--   0        0        0     1364 2024-04-13 05:06:33.848811 jageocoder-2.1.4/jageocoder/__init__.py
+-rw-r--r--   0        0        0     5605 2023-09-27 08:08:26.315234 jageocoder-2.1.4/jageocoder/__main__.py
+-rw-r--r--   0        0        0     2574 2023-08-03 02:25:59.209435 jageocoder-2.1.4/jageocoder/address.py
+-rw-r--r--   0        0        0     1421 2023-08-03 02:25:59.209435 jageocoder-2.1.4/jageocoder/aliases.json
+-rw-r--r--   0        0        0     8320 2024-04-10 08:33:59.049176 jageocoder-2.1.4/jageocoder/aza_master.py
+-rw-r--r--   0        0        0     1171 2023-08-03 02:25:59.209435 jageocoder-2.1.4/jageocoder/dataset.py
+-rw-r--r--   0        0        0      691 2023-08-03 02:25:59.209435 jageocoder-2.1.4/jageocoder/exceptions.py
+-rw-r--r--   0        0        0    19415 2024-01-04 06:10:34.702570 jageocoder-2.1.4/jageocoder/itaiji.py
+-rw-r--r--   0        0        0    14220 2023-08-03 02:25:59.209435 jageocoder-2.1.4/jageocoder/itaiji_dic.json
+-rw-r--r--   0        0        0    11718 2023-09-27 08:08:26.315234 jageocoder-2.1.4/jageocoder/module.py
+-rw-r--r--   0        0        0    53416 2024-04-13 04:34:54.673227 jageocoder-2.1.4/jageocoder/node.py
+-rw-r--r--   0        0        0     2631 2023-08-03 02:25:59.209435 jageocoder-2.1.4/jageocoder/result.py
+-rw-r--r--   0        0        0    15475 2023-12-08 05:15:55.172087 jageocoder-2.1.4/jageocoder/rtree.py
+-rw-r--r--   0        0        0     7795 2023-09-27 08:08:26.315234 jageocoder-2.1.4/jageocoder/strlib.py
+-rw-r--r--   0        0        0    52841 2024-04-10 07:13:06.853053 jageocoder-2.1.4/jageocoder/tree.py
+-rw-r--r--   0        0        0     4995 2023-08-03 02:25:59.213435 jageocoder-2.1.4/jageocoder/trie.py
+-rw-r--r--   0        0        0     1287 2024-04-13 05:03:29.014148 jageocoder-2.1.4/pyproject.toml
+-rw-r--r--   0        0        0     9773 1970-01-01 00:00:00.000000 jageocoder-2.1.4/PKG-INFO
```

### Comparing `jageocoder-2.1.2/README.md` & `jageocoder-2.1.4/README.md`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.2/jageocoder/__init__.py` & `jageocoder-2.1.4/jageocoder/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 running the following steps.
 
     >>> import jageocoder
     >>> jageocoder.init()
     >>> jageocoder.searchNode('<Japanese-address>')
 """
 
-__version__ = '2.1.2'  # The package version
+__version__ = '2.1.4'  # The package version
 __dictionary_version__ = '20230927'  # Compatible dictionary version
 __author__ = 'Takeshi Sagara <sagara@info-proto.com>'
 
 __all__ = [
     'init',
     'free',
     'is_initialized',
```

### Comparing `jageocoder-2.1.2/jageocoder/__main__.py` & `jageocoder-2.1.4/jageocoder/__main__.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.2/jageocoder/address.py` & `jageocoder-2.1.4/jageocoder/address.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.2/jageocoder/aliases.json` & `jageocoder-2.1.4/jageocoder/aliases.json`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.2/jageocoder/dataset.py` & `jageocoder-2.1.4/jageocoder/dataset.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.2/jageocoder/exceptions.py` & `jageocoder-2.1.4/jageocoder/exceptions.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.2/jageocoder/itaiji.py` & `jageocoder-2.1.4/jageocoder/itaiji.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,19 +118,19 @@
         for s in self.optional_strings_in_middle:
             if len(s) > 1:
                 self.first_letters_of_optional_strings_in_middle += s[0]
 
         # Patterns that cannot be omitted as AZA names
         hyphens = re.escape(strlib.hyphen)
         self.re_not_ommisible_aza_patterns = re.compile(
-            '(' +
+            r'([^。、，．0-9a-zA-Z\t\n\r\f\v]{,15}?)(' +
             rf'{numbers}[条線丁区番号{hyphens}]|' +
             rf'[{self.chiban_heads}]{numbers}|' +
             rf'{numbers}$' +
-            ')'
+            r')'
         )
 
         # Patterns that do not follow behind nodes at that level
         self.re_non_trailing_patterns = {
             AddressLevel.BLOCK: re.compile(r'[0-9A-Za-z甲乙丙丁]+\.?(番|番地|号|地)'),
             AddressLevel.BLD: re.compile(r'[0-9]+\.?(号|番地)'),
         }
@@ -471,19 +471,20 @@
             Position to start analysis
 
         Returns
         -------
         int
             Number of characters that can be omitted.
         """
-        m = self.re_not_ommisible_aza_patterns.search(string[pos:])
+        m = self.re_not_ommisible_aza_patterns.match(string[pos:])
         if m is None:
             return 0
 
-        n = string[pos:].find(m.group(0))
+        n = len(m.group(1))
+        # n = string[pos:].find(m.group(0))
         return n
 
         candidates = []
         i = 0
         while i <= self.max_skip_azaname:
             if pos + i >= len(string):
                 break
```

### Comparing `jageocoder-2.1.2/jageocoder/itaiji_dic.json` & `jageocoder-2.1.4/jageocoder/itaiji_dic.json`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.2/jageocoder/module.py` & `jageocoder-2.1.4/jageocoder/module.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.2/jageocoder/node.py` & `jageocoder-2.1.4/jageocoder/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -503,20 +503,20 @@
                 ).format(
                     self.name, self.id, child.name, child.id))
                 break
 
         return new_node
 
     def search_child_with_criteria(
-            self,
-            pattern: str,
-            min_candidate: Optional[str] = None,
-            gt_candidate: Optional[str] = None,
-            max_level: Optional[int] = None,
-            require_coordinates: bool = False) -> List[AddressNode]:
+        self,
+        pattern: str,
+        min_candidate: Optional[str] = None,
+        gt_candidate: Optional[str] = None,
+        max_level: Optional[int] = None,
+    ) -> List[AddressNode]:
         """
         Search for children nodes that satisfy the specified conditions.
 
         Parameters
         ----------
         pattern: str
             The regular expression that the child node's name must match.
@@ -524,33 +524,29 @@
             The smallest string that satisfies the condition
             as the name of a child node.
         gt_candidate: str, optional
             The smallest string that exceeds the upper limit
             that satisfies the condition as the name of a child node.
         max_level: int, optional
             Maximum level of child nodes; unlimited if None.
-        require_coordinates: bool [False]
-            If set to True, the child node must have valid coordinates.
 
         Returns
         -------
         List[AddressNode]
             A list of all child nodes that satisfy the specified condition.
         """
         logger.debug((
-            "Called with self:'{}'({}), pattern:{}, min:'{}', gt:'{}', "
-            "max_level: {}, require_coordinates: {}."
+            "Called with self:'{}'({}), pattern:{}, min:'{}', gt:'{}', max_level: {}."
         ).format(
             self.name,
             self.id,
             pattern,
             min_candidate,
             gt_candidate,
             max_level,
-            require_coordinates
         ))
         re_pattern = re.compile(pattern)
         address_node = self.table.get_record(pos=self.id)
         children = []
 
         if self.sibling_id == self.id + 1:  # No child
             logger.debug(
@@ -594,20 +590,18 @@
 
             if gt_candidate is not None and \
                     candidate.name_index >= gt_candidate:
                 break
 
             if re_pattern.match(candidate.name_index) and \
                     (max_level is None or candidate.level <= max_level):
-                if require_coordinates is False or candidate.y <= 90.0:
-                    children.append(candidate)
-                else:
+                if candidate.y > 90.0:
                     candidate = candidate.add_dummy_coordinates()
-                    if candidate.y <= 90.0:
-                        children.append(candidate)
+
+                children.append(candidate)
 
             next_pos = candidate.sibling_id
 
         logger.debug("Returns {} children.".format(len(children)))
         return children
 
     def search_recursive(
@@ -682,15 +676,15 @@
             max_level = AddressLevel.AZA
 
         filtered_children = self.search_child_with_criteria(
             pattern=substr,
             min_candidate=min_candidate,
             gt_candidate=gt_candidate,
             max_level=max_level,
-            require_coordinates=tree.get_config('require_coordinates'))
+        )
 
         # Check if the index begins with an extra character of
         # the current node.
         if len(filtered_children) == 0 and \
                 index[0] in tree.converter.extra_characters:
             logger.debug((
                 "Remove the leading extra character '{}' and "
@@ -698,20 +692,25 @@
             candidates = self.search_recursive(
                 tree=tree,
                 index=index[1:],
                 processed_nodes=processed_nodes)
             if len(candidates) > 0:
                 new_candidates = []
                 for candidate in candidates:
+                    if candidate.node.id == self.id:
+                        new_candidates.append(candidate)
+                        continue
+
                     new_candidate = Result(
                         candidate.node,
                         index[0] + candidate.matched,
                         l_optional_prefix + candidate.nchars)
                     new_candidates.append(new_candidate)
 
+                new_candidates.append(Result(self, "", 0))
                 return new_candidates
 
             return []
 
         if logger.isEnabledFor(logging.DEBUG):
             if len(filtered_children) == 0:
                 msg = "No matched children. (#children:{})".format(
@@ -734,14 +733,15 @@
                 tree=tree,
                 index=index,
                 optional_prefix=optional_prefix,
                 processed_nodes=processed_nodes)
 
             if len(new_candidates) > 0:
                 candidates += new_candidates
+                candidates.append(Result(self, "", 0))
 
         # Processes the region's own rules.
         parent_node = self.get_parent()
         if self.level == AddressLevel.WARD and parent_node.name == '京都市':
             # Street name (通り名) support in Kyoto City
             # If a matching part of the search string is found in the
             # child nodes, the part before the name is skipped
@@ -753,31 +753,35 @@
 
                 offset = pos + len(child.name_index)
                 rest_index = index[offset:]
                 logger.debug(
                     "child:{} match {} chars".format(child, offset))
                 processed_nodes.add(child.id)
                 logger.debug(f"{child.name}({child.id}) marked as processed")
-                for cand in child.search_recursive(
-                        tree=tree,
-                        index=rest_index,
-                        processed_nodes=processed_nodes):
+                new_candidates = child.search_recursive(
+                    tree=tree,
+                    index=rest_index,
+                    processed_nodes=processed_nodes)
+                for cand in new_candidates:
                     candidates.append(Result(
                         cand[0],
                         optional_prefix +
                         index[0: offset] + cand[1],
                         l_optional_prefix +
                         len(child.name_index) + len(cand[1])))
 
-        if len(candidates) == 0:
-            candidates += self.check_redirect(
-                tree, index, processed_nodes
-            )
+                if len(new_candidates) > 0:
+                    candidates.append(Result(self, "", 0))
+
+        # Search for nodes with possible address changes.
+        candidates += self.check_redirect(
+            tree, index, processed_nodes
+        )
 
-        # Search for subnodes with queries excludes Aza-name candidates
+        # Search for subnodes with queries excludes Aza-name candidates.
         omissible_index = None
         aza_skip = tree.get_config('aza_skip')
         if len(candidates) == 0 or \
                 len(index) - len(candidates[0].matched) > 2:
             logger.debug((
                 "Try to skip over the omissible Aza-names and "
                 "search for matching nodes since no candidates found."
@@ -814,27 +818,32 @@
                 tree.set_config(aza_skip=False)
                 sub_candidates = self.search_recursive(
                     tree=tree,
                     index=index[azalen:],
                     processed_nodes=processed_nodes)
                 tree.set_config(aza_skip=aza_skip)
                 if sub_candidates[0].matched != '':
+                    added = 0
                     for cand in sub_candidates:
                         if cand.node.level < AddressLevel.BLOCK and \
                                 cand.node.name_index not in \
                                 tree.converter.chiban_heads:
                             logger.debug("{} is ignored".format(
                                 cand.node.name))
                             continue
 
                         candidates.append(Result(
                             cand.node,
                             optional_prefix +
                             index[0:azalen] + cand.matched,
                             l_optional_prefix + cand.nchars))
+                        added += 1
+
+                    if added > 0:
+                        candidates.append(Result(self, "", 0))
 
         if False and len(candidates) == 0:
             # Search common names
             for k, v in self.get_notes():
                 if k != "cn":
                     continue
 
@@ -875,14 +884,15 @@
     def check_redirect(
         self,
         tree: AddressTree,
         index: str,
         processed_nodes: Set[int]
     ) -> List[Result]:
         auto_redirect = tree.get_config('auto_redirect')
+        require_coordinates = tree.get_config('require_coordinates')
         if auto_redirect is False:
             return []
 
         candidates = []
         # Search redirect nodes
         for k, v in self.get_notes():
             if k != "ref":
@@ -891,17 +901,20 @@
             for ref in v.split('|'):
                 logger.debug(
                     f"Redirect '{self.get_fullname()}' to '{ref}'"
                 )
                 processed_nodes.add(self.id)
                 logger.debug(
                     f"{self.name}({self.id}) marked as processed")
-                tree.set_config(auto_redirect=False)
+                tree.set_config(auto_redirect=False, require_coordinates=False)
                 redirect_results = tree.search_by_trie(ref)
-                tree.set_config(auto_redirect=auto_redirect)
+                tree.set_config(
+                    auto_redirect=auto_redirect,
+                    require_coordinates=require_coordinates
+                )
                 for node_id, val in redirect_results.items():
                     if node_id in processed_nodes:
                         continue
 
                     node: AddressNode = val[0]
                     for result in node.search_recursive(
                             tree, index, processed_nodes):
@@ -1083,14 +1096,15 @@
                         logger.debug(
                             "Can't omit substring '{}' from '{}' in {}".format(
                                 name, names[-1][1], omissible_index))
                         omissible_index = omissible_index[0:pos]
 
                         if pos == 0:
                             break
+
         else:  # strict mode
             # Consider omittable only those portions that can be omitted
             # with by Aza-master.
             omissible_index = ""
             for aza_record in aza_records:
                 if aza_record.startCountType == 1:
                     names = json.loads(aza_record.names)
```

### Comparing `jageocoder-2.1.2/jageocoder/result.py` & `jageocoder-2.1.4/jageocoder/result.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.2/jageocoder/rtree.py` & `jageocoder-2.1.4/jageocoder/rtree.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.2/jageocoder/strlib.py` & `jageocoder-2.1.4/jageocoder/strlib.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.2/jageocoder/tree.py` & `jageocoder-2.1.4/jageocoder/tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1219,18 +1219,18 @@
             key = index[0:offset]
             rest_index = index[offset:]
             for node_id in trie_node.nodes:
                 node = self.get_address_node(id=node_id)
 
                 if node.y > 90.0 and self.get_config('require_coordinates'):
                     node = node.add_dummy_coordinates()
-                    if node.y > 90.0:
-                        logger.debug("Node {}({}) has no coordinates.".format(
-                            node.name, node.id))
-                        continue
+                    # if node.y > 90.0:
+                    #     logger.debug("Node {}({}) has no coordinates.".format(
+                    #         node.name, node.id))
+                    #     continue
 
                 if min_key == '' and node.level <= AddressLevel.WARD:
                     # To make the process quicker, once a node higher
                     # than the city level is found, addresses shorter
                     # than the node are not searched after this.
                     logger.debug((
                         "A node with ward or higher levels found. "
@@ -1311,17 +1311,24 @@
                         for area in target_area:
                             inside = cand.node.is_inside(area)
                             if inside == 1:
                                 break
 
                         if inside != 1:
                             msg = "Node {}({}) is not in the target area."
-                            logger.debug(msg.format(node.name, node.id))
+                            logger.debug(msg.format(
+                                cand.node.name, cand.node.id))
                             continue
 
+                    if self.get_config("require_coordinates") and cand.node.y > 90.0:
+                        logger.debug("Node {}({}) has no coordinates.".format(
+                            cand.node.name, cand.node.id
+                        ))
+                        continue
+
                     _len = offset + cand.nchars
                     _part = offset + len(cand.matched)
                     msg = "candidate: {} ({})"
                     logger.debug(msg.format(key + cand.matched, _len))
                     if best_only:
                         if _len > max_len:
                             results = {
```

### Comparing `jageocoder-2.1.2/jageocoder/trie.py` & `jageocoder-2.1.4/jageocoder/trie.py`

 * *Files identical despite different names*

### Comparing `jageocoder-2.1.2/pyproject.toml` & `jageocoder-2.1.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "jageocoder"
-version = "2.1.2"
+version = "2.1.4"
 description = "A Japanese-address geocoder for Python."
 authors = ["Takeshi Sagara <sagara@info-proto.com>"]
 repository = "https://github.com/t-sagara/jageocoder/"
 license = "The MIT License"
 readme = "README.md"
 documentation = "https://jageocoder.readthedocs.io/"
 packages = [
@@ -17,35 +17,38 @@
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
 ]
 include = ["itaiji_dic.json", "islands.json"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
-marisa-trie = "^0.7.8"
-jaconv = "^0.3.4"
-docopt = "^0.6.2"
+certifi = ">=2023.7.22"
+cryptography = ">=42.0.4"
 deprecated = "^1.2.13"
-Werkzeug = ">=2.2.3"
-pycapnp = "^1.3.0"
+docopt = "^0.6.2"
+geographiclib = "^2.0"
+idna = ">=3.7"
+jaconv = "^0.3.4"
+marisa-trie = "^0.7.8"
+pycapnp = "*"
 portabletab = ">=0.3.3"
-tqdm = "^4.00.0"
 rtree = "^1.0.0"
-geographiclib = "^2.0"
-certifi = ">=2023.7.22"
-cryptography = ">=41.0.4"
+tqdm = "^4.00.0"
 urllib3 = ">=2.0.6"
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.2.1"
-flask = "^2.2.5"
-flask-cors = "^3.0.10"
-sphinx = ">=5.0.0,<6.0.0"
-sphinx-rtd-theme = "^1.2.0"
 twine = "^4.0.2"
 
+
+[tool.poetry.group.doc.dependencies]
+sphinx-rtd-theme = "^1.2.0"
+
+
+[tool.poetry.group.test.dependencies]
+pytest = "^7.2.1"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 jageocoder = "jageocoder.__main__:main"
```

### Comparing `jageocoder-2.1.2/PKG-INFO` & `jageocoder-2.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jageocoder
-Version: 2.1.2
+Version: 2.1.4
 Summary: A Japanese-address geocoder for Python.
 Home-page: https://github.com/t-sagara/jageocoder/
 License: The MIT License
 Author: Takeshi Sagara
 Author-email: sagara@info-proto.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -14,25 +14,25 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
-Requires-Dist: Werkzeug (>=2.2.3)
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: certifi (>=2023.7.22)
-Requires-Dist: cryptography (>=41.0.4)
+Requires-Dist: cryptography (>=42.0.4)
 Requires-Dist: deprecated (>=1.2.13,<2.0.0)
 Requires-Dist: docopt (>=0.6.2,<0.7.0)
 Requires-Dist: geographiclib (>=2.0,<3.0)
+Requires-Dist: idna (>=3.7)
 Requires-Dist: jaconv (>=0.3.4,<0.4.0)
 Requires-Dist: marisa-trie (>=0.7.8,<0.8.0)
 Requires-Dist: portabletab (>=0.3.3)
-Requires-Dist: pycapnp (>=1.3.0,<2.0.0)
+Requires-Dist: pycapnp
 Requires-Dist: rtree (>=1.0.0,<2.0.0)
 Requires-Dist: tqdm (>=4.00.0,<5.0.0)
 Requires-Dist: urllib3 (>=2.0.6)
 Project-URL: Documentation, https://jageocoder.readthedocs.io/
 Project-URL: Repository, https://github.com/t-sagara/jageocoder/
 Description-Content-Type: text/markdown
```

