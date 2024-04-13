# Comparing `tmp/pykrotik-0.0.5.tar.gz` & `tmp/pykrotik-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykrotik-0.0.5.tar", last modified: Fri Apr 12 06:19:52 2024, max compression
+gzip compressed data, was "pykrotik-0.0.6.tar", last modified: Sat Apr 13 06:26:32 2024, max compression
```

## Comparing `pykrotik-0.0.5.tar` & `pykrotik-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:19:52.657741 pykrotik-0.0.5/
--rw-r--r--   0 root         (0) root         (0)      254 2024-04-12 06:19:52.657741 pykrotik-0.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      792 2024-04-11 18:11:37.000000 pykrotik-0.0.5/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:19:52.657741 pykrotik-0.0.5/pykrotik/
--rw-r--r--   0 root         (0) root         (0)    37929 2024-04-12 06:10:17.000000 pykrotik-0.0.5/pykrotik/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:19:52.657741 pykrotik-0.0.5/pykrotik.egg-info/
--rw-r--r--   0 root         (0) root         (0)      254 2024-04-12 06:19:52.000000 pykrotik-0.0.5/pykrotik.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      232 2024-04-12 06:19:52.000000 pykrotik-0.0.5/pykrotik.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 06:19:52.000000 pykrotik-0.0.5/pykrotik.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2024-04-12 06:19:52.000000 pykrotik-0.0.5/pykrotik.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2024-04-12 06:19:52.000000 pykrotik-0.0.5/pykrotik.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      335 2024-04-12 06:18:12.000000 pykrotik-0.0.5/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 06:19:52.657741 pykrotik-0.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 18:11:37.000000 pykrotik-0.0.5/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 06:19:52.657741 pykrotik-0.0.5/tests/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-12 06:16:47.000000 pykrotik-0.0.5/tests/test_init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 06:26:32.307471 pykrotik-0.0.6/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-13 06:26:32.307471 pykrotik-0.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      792 2024-04-11 18:11:37.000000 pykrotik-0.0.6/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 06:26:32.297471 pykrotik-0.0.6/pykrotik/
+-rw-r--r--   0 root         (0) root         (0)    38461 2024-04-13 06:25:29.000000 pykrotik-0.0.6/pykrotik/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 06:26:32.297471 pykrotik-0.0.6/pykrotik.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      254 2024-04-13 06:26:32.000000 pykrotik-0.0.6/pykrotik.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      232 2024-04-13 06:26:32.000000 pykrotik-0.0.6/pykrotik.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-13 06:26:32.000000 pykrotik-0.0.6/pykrotik.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2024-04-13 06:26:32.000000 pykrotik-0.0.6/pykrotik.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2024-04-13 06:26:32.000000 pykrotik-0.0.6/pykrotik.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      335 2024-04-13 06:26:06.000000 pykrotik-0.0.6/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-13 06:26:32.307471 pykrotik-0.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-11 18:11:37.000000 pykrotik-0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-13 06:26:32.297471 pykrotik-0.0.6/tests/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-12 06:16:47.000000 pykrotik-0.0.6/tests/test_init.py
```

### Comparing `pykrotik-0.0.5/README.md` & `pykrotik-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pykrotik-0.0.5/pykrotik/__init__.py` & `pykrotik-0.0.6/pykrotik/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     id: str | None = pydantic.Field(default=None, alias=str(".id"))
     # the list the ip address belongs to
     list: str
     # the timeout for the address list record
     timeout: int | None = pydantic.Field(default=None)
 
 
-class IpFirewallNatProtocol(str, enum.Enum):
+class IpFirewallProtocol(str, enum.Enum):
     """
     List of protocols selectable when defining ip firewall nat rules
     """
 
     Dccp = "dccp"
     Ddp = "ddp"
     Egp = "egp"
