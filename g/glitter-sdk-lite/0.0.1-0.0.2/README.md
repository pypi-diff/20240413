# Comparing `tmp/glitter_sdk_lite-0.0.1.tar.gz` & `tmp/glitter_sdk_lite-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glitter_sdk_lite-0.0.1.tar", max compression
+gzip compressed data, was "glitter_sdk_lite-0.0.2.tar", max compression
```

## Comparing `glitter_sdk_lite-0.0.1.tar` & `glitter_sdk_lite-0.0.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1073 2024-04-04 03:26:11.278873 glitter_sdk_lite-0.0.1/LICENSE
--rw-r--r--   0        0        0       95 2024-04-04 03:26:11.279109 glitter_sdk_lite-0.0.1/README.md
--rw-r--r--   0        0        0       13 2024-04-04 03:26:11.280537 glitter_sdk_lite-0.0.1/glitter_sdk/.gitignore
--rw-r--r--   0        0        0      163 2024-04-04 03:26:11.280655 glitter_sdk_lite-0.0.1/glitter_sdk/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 03:26:11.280763 glitter_sdk_lite-0.0.1/glitter_sdk/client/__init__.py
--rw-r--r--   0        0        0       83 2024-04-07 07:10:39.384840 glitter_sdk_lite-0.0.1/glitter_sdk/client/lcd/__init__.py
--rw-r--r--   0        0        0     4995 2024-04-07 07:15:01.629120 glitter_sdk_lite-0.0.1/glitter_sdk/client/lcd/db.py
--rw-r--r--   0        0        0      431 2024-04-07 04:00:39.693586 glitter_sdk_lite-0.0.1/glitter_sdk/client/lcd/lcdclient.py
--rw-r--r--   0        0        0      150 2024-04-07 01:49:25.738295 glitter_sdk_lite-0.0.1/glitter_sdk/core/__init__.py
--rw-r--r--   0        0        0     5009 2023-09-03 07:54:13.159000 glitter_sdk_lite-0.0.1/glitter_sdk/core/bech32.py
--rw-r--r--   0        0        0      805 2023-09-03 07:54:13.306000 glitter_sdk_lite-0.0.1/glitter_sdk/core/msg.py
--rw-r--r--   0        0        0      188 2023-09-03 07:54:13.265000 glitter_sdk_lite-0.0.1/glitter_sdk/core/msgs/__init__.py
--rw-r--r--   0        0        0      813 2023-09-03 07:54:13.264000 glitter_sdk_lite-0.0.1/glitter_sdk/core/msgs/argument.py
--rw-r--r--   0        0        0     1927 2023-09-03 07:54:13.264000 glitter_sdk_lite-0.0.1/glitter_sdk/core/msgs/arguments.py
--rw-r--r--   0        0        0     2983 2023-09-03 07:54:13.274000 glitter_sdk_lite-0.0.1/glitter_sdk/core/msgs/msgs.py
--rw-r--r--   0        0        0      968 2024-04-04 03:26:11.302295 glitter_sdk_lite-0.0.1/glitter_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-04 03:26:11.303345 glitter_sdk_lite-0.0.1/glitter_sdk/util/__init__.py
--rw-r--r--   0        0        0     1678 2024-04-04 03:26:11.303468 glitter_sdk_lite-0.0.1/glitter_sdk/util/base.py
--rw-r--r--   0        0        0      878 2024-04-04 03:26:11.303687 glitter_sdk_lite-0.0.1/glitter_sdk/util/constants/CLIENT.py
--rw-r--r--   0        0        0      679 2024-04-04 03:26:11.303804 glitter_sdk_lite-0.0.1/glitter_sdk/util/constants/COMMAND.py
--rw-r--r--   0        0        0     1927 2024-04-04 03:26:11.303921 glitter_sdk_lite-0.0.1/glitter_sdk/util/constants/CR.py
--rw-r--r--   0        0        0    12296 2024-04-04 03:26:11.304090 glitter_sdk_lite-0.0.1/glitter_sdk/util/constants/ER.py
--rw-r--r--   0        0        0      370 2024-04-04 03:26:11.304209 glitter_sdk_lite-0.0.1/glitter_sdk/util/constants/FIELD_TYPE.py
--rw-r--r--   0        0        0      214 2024-04-04 03:26:11.304328 glitter_sdk_lite-0.0.1/glitter_sdk/util/constants/FLAG.py
--rw-r--r--   0        0        0      333 2024-04-04 03:26:11.304450 glitter_sdk_lite-0.0.1/glitter_sdk/util/constants/SERVER_STATUS.py
--rw-r--r--   0        0        0        0 2024-04-04 03:26:11.304508 glitter_sdk_lite-0.0.1/glitter_sdk/util/constants/__init__.py
--rw-r--r--   0        0        0     3253 2024-04-04 03:26:11.304632 glitter_sdk_lite-0.0.1/glitter_sdk/util/contract.py
--rw-r--r--   0        0        0      199 2024-04-04 03:26:11.304806 glitter_sdk_lite-0.0.1/glitter_sdk/util/converter.py
--rw-r--r--   0        0        0      211 2024-04-04 03:26:11.308892 glitter_sdk_lite-0.0.1/glitter_sdk/util/hash.py
--rw-r--r--   0        0        0      401 2024-04-04 03:26:11.309013 glitter_sdk_lite-0.0.1/glitter_sdk/util/highlight.py
--rw-r--r--   0        0        0     1696 2024-04-04 03:26:11.309132 glitter_sdk_lite-0.0.1/glitter_sdk/util/json.py
--rw-r--r--   0        0        0     1045 2024-04-04 03:26:11.309307 glitter_sdk_lite-0.0.1/glitter_sdk/util/parse_authorization.py
--rw-r--r--   0        0        0     2550 2024-04-04 03:26:11.309423 glitter_sdk_lite-0.0.1/glitter_sdk/util/parse_content.py
--rw-r--r--   0        0        0     3887 2024-04-04 03:26:11.309543 glitter_sdk_lite-0.0.1/glitter_sdk/util/parse_msg.py
--rw-r--r--   0        0        0      732 2024-04-04 03:26:11.309654 glitter_sdk_lite-0.0.1/glitter_sdk/util/parse_proto.py
--rw-r--r--   0        0        0     2950 2024-04-04 03:26:11.309779 glitter_sdk_lite-0.0.1/glitter_sdk/util/parse_query_str.py
--rw-r--r--   0        0        0    14729 2024-04-07 01:44:43.924396 glitter_sdk_lite-0.0.1/glitter_sdk/util/parse_sql.py
--rw-r--r--   0        0        0      294 2024-04-04 03:26:11.310087 glitter_sdk_lite-0.0.1/glitter_sdk/util/remove_none.py
--rw-r--r--   0        0        0      133 2024-04-04 03:26:11.310257 glitter_sdk_lite-0.0.1/glitter_sdk/util/url.py
--rw-r--r--   0        0        0      488 2024-04-07 10:07:11.443485 glitter_sdk_lite-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 glitter_sdk_lite-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-04 03:26:11.278873 glitter_sdk_lite-0.0.2/LICENSE
+-rw-r--r--   0        0        0       95 2024-04-04 03:26:11.279109 glitter_sdk_lite-0.0.2/README.md
+-rw-r--r--   0        0        0       13 2024-04-04 03:26:11.280537 glitter_sdk_lite-0.0.2/glitter_sdk_lite/.gitignore
+-rw-r--r--   0        0        0      163 2024-04-04 03:26:11.280655 glitter_sdk_lite-0.0.2/glitter_sdk_lite/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 03:26:11.280763 glitter_sdk_lite-0.0.2/glitter_sdk_lite/client/__init__.py
+-rw-r--r--   0        0        0       83 2024-04-07 07:10:39.384840 glitter_sdk_lite-0.0.2/glitter_sdk_lite/client/lcd/__init__.py
+-rw-r--r--   0        0        0     5010 2024-04-13 04:18:25.405114 glitter_sdk_lite-0.0.2/glitter_sdk_lite/client/lcd/db.py
+-rw-r--r--   0        0        0      431 2024-04-07 04:00:39.693586 glitter_sdk_lite-0.0.2/glitter_sdk_lite/client/lcd/lcdclient.py
+-rw-r--r--   0        0        0      150 2024-04-07 01:49:25.738295 glitter_sdk_lite-0.0.2/glitter_sdk_lite/core/__init__.py
+-rw-r--r--   0        0        0     5009 2023-09-03 07:54:13.159000 glitter_sdk_lite-0.0.2/glitter_sdk_lite/core/bech32.py
+-rw-r--r--   0        0        0      825 2024-04-13 04:18:25.369839 glitter_sdk_lite-0.0.2/glitter_sdk_lite/core/msg.py
+-rw-r--r--   0        0        0      188 2023-09-03 07:54:13.265000 glitter_sdk_lite-0.0.2/glitter_sdk_lite/core/msgs/__init__.py
+-rw-r--r--   0        0        0      818 2024-04-13 04:18:25.379958 glitter_sdk_lite-0.0.2/glitter_sdk_lite/core/msgs/argument.py
+-rw-r--r--   0        0        0     1932 2024-04-13 04:18:25.398056 glitter_sdk_lite-0.0.2/glitter_sdk_lite/core/msgs/arguments.py
+-rw-r--r--   0        0        0     2998 2024-04-13 04:18:25.424257 glitter_sdk_lite-0.0.2/glitter_sdk_lite/core/msgs/msgs.py
+-rw-r--r--   0        0        0      968 2024-04-04 03:26:11.302295 glitter_sdk_lite-0.0.2/glitter_sdk_lite/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-04 03:26:11.303345 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/__init__.py
+-rw-r--r--   0        0        0     1678 2024-04-04 03:26:11.303468 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/base.py
+-rw-r--r--   0        0        0      878 2024-04-04 03:26:11.303687 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/constants/CLIENT.py
+-rw-r--r--   0        0        0      679 2024-04-04 03:26:11.303804 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/constants/COMMAND.py
+-rw-r--r--   0        0        0     1927 2024-04-04 03:26:11.303921 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/constants/CR.py
+-rw-r--r--   0        0        0    12296 2024-04-04 03:26:11.304090 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/constants/ER.py
+-rw-r--r--   0        0        0      370 2024-04-04 03:26:11.304209 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/constants/FIELD_TYPE.py
+-rw-r--r--   0        0        0      214 2024-04-04 03:26:11.304328 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/constants/FLAG.py
+-rw-r--r--   0        0        0      333 2024-04-04 03:26:11.304450 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/constants/SERVER_STATUS.py
+-rw-r--r--   0        0        0        0 2024-04-04 03:26:11.304508 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/constants/__init__.py
+-rw-r--r--   0        0        0     3268 2024-04-13 04:18:25.361019 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/contract.py
+-rw-r--r--   0        0        0      199 2024-04-04 03:26:11.304806 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/converter.py
+-rw-r--r--   0        0        0      211 2024-04-04 03:26:11.308892 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/hash.py
+-rw-r--r--   0        0        0      401 2024-04-04 03:26:11.309013 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/highlight.py
+-rw-r--r--   0        0        0     1701 2024-04-13 04:18:25.393401 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/json.py
+-rw-r--r--   0        0        0     1050 2024-04-13 04:18:25.408796 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/parse_authorization.py
+-rw-r--r--   0        0        0     2575 2024-04-13 04:18:25.384325 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/parse_content.py
+-rw-r--r--   0        0        0     3947 2024-04-13 04:18:25.375486 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/parse_msg.py
+-rw-r--r--   0        0        0      737 2024-04-13 04:18:25.354258 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/parse_proto.py
+-rw-r--r--   0        0        0     2950 2024-04-04 03:26:11.309779 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/parse_query_str.py
+-rw-r--r--   0        0        0    14744 2024-04-13 04:18:25.421172 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/parse_sql.py
+-rw-r--r--   0        0        0      294 2024-04-04 03:26:11.310087 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/remove_none.py
+-rw-r--r--   0        0        0      133 2024-04-04 03:26:11.310257 glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/url.py
+-rw-r--r--   0        0        0      493 2024-04-13 04:18:45.199567 glitter_sdk_lite-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      865 1970-01-01 00:00:00.000000 glitter_sdk_lite-0.0.2/PKG-INFO
```

### Comparing `glitter_sdk_lite-0.0.1/LICENSE` & `glitter_sdk_lite-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/client/lcd/db.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/client/lcd/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import requests
 import base64
