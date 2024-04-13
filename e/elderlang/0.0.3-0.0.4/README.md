# Comparing `tmp/elderlang-0.0.3.tar.gz` & `tmp/elderlang-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elderlang-0.0.3.tar", last modified: Wed Mar 13 05:24:29 2024, max compression
+gzip compressed data, was "elderlang-0.0.4.tar", last modified: Sat Apr 13 06:59:41 2024, max compression
```

## Comparing `elderlang-0.0.3.tar` & `elderlang-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2024-03-13 05:24:29.897786 elderlang-0.0.3/
--rw-r--r--   0 eons      (1000) eons      (1000)      560 2024-03-13 05:24:29.897786 elderlang-0.0.3/PKG-INFO
--rw-rw-r--   0 eons      (1000) eons      (1000)       20 2024-03-13 05:23:59.000000 elderlang-0.0.3/README.md
-drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2024-03-13 05:24:29.853785 elderlang-0.0.3/pkg/
-drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2024-03-13 05:24:29.869785 elderlang-0.0.3/pkg/elderlang/
--rw-rw-r--   0 eons      (1000) eons      (1000)       80 2024-03-13 05:24:05.000000 elderlang-0.0.3/pkg/elderlang/__init__.py
--rw-rw-r--   0 eons      (1000) eons      (1000)       67 2024-03-13 05:24:05.000000 elderlang-0.0.3/pkg/elderlang/__main__.py
--rw-rw-r--   0 eons      (1000) eons      (1000)   236957 2024-03-13 05:24:05.000000 elderlang-0.0.3/pkg/elderlang/elderlang.py
-drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2024-03-13 05:24:29.893785 elderlang-0.0.3/pkg/elderlang.egg-info/
--rw-r--r--   0 eons      (1000) eons      (1000)      560 2024-03-13 05:24:29.000000 elderlang-0.0.3/pkg/elderlang.egg-info/PKG-INFO
--rw-rw-r--   0 eons      (1000) eons      (1000)      337 2024-03-13 05:24:29.000000 elderlang-0.0.3/pkg/elderlang.egg-info/SOURCES.txt
--rw-rw-r--   0 eons      (1000) eons      (1000)        1 2024-03-13 05:24:29.000000 elderlang-0.0.3/pkg/elderlang.egg-info/dependency_links.txt
--rw-rw-r--   0 eons      (1000) eons      (1000)       46 2024-03-13 05:24:29.000000 elderlang-0.0.3/pkg/elderlang.egg-info/entry_points.txt
--rw-rw-r--   0 eons      (1000) eons      (1000)       37 2024-03-13 05:24:29.000000 elderlang-0.0.3/pkg/elderlang.egg-info/requires.txt
--rw-rw-r--   0 eons      (1000) eons      (1000)       10 2024-03-13 05:24:29.000000 elderlang-0.0.3/pkg/elderlang.egg-info/top_level.txt
--rw-rw-r--   0 eons      (1000) eons      (1000)      104 2024-03-13 05:24:05.000000 elderlang-0.0.3/pyproject.toml
--rw-rw-r--   0 eons      (1000) eons      (1000)      764 2024-03-13 05:24:29.897786 elderlang-0.0.3/setup.cfg
+drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2024-04-13 06:59:41.563897 elderlang-0.0.4/
+-rw-r--r--   0 eons      (1000) eons      (1000)      524 2024-04-13 06:59:41.559897 elderlang-0.0.4/PKG-INFO
+-rw-rw-r--   0 eons      (1000) eons      (1000)       20 2024-04-13 06:59:02.000000 elderlang-0.0.4/README.md
+drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2024-04-13 06:59:41.371897 elderlang-0.0.4/pkg/
+drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2024-04-13 06:59:41.471897 elderlang-0.0.4/pkg/elderlang/
+-rw-rw-r--   0 eons      (1000) eons      (1000)       80 2024-04-13 06:59:11.000000 elderlang-0.0.4/pkg/elderlang/__init__.py
+-rw-rw-r--   0 eons      (1000) eons      (1000)       67 2024-04-13 06:59:11.000000 elderlang-0.0.4/pkg/elderlang/__main__.py
+-rw-rw-r--   0 eons      (1000) eons      (1000)   241280 2024-04-13 06:59:11.000000 elderlang-0.0.4/pkg/elderlang/elderlang.py
+drwxrwxr-x   0 eons      (1000) eons      (1000)        0 2024-04-13 06:59:41.551897 elderlang-0.0.4/pkg/elderlang.egg-info/
+-rw-r--r--   0 eons      (1000) eons      (1000)      524 2024-04-13 06:59:41.000000 elderlang-0.0.4/pkg/elderlang.egg-info/PKG-INFO
+-rw-rw-r--   0 eons      (1000) eons      (1000)      337 2024-04-13 06:59:41.000000 elderlang-0.0.4/pkg/elderlang.egg-info/SOURCES.txt
+-rw-rw-r--   0 eons      (1000) eons      (1000)        1 2024-04-13 06:59:41.000000 elderlang-0.0.4/pkg/elderlang.egg-info/dependency_links.txt
+-rw-rw-r--   0 eons      (1000) eons      (1000)       46 2024-04-13 06:59:41.000000 elderlang-0.0.4/pkg/elderlang.egg-info/entry_points.txt
+-rw-rw-r--   0 eons      (1000) eons      (1000)       16 2024-04-13 06:59:41.000000 elderlang-0.0.4/pkg/elderlang.egg-info/requires.txt
+-rw-rw-r--   0 eons      (1000) eons      (1000)       10 2024-04-13 06:59:41.000000 elderlang-0.0.4/pkg/elderlang.egg-info/top_level.txt
+-rw-rw-r--   0 eons      (1000) eons      (1000)      104 2024-04-13 06:59:11.000000 elderlang-0.0.4/pyproject.toml
+-rw-rw-r--   0 eons      (1000) eons      (1000)      742 2024-04-13 06:59:41.567897 elderlang-0.0.4/setup.cfg
```

### Comparing `elderlang-0.0.3/PKG-INFO` & `elderlang-0.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: elderlang
-Version: 0.0.3
+Version: 0.0.4
 Summary: The Elder Language
 Home-page: https://github.com/elderlang/elderlang
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/elderlang/elderlang/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: jsonpickle
-Requires-Dist: elderlangdefinitions
 Requires-Dist: eons
 
 # Elder
 
 coming soon
