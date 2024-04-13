# Comparing `tmp/evmchains-0.0.5.tar.gz` & `tmp/evmchains-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evmchains-0.0.5.tar", last modified: Tue Apr  9 22:52:33 2024, max compression
+gzip compressed data, was "evmchains-0.0.6.tar", last modified: Sat Apr 13 00:27:28 2024, max compression
```

## Comparing `evmchains-0.0.5.tar` & `evmchains-0.0.6.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:33.210523 evmchains-0.0.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:33.206523 evmchains-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:33.206523 evmchains-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-09 22:52:15.000000 evmchains-0.0.5/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-09 22:52:15.000000 evmchains-0.0.5/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-09 22:52:15.000000 evmchains-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-09 22:52:15.000000 evmchains-0.0.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-09 22:52:15.000000 evmchains-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-04-09 22:52:33.210523 evmchains-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-09 22:52:15.000000 evmchains-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:33.206523 evmchains-0.0.5/evmchains/
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-09 22:52:15.000000 evmchains-0.0.5/evmchains/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-09 22:52:33.000000 evmchains-0.0.5/evmchains/_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)    30014 2024-04-09 22:52:15.000000 evmchains-0.0.5/evmchains/chains.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:15.000000 evmchains-0.0.5/evmchains/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-09 22:52:15.000000 evmchains-0.0.5/evmchains/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:33.210523 evmchains-0.0.5/evmchains.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-04-09 22:52:33.000000 evmchains-0.0.5/evmchains.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-09 22:52:33.000000 evmchains-0.0.5/evmchains.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 22:52:33.000000 evmchains-0.0.5/evmchains.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-09 22:52:33.000000 evmchains-0.0.5/evmchains.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-09 22:52:33.000000 evmchains-0.0.5/evmchains.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-09 22:52:15.000000 evmchains-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:33.210523 evmchains-0.0.5/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     4379 2024-04-09 22:52:15.000000 evmchains-0.0.5/scripts/update.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-09 22:52:33.210523 evmchains-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-09 22:52:15.000000 evmchains-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 22:52:33.210523 evmchains-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-09 22:52:15.000000 evmchains-0.0.5/tests/test_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:28.871504 evmchains-0.0.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:28.863504 evmchains-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:28.867504 evmchains-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-04-13 00:27:09.000000 evmchains-0.0.6/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-13 00:27:09.000000 evmchains-0.0.6/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-13 00:27:09.000000 evmchains-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-13 00:27:09.000000 evmchains-0.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-04-13 00:27:09.000000 evmchains-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-04-13 00:27:28.871504 evmchains-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1411 2024-04-13 00:27:09.000000 evmchains-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:28.867504 evmchains-0.0.6/evmchains/
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-13 00:27:09.000000 evmchains-0.0.6/evmchains/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-13 00:27:28.000000 evmchains-0.0.6/evmchains/_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33001 2024-04-13 00:27:09.000000 evmchains-0.0.6/evmchains/chains.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:09.000000 evmchains-0.0.6/evmchains/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-13 00:27:09.000000 evmchains-0.0.6/evmchains/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:28.871504 evmchains-0.0.6/evmchains.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15772 2024-04-13 00:27:28.000000 evmchains-0.0.6/evmchains.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-13 00:27:28.000000 evmchains-0.0.6/evmchains.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 00:27:28.000000 evmchains-0.0.6/evmchains.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-13 00:27:28.000000 evmchains-0.0.6/evmchains.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 00:27:28.000000 evmchains-0.0.6/evmchains.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-13 00:27:09.000000 evmchains-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:28.867504 evmchains-0.0.6/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4453 2024-04-13 00:27:09.000000 evmchains-0.0.6/scripts/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-04-13 00:27:28.871504 evmchains-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-13 00:27:09.000000 evmchains-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:27:28.867504 evmchains-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-13 00:27:09.000000 evmchains-0.0.6/tests/test_func.py
```

### Comparing `evmchains-0.0.5/.github/workflows/release.yaml` & `evmchains-0.0.6/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.5/.github/workflows/test.yaml` & `evmchains-0.0.6/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.5/.gitignore` & `evmchains-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.5/CONTRIBUTING.md` & `evmchains-0.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.5/LICENSE` & `evmchains-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.5/PKG-INFO` & `evmchains-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evmchains
-Version: 0.0.5
+Version: 0.0.6
 Summary: Packaged metadata on Ethereum Virtual Machine (EVM) chains
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `evmchains-0.0.5/README.md` & `evmchains-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.5/evmchains/__init__.py` & `evmchains-0.0.6/evmchains/__init__.py`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.5/evmchains/chains.py` & `evmchains-0.0.6/evmchains/chains.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# This file is auto-generated by scripts/update_rpc.py
-# 2024-03-08 22:05:08.915228
+# This file is auto-generated by scripts/update.py
+# 2024-04-09 14:08:35.326760
 # Do not edit this file directly.
 from typing import Any, Dict
 
 PUBLIC_CHAIN_META: Dict[str, Dict[str, Dict[str, Any]]] = {
     "arbitrum": {
         "mainnet": {
             "chain": "ETH",
@@ -276,15 +276,15 @@
             "name": "Blast Sepolia Testnet",
             "nativeCurrency": {
                 "decimals": 18,
                 "name": "Sepolia Ether",
                 "symbol": "ETH",
             },
             "networkId": 168587773,
-            "rpc": ["https://sepolia.blast.io"],
+            "rpc": ["https://sepolia.blast.io", "https://blast-sepolia.drpc.org"],
             "shortName": "blastsepolia",
             "slip44": None,
         },
     },
     "bsc": {
         "mainnet": {
             "chain": "BSC",
@@ -406,14 +406,15 @@
                 "https://mainnet.gateway.tenderly.co",
                 "https://rpc.flashbots.net",
                 "https://rpc.flashbots.net/fast",
                 "https://rpc.mevblocker.io",
                 "https://rpc.mevblocker.io/fast",
                 "https://rpc.mevblocker.io/noreverts",
                 "https://rpc.mevblocker.io/fullprivacy",
+                "https://eth.drpc.org",
             ],
             "shortName": "eth",
             "slip44": 60,
         },
         "goerli": {
             "chain": "ETH",
             "chainId": 5,
@@ -484,14 +485,15 @@
                 "https://rpc.sepolia.org",
                 "https://rpc2.sepolia.org",
                 "https://rpc-sepolia.rockx.com",
                 "https://rpc.sepolia.ethpandaops.io",
                 "https://sepolia.infura.io/v3/${INFURA_API_KEY}",
                 "https://sepolia.gateway.tenderly.co",
                 "https://ethereum-sepolia-rpc.publicnode.com",
+                "https://sepolia.drpc.org",
             ],
             "shortName": "sep",
             "slip44": 1,
         },
     },
     "fantom": {
         "mainnet": {
@@ -515,15 +517,19 @@
             "faucets": [],
             "features": None,
             "icon": "fantom",
             "infoURL": "https://fantom.foundation",
             "name": "Fantom Opera",
             "nativeCurrency": {"decimals": 18, "name": "Fantom", "symbol": "FTM"},
             "networkId": 250,
-            "rpc": ["https://rpc.ftm.tools", "https://fantom-rpc.publicnode.com"],
+            "rpc": [
+                "https://rpc.ftm.tools",
+                "https://fantom-rpc.publicnode.com",
+                "https://fantom.drpc.org",
+            ],
             "shortName": "ftm",
             "slip44": None,
         },
         "testnet": {
             "chain": "FTM",
             "chainId": 4002,
             "ens": None,
@@ -541,14 +547,15 @@
             "infoURL": "https://docs.fantom.foundation/quick-start/short-guide#fantom-testnet",
             "name": "Fantom Testnet",
             "nativeCurrency": {"decimals": 18, "name": "Fantom", "symbol": "FTM"},
             "networkId": 4002,
             "rpc": [
                 "https://rpc.testnet.fantom.network",
                 "https://fantom-testnet-rpc.publicnode.com",
+                "https://fantom-testnet.drpc.org",
             ],
             "shortName": "tftm",
             "slip44": 1,
         },
     },
     "gnosis": {
         "mainnet": {
@@ -632,14 +639,15 @@
             "name": "OP Mainnet",
             "nativeCurrency": {"decimals": 18, "name": "Ether", "symbol": "ETH"},
             "networkId": 10,
             "rpc": [
                 "https://mainnet.optimism.io",
                 "https://optimism-rpc.publicnode.com",
                 "https://optimism.gateway.tenderly.co",
+                "https://optimism.drpc.org",
             ],
             "shortName": "oeth",
             "slip44": None,
         },
         "goerli": {
             "chain": "ETH",
             "chainId": 420,
@@ -659,14 +667,15 @@
             "name": "Optimism Goerli Testnet",
             "nativeCurrency": {"decimals": 18, "name": "Goerli Ether", "symbol": "ETH"},
             "networkId": 420,
             "rpc": [
                 "https://goerli.optimism.io",
                 "https://optimism-goerli-rpc.publicnode.com",
                 "https://optimism-goerli.gateway.tenderly.co",
+                "https://optimism-testnet.drpc.org",
             ],
             "shortName": "ogor",
             "slip44": 1,
         },
         "sepolia": {
             "chain": "ETH",
             "chainId": 11155420,
@@ -686,15 +695,15 @@
             "name": "OP Sepolia Testnet",
             "nativeCurrency": {
                 "decimals": 18,
                 "name": "Sepolia Ether",
                 "symbol": "ETH",
             },
             "networkId": 11155420,
-            "rpc": ["https://sepolia.optimism.io"],
+            "rpc": ["https://sepolia.optimism.io", "https://optimism-sepolia.drpc.org"],
             "shortName": "opsep",
             "slip44": 1,
         },
     },
     "oort": {
         "mainnet": {
             "chain": "Oort Mainnet",
@@ -773,14 +782,15 @@
                 "https://rpc-mainnet.matic.network",
                 "https://matic-mainnet.chainstacklabs.com",
                 "https://rpc-mainnet.maticvigil.com",
                 "https://rpc-mainnet.matic.quiknode.pro",
                 "https://matic-mainnet-full-rpc.bwarelabs.com",
                 "https://polygon-bor-rpc.publicnode.com",
                 "https://polygon.gateway.tenderly.co",
+                "https://polygon.drpc.org",
             ],
             "shortName": "matic",
             "slip44": 966,
         },
         "mumbai": {
             "chain": "Polygon",
             "chainId": 80001,
@@ -824,15 +834,15 @@
             "faucets": [],
             "features": None,
             "icon": "zkevm",
             "infoURL": "https://polygon.technology/polygon-zkevm",
             "name": "Polygon zkEVM",
             "nativeCurrency": {"decimals": 18, "name": "Ether", "symbol": "ETH"},
             "networkId": 1101,
-            "rpc": ["https://zkevm-rpc.com"],
+            "rpc": ["https://zkevm-rpc.com", "https://polygon-zkevm.drpc.org"],
             "shortName": "zkevm",
             "slip44": None,
         },
         "testnet": {
             "chain": "Polygon",
             "chainId": 1442,
             "ens": None,
@@ -846,13 +856,88 @@
             "faucets": [],
             "features": None,
             "icon": None,
             "infoURL": "https://polygon.technology/solutions/polygon-zkevm/",
             "name": "Polygon zkEVM Testnet",
             "nativeCurrency": {"decimals": 18, "name": "Ether", "symbol": "ETH"},
             "networkId": 1442,
-            "rpc": ["https://rpc.public.zkevm-test.net"],
+            "rpc": [
+                "https://rpc.public.zkevm-test.net",
+                "https://polygon-zkevm-testnet.drpc.org",
+            ],
             "shortName": "testnet-zkEVM-mango",
             "slip44": 1,
         },
     },