-from glitter_sdk.exceptions import *
-from glitter_sdk.util.url import urljoin
+from glitter_sdk_lite.exceptions import *
+from glitter_sdk_lite.util.url import urljoin
 from glitter_proto.blockved.glitterchain.index import *
-from glitter_sdk.util.parse_sql import to_glitter_arguments
+from glitter_sdk_lite.util.parse_sql import to_glitter_arguments
 
 __all__ = ["DB"]
 
 
 class DB:
     def __init__(self, url):
         self.url = url
```

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/core/bech32.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/core/bech32.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/core/msg.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/core/msg.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 from __future__ import annotations
 
 from betterproto.lib.google.protobuf import Any as Any_pb
 
-from glitter_sdk.util.base import BaseTerraData
+from glitter_sdk_lite.util.base import BaseTerraData
 
 
 class Msg(BaseTerraData):
     def to_proto(self):
         raise NotImplementedError
 
     def pack_any(self) -> Any_pb:
         return Any_pb(type_url=self.type_url, value=bytes(self.to_proto()))
 
     @staticmethod
     def from_data(data: dict) -> Msg:
-        from glitter_sdk.util.parse_msg import parse_msg
+        from glitter_sdk_lite.util.parse_msg import parse_msg
 
         return parse_msg(data)
 
     @staticmethod
     def from_proto(proto: any) -> Msg:
-        from glitter_sdk.util.parse_msg import parse_proto
+        from glitter_sdk_lite.util.parse_msg import parse_proto
 
         return parse_proto(proto)
 
     @staticmethod
     def unpack_any(any_pb: Any_pb) -> Msg:
-        from glitter_sdk.util.parse_msg import parse_unpack_any
+        from glitter_sdk_lite.util.parse_msg import parse_unpack_any
 
         return parse_unpack_any(any_pb)
```

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/core/msgs/argument.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/core/msgs/argument.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import attr
 from glitter_proto.blockved.glitterchain.index import Argument as Argument_pb
 from glitter_proto.blockved.glitterchain.index import ArgumentVarType as ArgumentVarType_pb