@@ -107,47 +107,47 @@
     Definition of an ip firewall nat
     """
 
     # the action the firewall filter will take
     action: IpFirewallNatAction
     # action-specific address list field
     address_list: str | None = pydantic.Field(default=None, alias=str("address-list"))
-    # protocl-specific field representing a source/destination port
+    # protocol-specific field representing a source/destination port
     any_port: int | None = pydantic.Field(default=None, alias=str("any-port"))
     # the chain the firewall filter belongs to
     chain: str
     # comment attached to the ip firewall filter
     comment: str = pydantic.Field(default="")
     # flag that dictates whether an ip firewall filter is active
     disabled: bool = pydantic.Field(default=False)
     # dst address for the firewall fitler
     dst_address: str | None = pydantic.Field(default=None, alias=str("dst-address"))
     # dst address list for the firewall fitler
     dst_address_list: str | None = pydantic.Field(
         default=None, alias=str("dst-address-list")
     )
-    # protocl-specific field representing a destination port
+    # protocol-specific field representing a destination port
     dst_port: int | None = pydantic.Field(default=None, alias=str("dst-port"))
     # the id for an ip firewall filter (NOTE: prefixed with '*')
     id: str | None = pydantic.Field(default=None, alias=str(".id"))
     # action-specific jump target
     jump_target: str | None = pydantic.Field(default=None, alias=str("jump-target"))
     # flag that dictates whether filter is logged
     log: bool = pydantic.Field(default=False)
     # log prefix for logged filter
     log_prefix: str = pydantic.Field(default="", alias=str("log-prefix"))
     # protocol for the nat filter
-    protocol: IpFirewallNatProtocol | None = pydantic.Field(default=None)
+    protocol: IpFirewallProtocol | None = pydantic.Field(default=None)
     # src address for the firewall fitler
     src_address: str | None = pydantic.Field(default=None, alias=str("src-address"))
     # src address list for the firewall fitler
     src_address_list: str | None = pydantic.Field(
         default=None, alias=str("src-address-list")
     )
-    # protocl-specific field representing a source port
+    # protocol-specific field representing a source port
     src_port: int | None = pydantic.Field(default=None, alias=str("src-port"))
     # action-specific field representing a target address
     to_addresses: str | None = pydantic.Field(default=None, alias=str("to-addresses"))
     # action-specific field representing a target port
     to_ports: str | None = pydantic.Field(default=None, alias=str("to-ports"))
 
 
@@ -174,34 +174,42 @@
     Definition of an ip firewall filter
     """
 
     # action to be performed by this firewall filter
     action: IpFirewallFilterAction
     # action-specific address list field
     address_list: str | None = pydantic.Field(default=None, alias=str("address-list"))
+    # protocol-specific field representing a source/destination port
+    any_port: int | None = pydantic.Field(default=None, alias=str("any-port"))
     # the chain the firewall filter belongs to
     chain: str
     # comment attached to the ip firewall filter
     comment: str = pydantic.Field(default="")
     # flag that dictates whether an ip firewall filter is active
     disabled: bool = pydantic.Field(default=False)
     # dst address for the firewall fitler
     dst_address: str | None = pydantic.Field(default=None, alias=str("dst-address"))
     # dst address list for the firewall fitler
     dst_address_list: str | None = pydantic.Field(
         default=None, alias=str("dst-address-list")
     )
+    # protocol-specific field representing a destination port
+    dst_port: int | None = pydantic.Field(default=None, alias=str("dst-port"))
     # the id for an ip firewall filter (NOTE: prefixed with '*')
     id: str | None = pydantic.Field(default=None, alias=str(".id"))
     # action-specific jump target
     jump_target: str | None = pydantic.Field(default=None, alias=str("jump-target"))
     # flag that dictates whether filter is logged
     log: bool = pydantic.Field(default=False)
     # log prefix for logged filter
     log_prefix: str = pydantic.Field(default="", alias=str("log-prefix"))
+    # protocol for the firewall filter
+    protocol: IpFirewallProtocol | None = pydantic.Field(default=None)
+    # protocol-specific field representing a source port
+    src_port: int | None = pydantic.Field(default=None, alias=str("src-port"))
     # src address for the firewall fitler
     src_address: str | None = pydantic.Field(default=None, alias=str("src-address"))
     # src address list for the firewall fitler
     src_address_list: str | None = pydantic.Field(
         default=None, alias=str("src-address-list")
     )
```

### Comparing `pykrotik-0.0.5/tests/test_init.py` & `pykrotik-0.0.6/tests/test_init.py`

 * *Files identical despite different names*