```

### Comparing `elderlang-0.0.3/pkg/elderlang/elderlang.py` & `elderlang-0.0.4/pkg/elderlang/elderlang.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 import copy
 import inspect
 import jsonpickle # NOTE: both pickle & dill fail to save and restore the Parser; however jsonpickle appears to work.
 from pathlib import Path
 from collections import OrderedDict
 from collections import defaultdict
 from collections import Counter
-import elderlangdefinitions
 import os
 import types
 from copy import deepcopy
 from typing import Any
 
 ######## START CONTENT ########
 
 class Structure (eons.Functor):
+
 	def __init__(this, name="Structure"):
 		super().__init__(name)
 
 		# Used when parsing. Terrible name per Sly.
 		this.optionalKWArgs['p'] = None
 
 		this.optionalKWArgs['exclusions'] = []
@@ -33,14 +33,18 @@
 			'this',
 		]
 		this.fetch.attr.use = []
 
 	def Function(this):
 		pass
 
+	def GetProduct(this, index):
+		# No mangling necessary.. yet..
+		return this.p[index]
+
 	def Engulf(this, substrate, escape=False):
 		if (
 			substrate is None
 			or isinstance(substrate, bool)
 			or isinstance(substrate, int)
 			or isinstance(substrate, float)
 			or isinstance(substrate, list)
@@ -79,15 +83,15 @@
 	# We must also filter for EOL tokens.
 	possibleContent = None
 	i = 0
 	failedMatches = []
 	reject = [r'^\s*$'] + openings + closings
 	while (True):
 		try:
-			possibleContent = this.p[i]
+			possibleContent = this.GetProduct(i)
 			logging.debug(f"{this.name} Block has possibleContent '{possibleContent}' ({i}).")
 
 			if (isinstance(possibleContent, str)):
 				if (not len(possibleContent)):
 					i += 1
 					continue
 
@@ -125,15 +129,15 @@
 # SymmetricBlocks use the same symbols for both openings and closings.
 @eons.kind(Block)
 def SymmetricBlock(
 	openings = [],
 	content = "",
 ):
 	# SymmetricBlocks should always have 1 opening and 1 closing.
-	return this.p[1]
+	return this.GetProduct(1)
 
 # OpenEndedBlocks only specify openings.
 # They are closed by the beginning of another block.
 # To make this possible, we just reinterpret closings as a list of blocks, not regexes.
 # NOTE: All OpenEndedBlocks are terminated by the end of the line (r'$')
 # NOTE: OpenEndedBlocks are not allowed to be nested: they are also automatically closed by all listed openings.
 @eons.kind(Block)
@@ -160,89 +164,100 @@
 @eons.kind(Block)
 def CatchAllBlock(
 	specialStarts = [
 		# Example only
 		# '/',
 	],
 ):
-	return this.p[0]
+	return this.GetProduct(0)
 
 # Expressions build the contents of all other Blocks beside the CatchAllBlock.
 @eons.kind(OpenEndedBlock)
 def Expression(
 	openings = [r';', r','],
 	nest = [], # List of blocks that can be nested inside this block.
 	exclusions = [
 		'EOL',
 	]
 ):
-	return this.Engulf(this.p[0])
+	return this.Engulf(this.GetProduct(0))
 
 # ExpressionSet is constructed from a series of Expressions.
 # Each nest in a Expression is realized through a ExpressionSet.
 @eons.kind(Block)
 def ExpressionSet():
 
-	if (isinstance(this.p[0], str)):
-		if (not len(this.p[0])):
+	if (isinstance(this.GetProduct(0), str)):
+		if (not len(this.GetProduct(0))):
 			return []
-		return [this.Engulf(this.p[0])]
-	elif (isinstance(this.p[0], int) or isinstance(this.p[0], float)):
-		return [this.p[0]]
+		return [this.Engulf(this.GetProduct(0))]
+	elif (isinstance(this.GetProduct(0), int) or isinstance(this.GetProduct(0), float)):
+		return [this.GetProduct(0)]
 
-	ret = this.p[0]
+	ret = this.GetProduct(0)
 
-	if (isinstance(this.p[0], list)):
+	if (isinstance(this.GetProduct(0), list)):
 		try:
-			if (isinstance(this.p[1], list)):
-				ret = this.p[0] + this.p[1]
-			elif (isinstance(this.p[1], str)):
-				if (not len(this.p[1])):
-					ret = this.p[0]
+			if (isinstance(this.GetProduct(1), list)):
+				ret = this.GetProduct(0) + this.GetProduct(1)
+			elif (isinstance(this.GetProduct(1), str)):
+				if (not len(this.GetProduct(1))):
+					ret = this.GetProduct(0)
 				else:
-					ret = this.p[0] + [this.Engulf(this.p[1])]
+					ret = this.GetProduct(0) + [this.Engulf(this.GetProduct(1))]
 			else:
-				ret.append(this.Engulf(this.p[1]))
+				ret.append(this.Engulf(this.GetProduct(1)))
 		except Exception as e:
 			pass
 	
 	return ret
 
 @eons.kind(SymmetricBlock)
 def UnformattedString(
 	openings = [r"\'"],
 	representation = "\\'UNFORMATTED_STRING\\'", #NOT a raw string
 	content = None,
 	overrides = [
 		'prioritize',
 	],
+	inclusions = [
+		'newline',
+	],
 ):
 	# UnformattedStrings are lexed wholesale.
-	return f"String('{this.Engulf(this.p[0], escape=True)}')"
+	string = this.Engulf(this.GetProduct(0), escape=True)
+
+	# Escape any newline characters.
+	string = string.replace('\n', '\\n')
+
+	return f"String('{string}')"
 
 @eons.kind(SymmetricBlock)
 def FormattedString(
 	lexer = None,
 	parser = None,
 	openings = [r'"', r'`'],
 	representation = '\"FORMATTED_STRING\"', #NOT a raw string
 	content = None,
 	nest = [
 		'Execution',
 	],
 	overrides = [
 		'prioritize',
 	],
+	inclusions = [
+		'newline',
+	],
 ):
 	if (lexer is None):
 		lexer = this.executor.Fetch('lexer')
 	if (parser is None):
 		parser = this.executor.Fetch('parser')
 
-	rawString = f"'{this.p[0][1:-1]}'" # Standardize quotations
+	rawString = f"'{this.GetProduct(0)[1:-1]}'" # Standardize quotations
 
 	# This is what we want to do, but python does not support the P<-...> module (only P<...>)
 	# executionBlocks = re.findall(r'{(?:[^{}]|(?P<open>{)|(?P<-open>}))*(?(open)(?!))}', rawString)
 
 	executionBlocks = []
 
 	openCount = 0
@@ -263,17 +278,24 @@
 
 	# logging.critical(f"Execution blocks: {executionBlocks}")
 
 	stringComponents = [rawString]
 	for i, block in enumerate(executionBlocks):
 		stringComponents[0] = stringComponents[0].replace(f"{{{block}}}", r"%s", 1)
 		stringComponents.append(parser.parse(lexer.tokenize(block)))
+	
+	# Escape any newline characters only AFTER the rawString has been processed.
+	stringComponents[0] = stringComponents[0].replace('\n', '\\\\n')
 
 	# logging.critical(f"String components: {stringComponents}")
 
+	# Wipe result data, since our return value here can apparently be clobbered by the parser calls.
+	import eons #huh?
+	this.result.data = eons.util.DotDict()
+
 	return f"String({', '.join([str(c) for c in stringComponents])})"
 
 @eons.kind(MetaBlock)
 def String(
 	compose = [
 		'UnformattedString',
 		'FormattedString',
@@ -281,60 +303,64 @@
 	representation = r'`STRING`',
 	content = None,
 	exclusions = ['lexer'],
 	overrides = [
 		'prioritize',
 	],
 ):
-	return this.p[0] # already parsed.
+	return this.GetProduct(0) # already parsed.
 
 @eons.kind(Block)
 def BlockComment(
 	openings = [r'/\*'],
 	closings = [r'\*/'],
 	representation = r'/\*BLOCK_COMMENT\*/',
 	content = None,
 	exclusions = [
 		'tokens',
 		'parser',
 	],
 	inclusions = [
 		'newline',
+		'space.padding',
 	],
 ):
 	return ''
 
 @eons.kind(OpenEndedBlock)
 def LineComment(
 	openings = [r'#', r'//'],
 	closings = [],
 	representation = r'//LINE_COMMENT',
 	content = None,
 	exclusions = [
 		'tokens',
 		'parser',
 	],
+	inclusions = [
+		'space.padding',
+	],
 ):
 	return ''
 
 @eons.kind(OpenEndedBlock)
 def Kind(
 	openings = [r':'],
 	closings = [],
 	representation = r':KIND',
 	content = "LimitedExpression",
 ):
 	if (len(this.p) <= 1):
 		return "Kind()"
 
-	if (this.p[0] in openings and this.p[1] in openings):
+	if (this.GetProduct(0) in openings and this.GetProduct(1) in openings):
 		return "Kind()"
-	if (this.p[0].startswith('Kind')):
-		return this.p[0]
-	kind = this.Engulf(this.p[1], escape=True)
+	if (this.GetProduct(0).startswith('Kind')):
+		return this.GetProduct(0)
+	kind = this.Engulf(this.GetProduct(1), escape=True)
 	if (len(kind)):
 		kind = f"'{kind}'"
 	return f"Kind({kind})"
 
 @eons.kind(Block)
 def Parameter(
 	openings = [r'\('],
@@ -404,65 +430,65 @@
 @eons.kind(BlockSyntax)
 def Invokation():
 	pass
 
 @eons.kind(FlexibleTokenSyntax)
 def OperatorOverload():
 	args = {
-		'name': this.p[0],
-		'kind': this.Engulf(this.p[1]),
+		'name': this.GetProduct(0),
+		'kind': this.Engulf(this.GetProduct(1)),
 		'parameter': None,
 		'execution': None,
 	}
 	if (len(this.p) == 3):
-		args['execution'] = this.Engulf(this.p[2])
+		args['execution'] = this.Engulf(this.GetProduct(2))
 	elif (len(this.p) == 4):
-		args['parameter'] = this.Engulf(this.p[2])
-		args['execution'] = this.Engulf(this.p[3])
+		args['parameter'] = this.Engulf(this.GetProduct(2))
+		args['execution'] = this.Engulf(this.GetProduct(3))
 
 	argString = ','.join([f'{k}={v}' for k, v in args.items()])
 
 	return f"Type({argString})"
 
 
 @eons.kind(BlockSyntax)
 def SimpleType(
 	blocks = [
 		'Name',
 		'Kind',
 	],
 ):
-	return f"Type(name={this.p[0]},kind={this.Engulf(this.p[1])})"
+	return f"Type(name={this.GetProduct(0)},kind={this.Engulf(this.GetProduct(1))})"
 
 @eons.kind(BlockSyntax)
 def ContainerAccess(
 	blocks = [
 		'Name',
 		'Container',
 	]
 ):
-	return f"Within(name={this.p[0]},container={this.Engulf(this.p[1])})"
+	return f"Within(name={this.GetProduct(0)},container={this.Engulf(this.GetProduct(1))})"
 
 @eons.kind(Invokation)
 def StandardInvokation(
 	blocks = [
 		'Name',
 		'Parameter',
 	]
 ):
-	return f"Invoke(name={this.p[0]},parameter={this.Engulf(this.p[1])})"
+	return f"Invoke(name={this.GetProduct(0)},parameter={this.Engulf(this.GetProduct(1))})"
 
 @eons.kind(Invokation)
 def AccessInvokation(
 	blocks = [
 		'ExplicitAccess',
 		'Parameter',
 	]
 ):
-	return f"Invoke(source='{this.Engulf(this.p[0], escape=True)}',parameter={this.Engulf(this.p[1])})"
+	return f"Invoke(source='{this.Engulf(this.GetProduct(0), escape=True)}',parameter={this.Engulf(this.GetProduct(1))})"
 
 @eons.kind(AccessInvokation)
 def ComplexAccessInvokation(
 	blocks = [
 		'ComplexExplicitAccess',
 		'Parameter',
 	]
@@ -472,90 +498,90 @@
 @eons.kind(Invokation)
 def InvokationWithExecution(
 	blocks = [
 		'Name',
 		'Execution',
 	]
 ):
-	return f"Invoke(name={this.p[0]},execution={this.Engulf(this.p[1])})"
+	return f"Invoke(name={this.GetProduct(0)},execution={this.Engulf(this.GetProduct(1))})"
 
 @eons.kind(BlockSyntax)
 def StructType(
 	blocks = [
 		'Name',
 		'Kind',
 		'Parameter',
 	],
 ):
-	if (this.p[0].startswith('Type')):
-		return f"{this.p[0][:-1]},parameter={this.Engulf(this.p[1])})"
-	return f"Type(name={this.p[0]},kind={this.Engulf(this.p[1])},parameter={this.Engulf(this.p[2])})"
+	if (this.GetProduct(0).startswith('Type')):
+		return f"{this.GetProduct(0)[:-1]},parameter={this.Engulf(this.GetProduct(1))})"
+	return f"Type(name={this.GetProduct(0)},kind={this.Engulf(this.GetProduct(1))},parameter={this.Engulf(this.GetProduct(2))})"
 
 # Executive type is terminal. No other types build on it.
 @eons.kind(BlockSyntax)
 def ExecutiveType(
 	blocks = [
 		'Name',
 		'Kind',
 		'Execution',
 	],
 ):
-	if (this.p[0].startswith('Type')):
-		return f"{this.p[0][:-1]},execution={this.Engulf(this.p[1])})"
-	return f"Type(name={this.p[0]},kind={this.Engulf(this.p[1])},execution={this.Engulf(this.p[2])})"
+	if (this.GetProduct(0).startswith('Type')):
+		return f"{this.GetProduct(0)[:-1]},execution={this.Engulf(this.GetProduct(1))})"
+	return f"Type(name={this.GetProduct(0)},kind={this.Engulf(this.GetProduct(1))},execution={this.Engulf(this.GetProduct(2))})"
 
 @eons.kind(Invokation)
 def InvokationWithParametersAndExecution(
 	blocks = [
 		'Name',
 		'Parameter',
 		'Execution',
 	]
 ):
-	if (this.p[0].startswith('Invoke')):
-		return f"{this.p[0][:-1]},execution={this.Engulf(this.p[1])})"
-	return f"Invoke(name={this.p[0]},parameter={this.Engulf(this.p[1])},execution={this.Engulf(this.p[2])})"
+	if (this.GetProduct(0).startswith('Invoke')):
+		return f"{this.GetProduct(0)[:-1]},execution={this.Engulf(this.GetProduct(1))})"
+	return f"Invoke(name={this.GetProduct(0)},parameter={this.Engulf(this.GetProduct(1))},execution={this.Engulf(this.GetProduct(2))})"
 
 @eons.kind(Invokation)
 def ContainerInvokation(
 	blocks = [
 		'Name',
 		'Container',
 		'Execution',
 	],
 ):
-	if (this.p[0].startswith('Within')):
-		return f"{this.p[0][:-1]},execution={this.Engulf(this.p[1])})"
-	return f"Within(name={this.p[0]},container={this.Engulf(this.p[1])},execution={this.Engulf(this.p[2])})"
+	if (this.GetProduct(0).startswith('Within')):
+		return f"{this.GetProduct(0)[:-1]},execution={this.Engulf(this.GetProduct(1))})"
+	return f"Within(name={this.GetProduct(0)},container={this.Engulf(this.GetProduct(1))},execution={this.Engulf(this.GetProduct(2))})"
 
 @eons.kind(Invokation)
 def ContainerInvokationWithParameters(
 	blocks = [
 		'Name',
 		'Parameter',
 		'Container',
 		'Execution',
 	],
 ):
-	if (this.p[0].startswith('Invoke')):
-		return f"{this.p[0][:-1]},container={this.Engulf(this.p[1])},execution={this.Engulf(this.p[2])})"
-	return f"Invoke(name={this.p[0]},parameter={this.Engulf(this.p[1])},container={this.Engulf(this.p[2])},execution={this.Engulf(this.p[3])})"
+	if (this.GetProduct(0).startswith('Invoke')):
+		return f"{this.GetProduct(0)[:-1]},container={this.Engulf(this.GetProduct(1))},execution={this.Engulf(this.GetProduct(2))})"
+	return f"Invoke(name={this.GetProduct(0)},parameter={this.Engulf(this.GetProduct(1))},container={this.Engulf(this.GetProduct(2))},execution={this.Engulf(this.GetProduct(3))})"
 
 @eons.kind(BlockSyntax)
 def FunctorType(
 	blocks = [
 		'Name',
 		'Kind',
 		'Parameter',
 		'Execution',
 	],
 ):
-	if (this.p[0].startswith('Type')):
-		return f"{this.p[0][:-1]},execution={this.Engulf(this.p[1])})"
-	return f"Type(name={this.p[0]},kind={this.Engulf(this.p[1])},parameter={this.Engulf(this.p[2])},execution={this.Engulf(this.p[3])})"
+	if (this.GetProduct(0).startswith('Type')):
+		return f"{this.GetProduct(0)[:-1]},execution={this.Engulf(this.GetProduct(1))})"
+	return f"Type(name={this.GetProduct(0)},kind={this.Engulf(this.GetProduct(1))},parameter={this.Engulf(this.GetProduct(2))},execution={this.Engulf(this.GetProduct(3))})"
 
 @eons.kind(ExactSyntax)
 def EOL(
 	match = r'[\\n\\r\\s]+',
 	exclusions = [
 		'parser',
 	],
@@ -621,15 +647,15 @@
 		}
 	],
 	recurseOn = "name",
 	overrides = [
 		'deprioritize'
 	]
 ):
-	return f"Autofill('{this.Engulf(this.p[0], escape=True)}','{this.Engulf(this.p[1], escape=True)}')"
+	return f"Autofill('{this.Engulf(this.GetProduct(0), escape=True)}','{this.Engulf(this.GetProduct(1), escape=True)}')"
 
 @eons.kind(FlexibleTokenSyntax)
 def AutofillInvokation(
 	match = [
 		{
 			'first': [
 				r'name',
@@ -683,22 +709,22 @@
 			],
 		}
 	],
 	overrides = [
 		'deprioritize'
 	]
 ):
-	return f"Call('{this.Engulf(this.p[0], escape=True)}',{this.Engulf(str(this.p[1]))})"
+	return f"Call('{this.Engulf(this.GetProduct(0), escape=True)}',{this.Engulf(str(this.GetProduct(1)))})"
 
 @eons.kind(ExactSyntax)
 def Sequence(
 	match = r'NAME/NAME',
 	# recurseOn = "name" # Now handled by ComplexSequence
 ):
-	return f"Sequence({this.p[0]},{this.p[2]})"
+	return f"Sequence({this.GetProduct(0)},{this.GetProduct(2)})"
 
 @eons.kind(FlexibleTokenSyntax)
 def ComplexSequence(
 	match = [
 		{
 			'first': [
 				r'sequence',
@@ -748,15 +774,15 @@
 				r'complexepidef',
 				r'globalscope',
 				r'caller',
 			],
 		}
 	]
 ):
-	return f"Sequence('{this.Engulf(this.p[0], escape=True)}','{this.Engulf(this.p[2], escape=True)}')"
+	return f"Sequence('{this.Engulf(this.GetProduct(0), escape=True)}','{this.Engulf(this.GetProduct(2), escape=True)}')"
 
 @eons.kind(OperatorOverload)
 def DivisionOverload(
 	match = [
 		r'SEQUENCE kind',
 		r'SEQUENCE kind execution',
 		r'SEQUENCE kind parameter execution',
@@ -767,15 +793,15 @@
 
 # We have to specify the /= operator to prevent it from getting caught in a SEQUENCE match.
 # TODO: Is there a fancier way to do a negative look ahead of an already matched name, so that we can include this logic in the SEQUENCE match?
 @eons.kind(ExactSyntax)
 def DivisionAssignment(
 	match = r'NAME/=NAME',
 ):
-	return f"{this.Engulf(this.p[0])} /= {this.Engulf(this.p[2])}"
+	return f"{this.Engulf(this.GetProduct(0))} /= {this.Engulf(this.GetProduct(2))}"
 
 # NOTE: Sequences and division CANNOT be combined.
 @eons.kind(FlexibleTokenSyntax)
 def ComplexDivisionAssignment(
 	match = [
 		{
 			'first': [
@@ -825,15 +851,15 @@
 				r'complexepidef',
 				r'globalscope',
 				r'caller',
 			],
 		}
 	]
 ):
-	return f"{this.Engulf(str(this.p[0]))} /= {this.Engulf(str(this.p[2]))}"
+	return f"{this.Engulf(str(this.GetProduct(0)))} /= {this.Engulf(str(this.GetProduct(2)))}"
 
 @eons.kind(OperatorOverload)
 def DivisionAssignmentOverload(
 	match = [
 		r'DIVISIONASSIGNMENT kind',
 		r'DIVISIONASSIGNMENT kind execution',
 		r'DIVISIONASSIGNMENT kind parameter execution',
@@ -842,15 +868,15 @@
 	return this.parent.Function(this)
 
 @eons.kind(ExactSyntax)
 def ExplicitAccess(
 	match = r'NAME\.NAME',
 	# recurseOn = "name" # Now handled by ComplexExplicitAccess
 ):
-	return f"Get({this.p[0]},{this.p[2]})"
+	return f"Get({this.GetProduct(0)},{this.GetProduct(2)})"
 
 @eons.kind(FlexibleTokenSyntax)
 def ComplexExplicitAccess(
 	match = [
 		{
 			'first': [
 				r'explicitaccess',
@@ -882,48 +908,48 @@
 			'third': [
 				r'standardinvokation',
 				r'containeraccess',
 			],
 		},
 	]
 ):
-	return f"Get('{this.Engulf(this.p[0], escape=True)}','{this.Engulf(this.p[2], escape=True)}')"
+	return f"Get('{this.Engulf(this.GetProduct(0), escape=True)}','{this.Engulf(this.GetProduct(2), escape=True)}')"
 
 @eons.kind(ExactSyntax)
 def ShortType(
 	match = r'NAME\s+:=\s+'
 ):
-	return f"Get(Type(name={this.p[0]}),'=')"
+	return f"Get(Type(name={this.GetProduct(0)}),'=')"
 
 @eons.kind(FlexibleTokenSyntax)
 def SimpleTypeWithShortTypeAssignment(
 	match = [r'name OPEN_KIND limitedexpression SHORTTYPE']
 ):
-	return f"Get(Type(name={this.Engulf(this.p[0])}, kind={this.Engulf(this.p[2])}))"
+	return f"Get(Type(name={this.Engulf(this.GetProduct(0))}, kind={this.Engulf(this.GetProduct(2))}))"
 
 @eons.kind(ExactSyntax)
 def This(
 	match = r'\./NAME'
 ):
-	toAccess = this.Engulf(this.p[1][1:-1])
+	toAccess = this.Engulf(this.GetProduct(1)[1:-1])
 	if (toAccess.startswith('this')):
 		return toAccess
 	return f"this.{toAccess}"
 
 @eons.kind(ExactSyntax)
 def EpidefOption1(
 	match = r'\.\.NAME'
 ):
-	return f"this.epidef.{this.Engulf(this.p[1][1:-1])}"
+	return f"this.epidef.{this.Engulf(this.GetProduct(1)[1:-1])}"
 
 @eons.kind(ExactSyntax)
 def EpidefOption2(
 	match = r'\.\./NAME'
 ):
-	return f"this.epidef.{this.Engulf(this.p[1][1:-1])}"
+	return f"this.epidef.{this.Engulf(this.GetProduct(1)[1:-1])}"
 
 @eons.kind(FlexibleTokenSyntax)
 def ComplexEpidef(
 	match = [
 		{
 			'first': [
 				r'EPIDEFOPTION2'
@@ -932,49 +958,49 @@
 				r'epidefoption1',
 				r'epidefoption2',
 				r'complexepidef'
 			]
 		}
 	]
 ):
-	return f"this.epidef.{this.Engulf(this.p[1][5:])}"
+	return f"this.epidef.{this.Engulf(this.GetProduct(1)[5:])}"
 
 @eons.kind(ExactSyntax)
 def GlobalScope(
 	match = r'~/NAME'
 ):
-	return f"HOME.Instance().{this.Engulf(this.p[1][1:-1])}"
+	return f"HOME.Instance().{this.Engulf(this.GetProduct(1)[1:-1])}"
 
 @eons.kind(ExactSyntax)
 def Caller(
 	match = r'@NAME',
 ):
 	# Enable @@... to become this.caller.caller...
-	toAccess = this.Engulf(this.p[1][1:-1])
+	toAccess = this.Engulf(this.GetProduct(1)[1:-1])
 	if (toAccess.startswith('this.caller')):
 		return f"this.caller.{toAccess[5:]}"
 	return f"this.caller.{toAccess}"
 
 
 # These don't actually do anything, they just help in ordering the files appropriately.
 
 @eons.kind(CatchAllBlock)
 def Name(
 	representation = r'NAME',
 ):
-	return f"'{this.p[0]}'"
+	return f"'{this.GetProduct(0)}'"
 
 @eons.kind(Expression)
 def ProtoExpression(
 	representation = r'PROTOEXPRESSION',
 	nest = [
 		'Name',
 		'Number',
 		'String',
-		
+
 		# ExactSyntaxes
 		'AutofillAccessOrInvokation',
 		'AutofillInvokation',
 		'Sequence',
 		'DivisionAssignment',
 		'This',
 		'ExplicitAccess',
@@ -1023,14 +1049,16 @@
 	return this.parent.Function(this)
 
 
 @eons.kind(Expression)
 def FullExpression(
 	representation = r'FULLEXPRESSION',
 	nest = [
+		# 'close_expression',
+
 		'LimitedExpression',
 		'LimitedExpressionSet',
 		'Kind',
 		# 'Parameter',
 
 		# BlockSyntaxes
 		'FunctorType',
@@ -1739,18 +1767,33 @@
 	__slots__ = ('_slice', '_namemap', '_stack')
 	def __init__(self, s, stack=None):
 		self._slice = s
 		self._namemap = { }
 		self._stack = stack
 
 	def __getitem__(self, n):
+		ret = None
 		if n >= 0:
-			return self._slice[n].value
+			try: 
+				ret = self._slice[n].value
+				# if (hasattr(ret, 'type') and ret.type == '$end'):
+				# 	ret = self.__getitem__(n+1)
+				# else:
+				# 	ret = ret.value
+			except Exception as e:
+				logging.debug(f'Could not get {self._slice}[{n}].value: {e}')
+				return None
 		else:
-			return self._stack[n].value
+			try:
+				ret = self._stack[n].value
+			except Exception as e:
+				logging.debug(f'Could not get {self._stack}[{n}].value: {e}')
+				return None
+		
+		return ret
 
 	def __setitem__(self, n, v):
 		if n >= 0:
 			self._slice[n].value = v
 		else:
 			self._stack[n].value = v
 
@@ -3459,19 +3502,19 @@
 	def __getitem__(self, key):
 		if key not in self and key.isupper() and key[:1] != '_':
 			return key.upper()
 		else:
 			return super().__getitem__(key)
 
 def _decorator(rule, *extra):
-	 rules = [rule, *extra]
-	 def decorate(func):
-		 func.rules = [ *getattr(func, 'rules', []), *rules[::-1] ]
-		 return func
-	 return decorate
+	rules = [rule, *extra]
+	def decorate(func):
+		func.rules = [ *getattr(func, 'rules', []), *rules[::-1] ]
+		return func
+	return decorate
 
 class ParserMeta(type):
 	@classmethod
 	def __prepare__(meta, *args, **kwargs):
 		d = ParserMetaDict()
 		d['_'] = _decorator
 		return d
@@ -3602,15 +3645,15 @@
 		if len(unused_rules) == 1:
 			logging.warning('There is 1 unused rule')
 		if len(unused_rules) > 1:
 			logging.warning('There are %d unused rules', len(unused_rules))
 
 		unreachable = grammar.find_unreachable()
 		for u in unreachable:
-		   logging.warning('Symbol %r is unreachable', u)
+			logging.warning('Symbol %r is unreachable', u)
 
 		if len(undefined_symbols) == 0:
 			infinite = grammar.infinite_cycles()
 			for inf in infinite:
 				errors += 'Infinite recursion detected for symbol %r\n' % inf
 
 		unused_prec = grammar.unused_precedence()
@@ -3701,19 +3744,19 @@
 	def error(self, token):
 		'''
 		Default error handling function.  This may be subclassed.
 		'''
 		if token:
 			lineno = getattr(token, 'lineno', 0)
 			if lineno:
-				sys.stderr.write(f'sly: Syntax error at line {lineno}, token={token.type}\n')
+				logging.critical(f'sly: Syntax error at line {lineno}, token={token.type}\n')
 			else:
-				sys.stderr.write(f'sly: Syntax error, token={token.type}')
+				logging.critical(f'sly: Syntax error, token={token.type}')
 		else:
-			sys.stderr.write('sly: Parse error in input. EOF\n')
+			logging.critical('sly: Parse error in input. EOF\n')
  
 	def errok(self):
 		'''
 		Clear the error status
 		'''
 		self.errorok = True
 
@@ -3725,14 +3768,34 @@
 		del self.symstack[:]
 		sym = YaccSymbol()
 		sym.type = '$end'
 		self.symstack.append(sym)
 		self.statestack.append(0)
 		self.state = 0
 
+	def does_current_production_match_symbols(self, symstack):
+		if (not self.production.len):
+			return True
+
+		# Some tokens are deliberately injected into the symbol stack to help with parsing.
+		# TODO: Make this dynamic.
+		if (self.production.name == "close_expression"):
+			return True
+
+		if (self.production.len > len(symstack)):
+			return False
+		
+		alignment = dict(zip([sym.type for sym in symstack[-self.production.len:]], list(self.production.namemap.keys())))
+		logging.debug(f"Checking alignment of {alignment}")
+		for sym, name in alignment.items():
+			if (not name.startswith(sym)):
+				return False
+		
+		return True
+
 	def parse(self, tokens):
 		'''
 		Parse the given input tokens.
 		'''
 		lookahead = None								  # Current lookahead symbol
 		lookaheadstack = []							   # Stack of lookahead symbols
 		actions = self._lrtable.lr_action				 # Local reference to action table (to avoid lookup on self.)
@@ -3791,24 +3854,58 @@
 					# Decrease error count on successful shift
 					if errorcount:
 						errorcount -= 1
 					continue
 
 				if t < 0:
 					# reduce a symbol on the stack, emit a production
-					self.production = p = prod[-t]
-					pname = p.name
-					plen  = p.len
-					pslice._namemap = p.namemap
+					self.production = prod[-t]
+					pname = self.production.name
+					plen  = self.production.len
+
+					# The following match logic has been added to account for situations where one production might match multiple different sets of symbols, each of a possibly different size.
+					# Usually, we don't need to worry about the symbol stacking matching exactly which production to use, since the functions are all the same.
+					# However, if the match is incorrect and uses, say a size larger than the symbol stack or some other erroneous value, we'll crash.
+					# So, for added safety, we take the time to make sure we select exactly the right production.
+					# TODO: If we ever start adding data to the parsing table, we should add the match length so we can skip this calculation.
+
+					matched = self.does_current_production_match_symbols(symstack)
+					if (not matched):
+						logging.debug(f"Attempting to correct improper product selection for {pname} in {symstack}")
+
+						offset = 0
+						while (not matched):
+							offset += 1
+							try:
+								possibleCorrectMatch = prod[-t-offset]
+								if (possibleCorrectMatch.name != pname):
+									break
+
+								logging.debug(f"Possible correct match: {possibleCorrectMatch.name} ({possibleCorrectMatch.namemap})")
+								self.production = possibleCorrectMatch
+
+								if (self.does_current_production_match_symbols(symstack)):
+									logging.debug(f"Correct match found: {possibleCorrectMatch.name} ({possibleCorrectMatch.namemap})")
+									plen = possibleCorrectMatch.len
+									matched = True
+									break
+
+							except:
+								break
+
+						if (not matched):
+							raise RuntimeError(f"Parse error: {pname} ({p.namemap}) cannot be reduced from {symstack}")
+
+					p = self.production
 
-					# Call the production function
+					pslice._namemap = p.namemap
 					pslice._slice = symstack[-plen:] if plen else []
 
 					sym = YaccSymbol()
-					sym.type = pname	   
+					sym.type = pname
 					value = p.func(self, pslice)
 					if value is pslice:
 						value = (pname, *(s.value for s in pslice._slice))
 
 					sym.value = value
 						
 					# Record positions
@@ -3928,27 +4025,27 @@
 		return self._line_positions[id(value)]
 
 	def index_position(self, value):
 		return self._index_positions[id(value)]
 	
 
 class ElderLexer(Lexer):
-	def error(self, t):
-		print("Illegal character '%s'" % t.value[0])
-		self.index += 1
+	def error(this, t):
+		logging.critical(f"Illegal character {t.value[0]!r} at index {this.index}")
+		this.index += 1
 
 	tokens = { UNFORMATTEDSTRING, FORMATTEDSTRING, OPEN_EXECUTION, OPEN_PARAMETER, OPEN_CONTAINER, OPEN_KIND, CLOSE_EXECUTION, CLOSE_PARAMETER, CLOSE_CONTAINER, CLOSE_EXPRESSION, DIVISIONASSIGNMENT, THIS, EPIDEFOPTION2, EPIDEFOPTION1, GLOBALSCOPE, EXPLICITACCESS, SEQUENCE, EOL, SHORTTYPE, CALLER, NAME, NUMBER }
 
 	ignore = ' \t'
 
-	ignore_blockcomment = r'(/\*)[\s\S]*?(\*/)'
-	ignore_linecomment = r'(#|//)(?:(?!:\n).)+'
+	ignore_blockcomment = r'(/\*)[\s\S]*?(\*/)\s*'
+	ignore_linecomment = r'(#|//)(?:(?!:\n).)+\s*'
 
-	UNFORMATTEDSTRING = r'(\').*?(\')'
-	FORMATTEDSTRING = r'("|`).*?("|`)'
+	UNFORMATTEDSTRING = r'((\')[\s\S]*?([^\\]\'))'
+	FORMATTEDSTRING = r'((")[\s\S]*?([^\\]")|(`)[\s\S]*?([^\\]`))'
 	DIVISIONASSIGNMENT = r'(/=)'
 	NUMBER = r'\d+'
 	SHORTTYPE = r'(:=)'
 	OPEN_KIND = r'(:)'
 	OPEN_EXECUTION = r'\s*({)\s*'
 	OPEN_PARAMETER = r'\s*(\()\s*'
 	OPEN_CONTAINER = r'\s*(\[)\s*'
@@ -3960,15 +4057,15 @@
 	EPIDEFOPTION2 = r'(\.\./)'
 	EPIDEFOPTION1 = r'(\.\.)'
 	GLOBALSCOPE = r'(~/)'
 	EXPLICITACCESS = r'(\.)'
 	SEQUENCE = r'(/)'
 	CALLER = r'(@)'
 	EOL = r'([\n\r\s]+)'
-	NAME = r'(?:(?!{|}|\(|\)|\[|\]|:|/\*|\*/|#|//|\'|"|`|;|,|/=|\./|\.\./|\.\.|~/|\.|/|[\n\r\s]+|:=|@)\S)+'
+	NAME = r'(?:(?!\\|{|}|\(|\)|\[|\]|:|/\*|\*/|#|//|\'|"|`|;|,|/=|\./|\.\./|\.\.|~/|\.|/|[\n\r\s]+|:=|@)\S)+'
 
 	CLOSE_EXECUTION[''] = ['CLOSE_EXPRESSION', 'CLOSE_EXECUTION']
 	CLOSE_PARAMETER[''] = ['CLOSE_EXPRESSION', 'CLOSE_PARAMETER']
 	CLOSE_CONTAINER[''] = ['CLOSE_EXPRESSION', 'CLOSE_CONTAINER']
 
 
 class ElderParser(Parser):
@@ -4089,60 +4186,60 @@
 		pstr = ''.join([str(p[i]) for i in range(len(p))])
 		logging.info(f"Given {pstr}...")
 		ret = this.executor.Execute("InvokationWithExecution", p=p).returned
 		logging.info(f"...InvokationWithExecution produced {ret}")
 		return ret
 
 	@_(
-		'name kind parameter  %prec STRUCTTYPE',
 		'simpletype parameter  %prec STRUCTTYPE',
+		'name kind parameter  %prec STRUCTTYPE',
 	)
 	def structtype(this, p):
 		pstr = ''.join([str(p[i]) for i in range(len(p))])
 		logging.info(f"Given {pstr}...")
 		ret = this.executor.Execute("StructType", p=p).returned
 		logging.info(f"...StructType produced {ret}")
 		return ret
 
 	@_(
-		'name kind execution  %prec EXECUTIVETYPE',
 		'simpletype execution  %prec EXECUTIVETYPE',
+		'name kind execution  %prec EXECUTIVETYPE',
 	)
 	def executivetype(this, p):
 		pstr = ''.join([str(p[i]) for i in range(len(p))])
 		logging.info(f"Given {pstr}...")
 		ret = this.executor.Execute("ExecutiveType", p=p).returned
 		logging.info(f"...ExecutiveType produced {ret}")
 		return ret
 
 	@_(
-		'standardinvokation execution  %prec INVOKATIONWITHPARAMETERSANDEXECUTION',
 		'name parameter execution  %prec INVOKATIONWITHPARAMETERSANDEXECUTION',
+		'standardinvokation execution  %prec INVOKATIONWITHPARAMETERSANDEXECUTION',
 	)
 	def invokationwithparametersandexecution(this, p):
 		pstr = ''.join([str(p[i]) for i in range(len(p))])
 		logging.info(f"Given {pstr}...")
 		ret = this.executor.Execute("InvokationWithParametersAndExecution", p=p).returned
 		logging.info(f"...InvokationWithParametersAndExecution produced {ret}")
 		return ret
 
 	@_(
-		'name container execution  %prec CONTAINERINVOKATION',
 		'containeraccess execution  %prec CONTAINERINVOKATION',
+		'name container execution  %prec CONTAINERINVOKATION',
 	)
 	def containerinvokation(this, p):
 		pstr = ''.join([str(p[i]) for i in range(len(p))])
 		logging.info(f"Given {pstr}...")
 		ret = this.executor.Execute("ContainerInvokation", p=p).returned
 		logging.info(f"...ContainerInvokation produced {ret}")
 		return ret
 
 	@_(
-		'name parameter container execution  %prec CONTAINERINVOKATIONWITHPARAMETERS',
 		'standardinvokation container execution  %prec CONTAINERINVOKATIONWITHPARAMETERS',
+		'name parameter container execution  %prec CONTAINERINVOKATIONWITHPARAMETERS',
 	)
 	def containerinvokationwithparameters(this, p):
 		pstr = ''.join([str(p[i]) for i in range(len(p))])
 		logging.info(f"Given {pstr}...")
 		ret = this.executor.Execute("ContainerInvokationWithParameters", p=p).returned
 		logging.info(f"...ContainerInvokationWithParameters produced {ret}")
 		return ret
@@ -4182,16 +4279,16 @@
 		pstr = ''.join([str(p[i]) for i in range(len(p))])
 		logging.info(f"Given {pstr}...")
 		ret = this.executor.Execute("FullExpression", p=p).returned
 		logging.info(f"...FullExpression produced {ret}")
 		return ret
 
 	@_(
-		'structtype execution  %prec FUNCTORTYPE',
 		'name kind parameter execution  %prec FUNCTORTYPE',
+		'structtype execution  %prec FUNCTORTYPE',
 	)
 	def functortype(this, p):
 		pstr = ''.join([str(p[i]) for i in range(len(p))])
 		logging.info(f"Given {pstr}...")
 		ret = this.executor.Execute("FunctorType", p=p).returned
 		logging.info(f"...FunctorType produced {ret}")
 		return ret
@@ -6849,15 +6946,15 @@
 
 		parameters = {
 			'constructor': eons.util.DotDict({
 				'name': 'constructor',
 				'kind': inspect.Parameter.POSITIONAL_OR_KEYWORD,
 				'default': f'''
 if (this.name is None):
-	this.name = {this.name}
+	this.name = '{this.name}'
 
 if ('value' in kwargs):
 	this.value = kwargs['value']
 	del kwargs['value']
 '''
 			})
 		}
```

### Comparing `elderlang-0.0.3/pkg/elderlang.egg-info/PKG-INFO` & `elderlang-0.0.4/pkg/elderlang.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: elderlang
-Version: 0.0.3
+Version: 0.0.4
 Summary: The Elder Language
 Home-page: https://github.com/elderlang/elderlang
 Author: eons
 Author-email: support@eons.llc
 Project-URL: Bug Tracker, https://github.com/elderlang/elderlang/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: jsonpickle
-Requires-Dist: elderlangdefinitions
 Requires-Dist: eons
 
 # Elder
 
 coming soon
```

### Comparing `elderlang-0.0.3/setup.cfg` & `elderlang-0.0.4/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = elderlang
-version = 0.0.3
+version = 0.0.4
 author = eons
 author_email = support@eons.llc
 description = The Elder Language
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/elderlang/elderlang
@@ -18,15 +18,14 @@
 [options]
 package_dir = 
 	= pkg
 packages = find:
 python_requires = >=3.7
 install_requires = 
 	jsonpickle
-	elderlangdefinitions
 	eons
 
 [options.packages.find]
 where = pkg
 
 [options.entry_points]
 console_scripts =
```