-from glitter_sdk.util.json import JSONSerializable
+from glitter_sdk_lite.util.json import JSONSerializable
 
 
 
 @attr.s(frozen=True)
 class Argument(JSONSerializable):
     """Represents a (type, value) pairing
     """
```

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/core/msgs/arguments.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/core/msgs/arguments.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import copy
 from typing import Any, Callable, Dict, Iterable, Iterator, List, Optional, Union
 
 from glitter_proto.blockved.glitterchain.index import Argument as Argument_pb
 
-from glitter_sdk.util.json import JSONSerializable
+from glitter_sdk_lite.util.json import JSONSerializable
 
 from .argument import Argument
 
 
 class Arguments():
     """Represents an unordered collection of :class:`Argument` objects
```

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/core/msgs/msgs.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/core/msgs/msgs.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 from betterproto.lib.google.protobuf import Any as Any_pb
 from glitter_proto.cosmos.bank.v1beta1 import Input as Input_pb
 from glitter_proto.cosmos.bank.v1beta1 import MsgMultiSend as MsgMultiSend_pb
 from glitter_proto.blockved.glitterchain.index import SqlExecRequest as SQLExecRequest_pb
 from glitter_proto.blockved.glitterchain.index import SqlGrantRequest as SQLGrantRequest_pb
 from glitter_proto.cosmos.bank.v1beta1 import Output as Output_pb
 