+    "linea": {
+        "mainnet": {
+            "chain": "ETH",
+            "chainId": 59144,
+            "ens": None,
+            "explorers": [
+                {
+                    "icon": "linea",
+                    "name": "Etherscan",
+                    "standard": "EIP3091",
+                    "url": "https://lineascan.build",
+                },
+                {
+                    "icon": "linea",
+                    "name": "Blockscout",
+                    "standard": "EIP3091",
+                    "url": "https://explorer.linea.build",
+                },
+                {
+                    "icon": "linea",
+                    "name": "L2scan",
+                    "standard": "EIP3091",
+                    "url": "https://linea.l2scan.co",
+                },
+            ],
+            "faucets": [],
+            "features": None,
+            "icon": "linea",
+            "infoURL": "https://linea.build",
+            "name": "Linea",
+            "nativeCurrency": {"decimals": 18, "name": "Linea Ether", "symbol": "ETH"},
+            "networkId": 59144,
+            "rpc": [
+                "https://rpc.linea.build",
+                "https://linea-mainnet.infura.io/v3/${INFURA_API_KEY}",
+            ],
+            "shortName": "linea",
+            "slip44": None,
+        },
+        "sepolia": {
+            "chain": "ETH",
+            "chainId": 59141,
+            "ens": None,
+            "explorers": [
+                {
+                    "icon": "linea",
+                    "name": "Etherscan",
+                    "standard": "EIP3091",
+                    "url": "https://sepolia.lineascan.build",
+                },
+                {
+                    "icon": "linea",
+                    "name": "Blockscout",
+                    "standard": "EIP3091",
+                    "url": "https://explorer.sepolia.linea.build",
+                },
+            ],
+            "faucets": [],
+            "features": None,
+            "icon": "linea",
+            "infoURL": "https://linea.build",
+            "name": "Linea Sepolia",
+            "nativeCurrency": {"decimals": 18, "name": "Linea Ether", "symbol": "ETH"},
+            "networkId": 59141,
+            "rpc": [
+                "https://rpc.sepolia.linea.build",
+                "https://linea-sepolia.infura.io/v3/${INFURA_API_KEY}",
+            ],
+            "shortName": "linea-sepolia",
+            "slip44": 1,
+        },
+    },
 }
```

### Comparing `evmchains-0.0.5/evmchains.egg-info/PKG-INFO` & `evmchains-0.0.6/evmchains.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evmchains
-Version: 0.0.5
+Version: 0.0.6
 Summary: Packaged metadata on Ethereum Virtual Machine (EVM) chains
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `evmchains-0.0.5/pyproject.toml` & `evmchains-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `evmchains-0.0.5/scripts/update.py` & `evmchains-0.0.6/scripts/update.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,18 @@
         "mainnet": 137,
         "mumbai": 80001,
     },
     "polygon-zkevm": {
         "mainnet": 1101,
         "testnet": 1442,
     },
+    "linea": {
+        "mainnet": 59144,
+        "sepolia": 59141,
+    },
 }
 
 pp = PrettyPrinter(indent=4)
 logger = logging.getLogger("update")
 logger.setLevel(logging.DEBUG)
```

### Comparing `evmchains-0.0.5/tests/test_func.py` & `evmchains-0.0.6/tests/test_func.py`

 * *Files identical despite different names*