-from glitter_sdk.core import AccAddress
-from glitter_sdk.core.msg import Msg
-from glitter_sdk.util.json import JSONSerializable
+from glitter_sdk_lite.core import AccAddress
+from glitter_sdk_lite.core.msg import Msg
+from glitter_sdk_lite.util.json import JSONSerializable
 from .arguments import Arguments
 
 __all__ = ["SQLExecRequest", "SQLGrantRequest"]
 
 import attr
```

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/exceptions.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/exceptions.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/util/base.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/base.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/util/constants/CLIENT.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/constants/CLIENT.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/util/constants/COMMAND.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/constants/COMMAND.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/util/constants/CR.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/constants/CR.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/util/constants/ER.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/constants/ER.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/util/contract.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/contract.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Useful contract-related functions."""
 
 import base64
 from typing import Dict, List, Union
 
-from glitter_sdk.core import AccAddress
-from glitter_sdk.core.auth import TxInfo
-from glitter_sdk.core.broadcast import BlockTxBroadcastResult
+from glitter_sdk_lite.core import AccAddress
+from glitter_sdk_lite.core.auth import TxInfo
+from glitter_sdk_lite.core.broadcast import BlockTxBroadcastResult
 
 __all__ = [
     "read_file_as_b64",
     "get_code_id",
     "get_contract_address",
     "get_contract_events",
 ]
```

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/util/json.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import copy
 import json
 from abc import ABC
 from datetime import datetime
 from typing import Any
 
-from glitter_sdk.util.converter import to_isoformat
+from glitter_sdk_lite.util.converter import to_isoformat
 
 
 def to_data(x: Any) -> Any:
     if hasattr(x, "to_data"):
         return x.to_data()
     if isinstance(x, int):
         return str(x)
```

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/util/parse_authorization.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/parse_authorization.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
     GenericAuthorization as GenericAuthorization_pb,
 )
 from glitter_proto.cosmos.bank.v1beta1 import SendAuthorization as SendAuthorization_pb
 from glitter_proto.cosmos.staking.v1beta1 import (
     StakeAuthorization as StakeAuthorization_pb,
 )
 
-from glitter_sdk.core.authz import (
+from glitter_sdk_lite.core.authz import (
     GenericAuthorization,
     SendAuthorization,
     StakeAuthorization,
 )
 
 from .base import (
     create_demux,
```

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/util/parse_content.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/parse_content.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from glitter_proto.cosmos.upgrade.v1beta1 import (
     SoftwareUpgradeProposal as SoftwareUpgradeProposal_pb,
 )
 from glitter_proto.ibc.core.client.v1 import (
     ClientUpdateProposal as ClientUpdateProposal_pb,
 )
 
-from glitter_sdk.core.distribution.proposals import CommunityPoolSpendProposal
-from glitter_sdk.core.gov.proposals import TextProposal
-from glitter_sdk.core.ibc.proposals import ClientUpdateProposal
-from glitter_sdk.core.params.proposals import ParameterChangeProposal
-from glitter_sdk.core.upgrade import (
+from glitter_sdk_lite.core.distribution.proposals import CommunityPoolSpendProposal
+from glitter_sdk_lite.core.gov.proposals import TextProposal
+from glitter_sdk_lite.core.ibc.proposals import ClientUpdateProposal
+from glitter_sdk_lite.core.params.proposals import ParameterChangeProposal
+from glitter_sdk_lite.core.upgrade import (
     CancelSoftwareUpgradeProposal,
     SoftwareUpgradeProposal,
 )
 
 from .base import create_demux, create_demux_proto, create_demux_unpack_any
 
 Content = Union[
```

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/util/parse_msg.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/parse_msg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # core msgs
-from glitter_sdk.core.auth import(
+from glitter_sdk_lite.core.auth import(
     MsgDonateAllVestingTokens,
     MsgCreatePeriodicVestingAccount,
     MsgCreateVestingAccount
 )
-from glitter_sdk.core.authz import (
+from glitter_sdk_lite.core.authz import (
     MsgExecAuthorized,
     MsgGrantAuthorization,
     MsgRevokeAuthorization,
 )
-from glitter_sdk.core.bank import MsgMultiSend, MsgSend
-from glitter_sdk.core.crisis import MsgVerifyInvariant
-from glitter_sdk.core.distribution import (
+from glitter_sdk_lite.core.bank import MsgMultiSend, MsgSend
+from glitter_sdk_lite.core.crisis import MsgVerifyInvariant
+from glitter_sdk_lite.core.distribution import (
     MsgFundCommunityPool,
     MsgSetWithdrawAddress,
     MsgWithdrawDelegatorReward,
     MsgWithdrawValidatorCommission,
 )
-from glitter_sdk.core.feegrant import MsgGrantAllowance, MsgRevokeAllowance
-from glitter_sdk.core.gov.msgs import MsgDeposit, MsgSubmitProposal, MsgVote
-from glitter_sdk.core.ibc.msgs import (
+from glitter_sdk_lite.core.feegrant import MsgGrantAllowance, MsgRevokeAllowance
+from glitter_sdk_lite.core.gov.msgs import MsgDeposit, MsgSubmitProposal, MsgVote
+from glitter_sdk_lite.core.ibc.msgs import (
     MsgAcknowledgement,
     MsgChannelCloseConfirm,
     MsgChannelCloseInit,
     MsgChannelOpenAck,
     MsgChannelOpenConfirm,
     MsgChannelOpenInit,
     MsgChannelOpenTry,
@@ -34,24 +34,24 @@
     MsgCreateClient,
     MsgRecvPacket,
     MsgSubmitMisbehaviour,
     MsgTimeout,
     MsgUpdateClient,
     MsgUpgradeClient,
 )
-from glitter_sdk.core.ibc_transfer import MsgTransfer
-from glitter_sdk.core.slashing import MsgUnjail
-from glitter_sdk.core.staking import (
+from glitter_sdk_lite.core.ibc_transfer import MsgTransfer
+from glitter_sdk_lite.core.slashing import MsgUnjail
+from glitter_sdk_lite.core.staking import (
     MsgBeginRedelegate,
     MsgCreateValidator,
     MsgDelegate,
     MsgEditValidator,
     MsgUndelegate,
 )
-from glitter_sdk.core.wasm import (
+from glitter_sdk_lite.core.wasm import (
     MsgClearAdmin,
     MsgExecuteContract,
     MsgInstantiateContract,
     MsgMigrateContract,
     MsgStoreCode,
     MsgUpdateAdmin,
 )
```

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/util/parse_proto.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/parse_proto.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from glitter_sdk.core.authz import GenericAuthorization, SendAuthorization,StakeAuthorization
+from glitter_sdk_lite.core.authz import GenericAuthorization, SendAuthorization,StakeAuthorization
 
 from .base import (
     create_demux,
     create_demux_amino,
     create_demux_proto,
     create_demux_unpack_any,
 )
```

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/util/parse_query_str.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/parse_query_str.py`

 * *Files identical despite different names*

### Comparing `glitter_sdk_lite-0.0.1/glitter_sdk/util/parse_sql.py` & `glitter_sdk_lite-0.0.2/glitter_sdk_lite/util/parse_sql.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import datetime
 import re
 import time
 import base64
 from decimal import Decimal
-from glitter_sdk.core.msgs import Arguments
+from glitter_sdk_lite.core.msgs import Arguments
 from glitter_proto.blockved.glitterchain.index import Argument as Argument_pb
 from glitter_proto.blockved.glitterchain.index import *
-from glitter_sdk.exceptions import SQLError, ParamError
-from glitter_sdk.util.constants import FIELD_TYPE
+from glitter_sdk_lite.exceptions import SQLError, ParamError
+from glitter_sdk_lite.util.constants import FIELD_TYPE
 
 
 def to_glitter_arguments(args: List) -> Arguments:
     """
     Convert a list of Python arguments to Glitter Arguments protobuf.
 
     Args:
```

### Comparing `glitter_sdk_lite-0.0.1/PKG-INFO` & `glitter_sdk_lite-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glitter-sdk-lite
-Version: 0.0.1
+Version: 0.0.2
 Summary: glitter-sdk-lite is a lite SDK for accessing the glitter network.
 Author: Glitter Protocol
 Author-email: ted@glitterprotocol.io
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

