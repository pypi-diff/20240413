# Comparing `tmp/UniswapPy-1.1.4.tar.gz` & `tmp/UniswapPy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UniswapPy-1.1.4.tar", last modified: Wed Feb 14 00:36:56 2024, max compression
+gzip compressed data, was "UniswapPy-1.2.0.tar", last modified: Fri Apr 12 22:51:17 2024, max compression
```

## Comparing `UniswapPy-1.1.4.tar` & `UniswapPy-1.2.0.tar`

### file list

```diff
@@ -1,110 +1,116 @@
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.582322 UniswapPy-1.1.4/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1065 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/LICENSE.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)     2872 2024-02-14 00:36:56.582256 UniswapPy-1.1.4/PKG-INFO
--rw-r--r--   0 ian_moore   (501) staff       (20)     2568 2024-02-11 01:32:07.000000 UniswapPy-1.1.4/README.md
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.568336 UniswapPy-1.1.4/UniswapPy.egg-info/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2872 2024-02-14 00:36:56.000000 UniswapPy-1.1.4/UniswapPy.egg-info/PKG-INFO
--rw-r--r--   0 ian_moore   (501) staff       (20)     2904 2024-02-14 00:36:56.000000 UniswapPy-1.1.4/UniswapPy.egg-info/SOURCES.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-02-14 00:36:56.000000 UniswapPy-1.1.4/UniswapPy.egg-info/dependency_links.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-02-11 00:15:12.000000 UniswapPy-1.1.4/UniswapPy.egg-info/not-zip-safe
--rw-r--r--   0 ian_moore   (501) staff       (20)       13 2024-02-14 00:36:56.000000 UniswapPy-1.1.4/UniswapPy.egg-info/requires.txt
--rw-r--r--   0 ian_moore   (501) staff       (20)       10 2024-02-14 00:36:56.000000 UniswapPy-1.1.4/UniswapPy.egg-info/top_level.txt
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.564854 UniswapPy-1.1.4/python/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.568480 UniswapPy-1.1.4/python/prod/
--rw-r--r--   0 ian_moore   (501) staff       (20)      804 2024-02-08 01:27:16.000000 UniswapPy-1.1.4/python/prod/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.565376 UniswapPy-1.1.4/python/prod/cpt/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.569331 UniswapPy-1.1.4/python/prod/cpt/exchg/
--rw-r--r--   0 ian_moore   (501) staff       (20)     7376 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/cpt/exchg/ChildUniswapExchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)    21514 2024-02-13 20:28:17.000000 UniswapPy-1.1.4/python/prod/cpt/exchg/UniswapExchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       99 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/cpt/exchg/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.569826 UniswapPy-1.1.4/python/prod/cpt/factory/
--rw-r--r--   0 ian_moore   (501) staff       (20)     3516 2024-02-13 21:52:11.000000 UniswapPy-1.1.4/python/prod/cpt/factory/UniswapFactory.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       44 2024-02-07 00:37:49.000000 UniswapPy-1.1.4/python/prod/cpt/factory/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.570571 UniswapPy-1.1.4/python/prod/cpt/index/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1719 2024-02-13 21:41:28.000000 UniswapPy-1.1.4/python/prod/cpt/index/RebaseIndexToken.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1712 2024-02-13 21:41:15.000000 UniswapPy-1.1.4/python/prod/cpt/index/SettlementLPToken.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/cpt/index/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.571831 UniswapPy-1.1.4/python/prod/cpt/quote/
--rw-r--r--   0 ian_moore   (501) staff       (20)     6938 2024-02-13 21:15:34.000000 UniswapPy-1.1.4/python/prod/cpt/quote/IndexTokenQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     6990 2024-02-13 21:32:43.000000 UniswapPy-1.1.4/python/prod/cpt/quote/LPQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1752 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/cpt/quote/LPTokenQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/cpt/quote/TreeAmountQuote.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/cpt/quote/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.572375 UniswapPy-1.1.4/python/prod/cpt/vault/
--rw-r--r--   0 ian_moore   (501) staff       (20)    15329 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/cpt/vault/IndexVault.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      651 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/cpt/vault/Vault.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       59 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/cpt/vault/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.572779 UniswapPy-1.1.4/python/prod/cpt/wallet/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2646 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/cpt/wallet/Wallets.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/cpt/wallet/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.573756 UniswapPy-1.1.4/python/prod/erc/
--rw-r--r--   0 ian_moore   (501) staff       (20)     1684 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/erc/DOAERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1521 2024-02-13 20:20:26.000000 UniswapPy-1.1.4/python/prod/erc/ERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1103 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/erc/IndexERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1720 2024-02-13 20:20:33.000000 UniswapPy-1.1.4/python/prod/erc/LPERC20.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      119 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/erc/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.565962 UniswapPy-1.1.4/python/prod/math/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.574216 UniswapPy-1.1.4/python/prod/math/basic/
--rw-r--r--   0 ian_moore   (501) staff       (20)      500 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/math/basic/IDGenerator.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      485 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/math/basic/RoundFloat.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       52 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/math/basic/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.574666 UniswapPy-1.1.4/python/prod/math/interest/
--rw-r--r--   0 ian_moore   (501) staff       (20)      410 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/math/interest/CompoundReturn.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      519 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/math/interest/Yield.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       50 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/math/interest/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.575361 UniswapPy-1.1.4/python/prod/math/interest/ips/
--rw-r--r--   0 ian_moore   (501) staff       (20)      766 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/math/interest/ips/ConstantIPS.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      390 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/math/interest/ips/IPS.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       45 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/math/interest/ips/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.575713 UniswapPy-1.1.4/python/prod/math/interest/ips/aggregate/
--rw-r--r--   0 ian_moore   (501) staff       (20)      496 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/math/interest/ips/aggregate/AggregateIPS.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       27 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/math/interest/ips/aggregate/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.576625 UniswapPy-1.1.4/python/prod/math/model/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2069 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/math/model/BrownianModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      504 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/math/model/EventSelectionModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      591 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/math/model/ModelQueue.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      762 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/math/model/TimeDeltaModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1262 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/math/model/TokenDeltaModel.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      151 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/math/model/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.577065 UniswapPy-1.1.4/python/prod/math/risk/
--rw-r--r--   0 ian_moore   (501) staff       (20)     5556 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/math/risk/MaxDrop.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       22 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/math/risk/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.577390 UniswapPy-1.1.4/python/prod/process/
--rw-r--r--   0 ian_moore   (501) staff       (20)      300 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/process/Process.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/process/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.577808 UniswapPy-1.1.4/python/prod/process/burn/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2470 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/process/burn/IndexTokenBurn.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       43 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/process/burn/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.578105 UniswapPy-1.1.4/python/prod/process/deposit/
--rw-r--r--   0 ian_moore   (501) staff       (20)     3690 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/process/deposit/SwapDeposit.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/process/deposit/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.578567 UniswapPy-1.1.4/python/prod/process/liquidity/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2434 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/process/liquidity/AddLiquidity.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     2393 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/process/liquidity/RemoveLiquidity.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       83 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/process/liquidity/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.578858 UniswapPy-1.1.4/python/prod/process/mint/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2747 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/process/mint/SwapIndexMint.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       40 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/process/mint/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.579624 UniswapPy-1.1.4/python/prod/process/swap/
--rw-r--r--   0 ian_moore   (501) staff       (20)     2328 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/process/swap/RandomSwap.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1805 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/process/swap/Swap.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     3996 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/process/swap/WithdrawSwap.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/process/swap/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.580556 UniswapPy-1.1.4/python/prod/simulate/
--rw-r--r--   0 ian_moore   (501) staff       (20)     3383 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/simulate/Arbitrage.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     3648 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/simulate/MarkovState.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     2712 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/simulate/SimpleLPSimulation.py
--rw-r--r--   0 ian_moore   (501) staff       (20)     1850 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/simulate/SolveDeltas.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      158 2024-02-07 00:37:32.000000 UniswapPy-1.1.4/python/prod/simulate/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.566724 UniswapPy-1.1.4/python/prod/utils/
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.581259 UniswapPy-1.1.4/python/prod/utils/data/
--rw-r--r--   0 ian_moore   (501) staff       (20)      261 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/utils/data/ExchangeData.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      324 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/utils/data/FactoryData.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      341 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/utils/data/UniswapExchangeData.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      128 2024-02-08 01:23:29.000000 UniswapPy-1.1.4/python/prod/utils/data/__init__.py
-drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-02-14 00:36:56.581799 UniswapPy-1.1.4/python/prod/utils/interfaces/
--rw-r--r--   0 ian_moore   (501) staff       (20)      439 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/utils/interfaces/IExchange.py
--rw-r--r--   0 ian_moore   (501) staff       (20)      506 2024-02-11 00:47:28.000000 UniswapPy-1.1.4/python/prod/utils/interfaces/IExchangeFactory.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-02-07 00:37:49.000000 UniswapPy-1.1.4/python/prod/utils/interfaces/__init__.py
--rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-02-14 00:36:56.582665 UniswapPy-1.1.4/setup.cfg
--rw-r--r--   0 ian_moore   (501) staff       (20)     1395 2024-02-14 00:29:52.000000 UniswapPy-1.1.4/setup.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.019214 UniswapPy-1.2.0/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1065 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/LICENSE.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3714 2024-04-12 22:51:17.019281 UniswapPy-1.2.0/PKG-INFO
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3418 2024-04-10 18:19:34.000000 UniswapPy-1.2.0/README.md
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.000437 UniswapPy-1.2.0/UniswapPy.egg-info/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3714 2024-04-12 22:51:16.000000 UniswapPy-1.2.0/UniswapPy.egg-info/PKG-INFO
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3087 2024-04-12 22:51:16.000000 UniswapPy-1.2.0/UniswapPy.egg-info/SOURCES.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-04-12 22:51:16.000000 UniswapPy-1.2.0/UniswapPy.egg-info/dependency_links.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)        1 2024-02-11 00:15:12.000000 UniswapPy-1.2.0/UniswapPy.egg-info/not-zip-safe
+-rw-r--r--   0 ian_moore   (501) staff       (20)       13 2024-04-12 22:51:16.000000 UniswapPy-1.2.0/UniswapPy.egg-info/requires.txt
+-rw-r--r--   0 ian_moore   (501) staff       (20)       10 2024-04-12 22:51:16.000000 UniswapPy-1.2.0/UniswapPy.egg-info/top_level.txt
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:16.996923 UniswapPy-1.2.0/python/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.000565 UniswapPy-1.2.0/python/prod/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      841 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:16.997413 UniswapPy-1.2.0/python/prod/cpt/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.001459 UniswapPy-1.2.0/python/prod/cpt/exchg/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     7376 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/cpt/exchg/ChildUniswapExchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    21514 2024-02-13 20:28:17.000000 UniswapPy-1.2.0/python/prod/cpt/exchg/UniswapExchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       99 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/cpt/exchg/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.001897 UniswapPy-1.2.0/python/prod/cpt/factory/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3516 2024-02-13 21:52:11.000000 UniswapPy-1.2.0/python/prod/cpt/factory/UniswapFactory.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       44 2024-02-07 00:37:49.000000 UniswapPy-1.2.0/python/prod/cpt/factory/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.002563 UniswapPy-1.2.0/python/prod/cpt/index/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1719 2024-02-13 21:41:28.000000 UniswapPy-1.2.0/python/prod/cpt/index/RebaseIndexToken.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1712 2024-02-13 21:41:15.000000 UniswapPy-1.2.0/python/prod/cpt/index/SettlementLPToken.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/cpt/index/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.008665 UniswapPy-1.2.0/python/prod/cpt/quote/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6938 2024-02-13 21:15:34.000000 UniswapPy-1.2.0/python/prod/cpt/quote/IndexTokenQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     6990 2024-02-13 21:32:43.000000 UniswapPy-1.2.0/python/prod/cpt/quote/LPQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1752 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/cpt/quote/LPTokenQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4677 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/cpt/quote/TreeAmountQuote.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/cpt/quote/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.009281 UniswapPy-1.2.0/python/prod/cpt/vault/
+-rw-r--r--   0 ian_moore   (501) staff       (20)    15329 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/cpt/vault/IndexVault.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      651 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/cpt/vault/Vault.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       59 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/cpt/vault/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.010123 UniswapPy-1.2.0/python/prod/cpt/wallet/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2646 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/cpt/wallet/Wallets.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/cpt/wallet/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.011047 UniswapPy-1.2.0/python/prod/erc/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1684 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/erc/DOAERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1456 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/erc/ERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1103 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/erc/IndexERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1720 2024-02-13 20:20:33.000000 UniswapPy-1.2.0/python/prod/erc/LPERC20.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      119 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/erc/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:16.998030 UniswapPy-1.2.0/python/prod/math/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.011488 UniswapPy-1.2.0/python/prod/math/basic/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      500 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/basic/IDGenerator.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      485 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/basic/RoundFloat.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       52 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/basic/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.011883 UniswapPy-1.2.0/python/prod/math/interest/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      410 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/interest/CompoundReturn.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      519 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/interest/Yield.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       50 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/interest/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.012276 UniswapPy-1.2.0/python/prod/math/interest/ips/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      766 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/interest/ips/ConstantIPS.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      390 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/interest/ips/IPS.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       45 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/interest/ips/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.012539 UniswapPy-1.2.0/python/prod/math/interest/ips/aggregate/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      496 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/interest/ips/aggregate/AggregateIPS.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       27 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/interest/ips/aggregate/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.013315 UniswapPy-1.2.0/python/prod/math/model/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2069 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/model/BrownianModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      504 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/model/EventSelectionModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      591 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/model/ModelQueue.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      762 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/model/TimeDeltaModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1262 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/model/TokenDeltaModel.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      151 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/math/model/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.013671 UniswapPy-1.2.0/python/prod/math/risk/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     5556 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/risk/MaxDrop.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       22 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/math/risk/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.013911 UniswapPy-1.2.0/python/prod/process/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      300 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/Process.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       28 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/process/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.014263 UniswapPy-1.2.0/python/prod/process/burn/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2470 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/burn/IndexTokenBurn.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       43 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/process/burn/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.014508 UniswapPy-1.2.0/python/prod/process/deposit/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3690 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/deposit/SwapDeposit.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       36 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/process/deposit/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.014869 UniswapPy-1.2.0/python/prod/process/liquidity/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2434 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/liquidity/AddLiquidity.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2393 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/liquidity/RemoveLiquidity.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       83 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/process/liquidity/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.015111 UniswapPy-1.2.0/python/prod/process/mint/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2747 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/mint/SwapIndexMint.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       40 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/process/mint/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.015850 UniswapPy-1.2.0/python/prod/process/swap/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2329 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/process/swap/RandomSwap.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1805 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/swap/Swap.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3996 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/process/swap/WithdrawSwap.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       96 2024-02-07 00:37:32.000000 UniswapPy-1.2.0/python/prod/process/swap/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.017005 UniswapPy-1.2.0/python/prod/simulate/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3383 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/simulate/Arbitrage.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     4185 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/simulate/CorrectReserves.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     3648 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/simulate/MarkovState.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)    15429 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/simulate/QuantTerminal.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2712 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/simulate/SimpleLPSimulation.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1850 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/simulate/SolveDeltas.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      244 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/simulate/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:16.998821 UniswapPy-1.2.0/python/prod/utils/
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.017254 UniswapPy-1.2.0/python/prod/utils/client/
+-rw-r--r--   0 ian_moore   (501) staff       (20)     2164 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/utils/client/API0x.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       24 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/utils/client/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.018595 UniswapPy-1.2.0/python/prod/utils/data/
+-rw-r--r--   0 ian_moore   (501) staff       (20)    10464 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/utils/data/Chain0x.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      261 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/utils/data/ExchangeData.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      324 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/utils/data/FactoryData.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      341 2024-03-25 21:57:46.000000 UniswapPy-1.2.0/python/prod/utils/data/UniswapExchangeData.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      157 2024-04-10 18:17:44.000000 UniswapPy-1.2.0/python/prod/utils/data/__init__.py
+drwxr-xr-x   0 ian_moore   (501) staff       (20)        0 2024-04-12 22:51:17.018973 UniswapPy-1.2.0/python/prod/utils/interfaces/
+-rw-r--r--   0 ian_moore   (501) staff       (20)      439 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/utils/interfaces/IExchange.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)      506 2024-02-11 00:47:28.000000 UniswapPy-1.2.0/python/prod/utils/interfaces/IExchangeFactory.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-02-07 00:37:49.000000 UniswapPy-1.2.0/python/prod/utils/interfaces/__init__.py
+-rw-r--r--   0 ian_moore   (501) staff       (20)       79 2024-04-12 22:51:17.019490 UniswapPy-1.2.0/setup.cfg
+-rw-r--r--   0 ian_moore   (501) staff       (20)     1440 2024-04-12 22:46:30.000000 UniswapPy-1.2.0/setup.py
```

### Comparing `UniswapPy-1.1.4/LICENSE.txt` & `UniswapPy-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/PKG-INFO` & `UniswapPy-1.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,45 @@
-Metadata-Version: 2.1
-Name: UniswapPy
-Version: 1.1.4
-Summary: Uniswap Analytics with Python
-Home-page: https://github.com/defipy-devs/uniswappy
-Author: icmoore
-Author-email: defipy.devs@gmail.com
-License: MIT
-Description-Content-Type: text/markdown
-License-File: LICENSE.txt
-Requires-Dist: scipy>=1.7.3
-
-# UniswapPy
-This package is a python re-factor of the original [Uniswap V2 pairing code](https://github.com/Uniswap/v2-core/blob/master/contracts/UniswapV2Pair.sol) and can be 
+# UniswapPy: Uniswap Analytics with Python
+This package is a python re-factor of the original [Uniswap V2 pairing 
+code](https://github.com/Uniswap/v2-core/blob/master/contracts/UniswapV2Pair.sol) 
+and can be 
 utilized for the purpose of analysing and modelling its behavior for DeFi
 
-To install package:
+## Docs
+Visit [docs](https://defipy.org) for full documentation with walk-through 
+tutorials
+
+## Installation 
 ```
 > git clone https://github.com/defipy-devs/uniswappy
 > pip install .
 ```
 or
 ```
 > pip install UniswapPy
 ```
 
-# Basic Usage
+## Basic Usage
 
-* See [test notebook](https://github.com/icmoore/uniswappy/blob/main/notebooks/tutorials/pairingcode.ipynb) for basic usage
+* See [test notebook](https://github.com/icmoore/uniswappy/blob/main/notebooks/tutorials/pairingcode.ipynb) 
+for basic usage
 
 ```
 from uniswappy.erc import ERC20
 from uniswappy.cpt.factory import UniswapFactory
 from uniswappy.utils.data import UniswapExchangeData
 
 user_nm = 'user_intro'
 eth_amount = 1000
 dai_amount = 1000000
 
 dai = ERC20("DAI", "0x111")
 eth = ERC20("ETH", "0x09")
-exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", address="0x011")
+exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", 
+address="0x011")
 
 factory = UniswapFactory("ETH pool factory", "0x2")
 lp = factory.deploy(exchg_data)
 lp.add_liquidity("user0", eth_amount, dai_amount, eth_amount, dai_amount)
 lp.summary()
 ```
 
@@ -59,15 +55,45 @@
 ```
 
 #### OUTPUT:
 Exchange ETH-DAI (LP) <br/>
 Reserves: ETH = 999.00399301896, DAI = 1001000 <br/>
 Liquidity: 31622.776601683792 <br/><br/>
 
-# Special Features
- * **Abstracted Actions**: Obfuscation is removed from standard Uniswap action events to help streamline analysis and lower line count; see article [How to Handle Uniswap Withdrawals like an OG](https://medium.com/coinmonks/handle-uniswap-withdrawals-like-an-og-389fe74be18c), and [Setup your Uniswap Deposits like a Baller](https://medium.com/coinmonks/setup-your-uniswap-deposits-like-a-baller-b99340ea302f)
- * **Indexing**: Can calculate settlment LP token amounts given token amounts and vice versa; see article [The Uniswap Indexing Problem](https://medium.com/datadriveninvestor/the-uniswap-indexing-problem-8078b8b110fc)
- * **Simulation**: Can simulate trading using Geometric Brownian Motion (GBM) process, or feed in actual raw price data to analyze behavior; see article [How to Simulate a Liquidity Pool for Decentralized Finance](https://medium.com/@icmoore/simulating-a-liquidity-pool-for-decentralized-finance-6f357ec8564b)
- * **Randomized Events**: Token amount and time delta models to simulate possible trading behavior
- * **Analytical Tools**: Basic yeild calculators and risk tools to assist in analyzing outcomes
+## 0x Quant Terminal
+
+This application utilizes the 0x API to produce a mock Uniswap pool which allows end-users to stress test
+the limitations of a Uniswap pool setup using live price feeds from [0x API](https://0x.org); for backend setup, see 
+[notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/quant_terminal.ipynb) 
+
+Click [dashboard.defipy.org](https://dashboard.defipy.org/) for live link; for more detail see 
+[README](https://github.com/defipy-devs/uniswappy/tree/main/python/application/quant_terminal#readme) 
+
+![plot](./doc/quant_terminal/screenshot.png)
+
+### Run application locally  
+
+```
+> bokeh serve --show python/application/quant_terminal/bokeh_server.py
+```
+
+## Special Features
+ * **Abstracted Actions**: Obfuscation is removed from standard Uniswap 
+action events to help streamline analysis and lower line count; see 
+article [How to Handle Uniswap Withdrawals like an 
+OG](https://medium.com/coinmonks/handle-uniswap-withdrawals-like-an-og-389fe74be18c), 
+and [Setup your Uniswap Deposits like a 
+Baller](https://medium.com/coinmonks/setup-your-uniswap-deposits-like-a-baller-b99340ea302f)
+ * **Indexing**: Can calculate settlment LP token amounts given token 
+amounts and vice versa; see article [The Uniswap Indexing 
+Problem](https://medium.com/datadriveninvestor/the-uniswap-indexing-problem-8078b8b110fc)
+ * **Simulation**: Can simulate trading using Geometric Brownian Motion 
+(GBM) process, or feed in actual raw price data to analyze behavior; see 
+article [How to Simulate a Liquidity Pool for Decentralized 
+Finance](https://medium.com/@icmoore/simulating-a-liquidity-pool-for-decentralized-finance-6f357ec8564b)
+ * **Randomized Events**: Token amount and time delta models to simulate 
+possible trading behavior
+ * **Analytical Tools**: Basic yeild calculators and risk tools to assist 
+in analyzing outcomes
  
  
+
```

### Comparing `UniswapPy-1.1.4/README.md` & `UniswapPy-1.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,37 +1,57 @@
-# UniswapPy
-This package is a python re-factor of the original [Uniswap V2 pairing code](https://github.com/Uniswap/v2-core/blob/master/contracts/UniswapV2Pair.sol) and can be 
+Metadata-Version: 2.1
+Name: UniswapPy
+Version: 1.2.0
+Summary: Uniswap Analytics with Python
+Home-page: https://github.com/defipy-devs/uniswappy
+Author: icmoore
+Author-email: defipy.devs@gmail.com
+License: MIT
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# UniswapPy: Uniswap Analytics with Python
+This package is a python re-factor of the original [Uniswap V2 pairing 
+code](https://github.com/Uniswap/v2-core/blob/master/contracts/UniswapV2Pair.sol) 
+and can be 
 utilized for the purpose of analysing and modelling its behavior for DeFi
 
-To install package:
+## Docs
+Visit [docs](https://defipy.org) for full documentation with walk-through 
+tutorials
+
+## Installation 
 ```
 > git clone https://github.com/defipy-devs/uniswappy
 > pip install .
 ```
 or
 ```
 > pip install UniswapPy
 ```
 
-# Basic Usage
+## Basic Usage
 
-* See [test notebook](https://github.com/icmoore/uniswappy/blob/main/notebooks/tutorials/pairingcode.ipynb) for basic usage
+* See [test notebook](https://github.com/icmoore/uniswappy/blob/main/notebooks/tutorials/pairingcode.ipynb) 
+for basic usage
 
 ```
 from uniswappy.erc import ERC20
 from uniswappy.cpt.factory import UniswapFactory
 from uniswappy.utils.data import UniswapExchangeData
 
 user_nm = 'user_intro'
 eth_amount = 1000
 dai_amount = 1000000
 
 dai = ERC20("DAI", "0x111")
 eth = ERC20("ETH", "0x09")
-exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", address="0x011")
+exchg_data = UniswapExchangeData(tkn0 = eth, tkn1 = dai, symbol="LP", 
+address="0x011")
 
 factory = UniswapFactory("ETH pool factory", "0x2")
 lp = factory.deploy(exchg_data)
 lp.add_liquidity("user0", eth_amount, dai_amount, eth_amount, dai_amount)
 lp.summary()
 ```
 
@@ -47,15 +67,47 @@
 ```
 
 #### OUTPUT:
 Exchange ETH-DAI (LP) <br/>
 Reserves: ETH = 999.00399301896, DAI = 1001000 <br/>
 Liquidity: 31622.776601683792 <br/><br/>
 
-# Special Features
- * **Abstracted Actions**: Obfuscation is removed from standard Uniswap action events to help streamline analysis and lower line count; see article [How to Handle Uniswap Withdrawals like an OG](https://medium.com/coinmonks/handle-uniswap-withdrawals-like-an-og-389fe74be18c), and [Setup your Uniswap Deposits like a Baller](https://medium.com/coinmonks/setup-your-uniswap-deposits-like-a-baller-b99340ea302f)
- * **Indexing**: Can calculate settlment LP token amounts given token amounts and vice versa; see article [The Uniswap Indexing Problem](https://medium.com/datadriveninvestor/the-uniswap-indexing-problem-8078b8b110fc)
- * **Simulation**: Can simulate trading using Geometric Brownian Motion (GBM) process, or feed in actual raw price data to analyze behavior; see article [How to Simulate a Liquidity Pool for Decentralized Finance](https://medium.com/@icmoore/simulating-a-liquidity-pool-for-decentralized-finance-6f357ec8564b)
- * **Randomized Events**: Token amount and time delta models to simulate possible trading behavior
- * **Analytical Tools**: Basic yeild calculators and risk tools to assist in analyzing outcomes
+## 0x Quant Terminal
+
+This application utilizes the 0x API to produce a mock Uniswap pool which allows end-users to stress test
+the limitations of a Uniswap pool setup using live price feeds from [0x API](https://0x.org); for backend setup, see 
+[notebook](https://github.com/defipy-devs/uniswappy/blob/main/notebooks/tutorials/quant_terminal.ipynb) 
+
+Click [dashboard.defipy.org](https://dashboard.defipy.org/) for live link; for more detail see 
+[README](https://github.com/defipy-devs/uniswappy/tree/main/python/application/quant_terminal#readme) 
+
+![plot](./doc/quant_terminal/screenshot.png)
+
+### Run application locally  
+
+```
+> bokeh serve --show python/application/quant_terminal/bokeh_server.py
+```
+
+## Special Features
+ * **Abstracted Actions**: Obfuscation is removed from standard Uniswap 
+action events to help streamline analysis and lower line count; see 
+article [How to Handle Uniswap Withdrawals like an 
+OG](https://medium.com/coinmonks/handle-uniswap-withdrawals-like-an-og-389fe74be18c), 
+and [Setup your Uniswap Deposits like a 
+Baller](https://medium.com/coinmonks/setup-your-uniswap-deposits-like-a-baller-b99340ea302f)
+ * **Indexing**: Can calculate settlment LP token amounts given token 
+amounts and vice versa; see article [The Uniswap Indexing 
+Problem](https://medium.com/datadriveninvestor/the-uniswap-indexing-problem-8078b8b110fc)
+ * **Simulation**: Can simulate trading using Geometric Brownian Motion 
+(GBM) process, or feed in actual raw price data to analyze behavior; see 
+article [How to Simulate a Liquidity Pool for Decentralized 
+Finance](https://medium.com/@icmoore/simulating-a-liquidity-pool-for-decentralized-finance-6f357ec8564b)
+ * **Randomized Events**: Token amount and time delta models to simulate 
+possible trading behavior
+ * **Analytical Tools**: Basic yeild calculators and risk tools to assist 
+in analyzing outcomes
  
  
+
+
+
```

### Comparing `UniswapPy-1.1.4/UniswapPy.egg-info/SOURCES.txt` & `UniswapPy-1.2.0/UniswapPy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -63,18 +63,23 @@
 python/prod/process/mint/SwapIndexMint.py
 python/prod/process/mint/__init__.py
 python/prod/process/swap/RandomSwap.py
 python/prod/process/swap/Swap.py
 python/prod/process/swap/WithdrawSwap.py
 python/prod/process/swap/__init__.py
 python/prod/simulate/Arbitrage.py
+python/prod/simulate/CorrectReserves.py
 python/prod/simulate/MarkovState.py
+python/prod/simulate/QuantTerminal.py
 python/prod/simulate/SimpleLPSimulation.py
 python/prod/simulate/SolveDeltas.py
 python/prod/simulate/__init__.py
+python/prod/utils/client/API0x.py
+python/prod/utils/client/__init__.py
+python/prod/utils/data/Chain0x.py
 python/prod/utils/data/ExchangeData.py
 python/prod/utils/data/FactoryData.py
 python/prod/utils/data/UniswapExchangeData.py
 python/prod/utils/data/__init__.py
 python/prod/utils/interfaces/IExchange.py
 python/prod/utils/interfaces/IExchangeFactory.py
 python/prod/utils/interfaces/__init__.py
```

### Comparing `UniswapPy-1.1.4/python/prod/__init__.py` & `UniswapPy-1.2.0/python/prod/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,8 +15,9 @@
 from uniswappy.process.burn import *
 from uniswappy.process.deposit import *
 from uniswappy.process.liquidity import *
 from uniswappy.process.mint import *
 from uniswappy.process.swap import *
 from uniswappy.simulate import *
 from uniswappy.utils.interfaces import *
-from uniswappy.utils.data import *
+from uniswappy.utils.data import *
+from uniswappy.utils.client import *
```

### Comparing `UniswapPy-1.1.4/python/prod/cpt/exchg/ChildUniswapExchange.py` & `UniswapPy-1.2.0/python/prod/cpt/exchg/ChildUniswapExchange.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/cpt/exchg/UniswapExchange.py` & `UniswapPy-1.2.0/python/prod/cpt/exchg/UniswapExchange.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/cpt/factory/UniswapFactory.py` & `UniswapPy-1.2.0/python/prod/cpt/factory/UniswapFactory.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/cpt/index/RebaseIndexToken.py` & `UniswapPy-1.2.0/python/prod/cpt/index/RebaseIndexToken.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/cpt/index/SettlementLPToken.py` & `UniswapPy-1.2.0/python/prod/cpt/index/SettlementLPToken.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/cpt/quote/IndexTokenQuote.py` & `UniswapPy-1.2.0/python/prod/cpt/quote/IndexTokenQuote.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/cpt/quote/LPQuote.py` & `UniswapPy-1.2.0/python/prod/cpt/quote/LPQuote.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/cpt/quote/LPTokenQuote.py` & `UniswapPy-1.2.0/python/prod/cpt/quote/LPTokenQuote.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/cpt/quote/TreeAmountQuote.py` & `UniswapPy-1.2.0/python/prod/cpt/quote/TreeAmountQuote.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/cpt/vault/IndexVault.py` & `UniswapPy-1.2.0/python/prod/cpt/vault/IndexVault.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/cpt/vault/Vault.py` & `UniswapPy-1.2.0/python/prod/cpt/vault/Vault.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/cpt/wallet/Wallets.py` & `UniswapPy-1.2.0/python/prod/cpt/wallet/Wallets.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/erc/DOAERC20.py` & `UniswapPy-1.2.0/python/prod/erc/DOAERC20.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/erc/ERC20.py` & `UniswapPy-1.2.0/python/prod/erc/ERC20.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Distributed under the MIT License (license terms are at http://opensource.org/licenses/MIT).
 # Email: defipy.devs@gmail.com
 
 GWEI_PRECISION = 18
 
 class ERC20:
     
-    """ ERC20 token akjhsflkjbvjn cn vvk
+    """ ERC20 token
 
         Parameters
         -----------------
         self.token_name : str
             Token name 
         self.token_addr : str
             Token address  
@@ -23,15 +23,15 @@
         self.token_addr = addr
         self.token_total = 0
         self.token_decimal = GWEI_PRECISION if decimal == None else decimal
         self.type = 'standard'
 
     def deposit(self, _from, value):
         
-        """ deposit intlkaflkw nsdlkamnas
+        """ deposit
 
             Deposit token
                 
             Parameters
             -----------------
             _from : str
                 user address   
@@ -39,15 +39,15 @@
                 delta to add to total                
         """           
         
         self.token_total += value
 
     def transfer(self, _to, value):
         
-        """ transfer intlkaflkwns dlkamnas
+        """ transfer
 
             Transfer token
                 
             Parameters
             -----------------
             _to : str
                 user address
```

### Comparing `UniswapPy-1.1.4/python/prod/erc/IndexERC20.py` & `UniswapPy-1.2.0/python/prod/erc/IndexERC20.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/erc/LPERC20.py` & `UniswapPy-1.2.0/python/prod/erc/LPERC20.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/math/interest/Yield.py` & `UniswapPy-1.2.0/python/prod/math/interest/Yield.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/math/interest/ips/ConstantIPS.py` & `UniswapPy-1.2.0/python/prod/math/interest/ips/ConstantIPS.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/math/model/BrownianModel.py` & `UniswapPy-1.2.0/python/prod/math/model/BrownianModel.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/math/model/ModelQueue.py` & `UniswapPy-1.2.0/python/prod/math/model/ModelQueue.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/math/model/TimeDeltaModel.py` & `UniswapPy-1.2.0/python/prod/math/model/TimeDeltaModel.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/math/model/TokenDeltaModel.py` & `UniswapPy-1.2.0/python/prod/math/model/TokenDeltaModel.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/math/risk/MaxDrop.py` & `UniswapPy-1.2.0/python/prod/math/risk/MaxDrop.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/process/burn/IndexTokenBurn.py` & `UniswapPy-1.2.0/python/prod/process/burn/IndexTokenBurn.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/process/deposit/SwapDeposit.py` & `UniswapPy-1.2.0/python/prod/process/deposit/SwapDeposit.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/process/liquidity/AddLiquidity.py` & `UniswapPy-1.2.0/python/prod/process/liquidity/AddLiquidity.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/process/liquidity/RemoveLiquidity.py` & `UniswapPy-1.2.0/python/prod/process/liquidity/RemoveLiquidity.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/process/mint/SwapIndexMint.py` & `UniswapPy-1.2.0/python/prod/process/mint/SwapIndexMint.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/process/swap/RandomSwap.py` & `UniswapPy-1.2.0/python/prod/process/swap/RandomSwap.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
             -------
             amount_out_expected : float
                 exchanged token amount               
         """         
         
         amount_in = self.tDel.delta() if amount_in == None else amount_in
         direction = self.ev.bi_select(self.buy_sell_prob) 
-        tokens = lp.factory.exchange_to_tokens[lp.name]
+        tokens = lp.factory.token_from_exchange[lp.name]
         
         
         #print('direction {}, p {}'.format(direction, self.buy_sell_prob))
 
         if(direction == 0):
             token_in = tokens[lp.token0]
             amount_out_expected = Swap().apply(lp, token_in, user_nm, amount_in)
```

### Comparing `UniswapPy-1.1.4/python/prod/process/swap/Swap.py` & `UniswapPy-1.2.0/python/prod/process/swap/Swap.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/process/swap/WithdrawSwap.py` & `UniswapPy-1.2.0/python/prod/process/swap/WithdrawSwap.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/simulate/Arbitrage.py` & `UniswapPy-1.2.0/python/prod/simulate/Arbitrage.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/simulate/MarkovState.py` & `UniswapPy-1.2.0/python/prod/simulate/MarkovState.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/simulate/SimpleLPSimulation.py` & `UniswapPy-1.2.0/python/prod/simulate/SimpleLPSimulation.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/python/prod/simulate/SolveDeltas.py` & `UniswapPy-1.2.0/python/prod/simulate/SolveDeltas.py`

 * *Files identical despite different names*

### Comparing `UniswapPy-1.1.4/setup.py` & `UniswapPy-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup
 
 with open('README.md') as f:
     long_description = f.read()
 
 setup(name='UniswapPy',
-      version='1.1.4',
+      version='1.2.0',
       description='Uniswap Analytics with Python',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/defipy-devs/uniswappy',
       author = "icmoore",
       author_email = "defipy.devs@gmail.com",
       license='MIT',
@@ -32,13 +32,14 @@
           'uniswappy.process.burn',
           'uniswappy.process.deposit',
           'uniswappy.process.liquidity',
           'uniswappy.process.mint',
           'uniswappy.process.swap',
           'uniswappy.simulate',
           'uniswappy.utils.interfaces',
-          'uniswappy.utils.data'
+          'uniswappy.utils.data',
+          'uniswappy.utils.client'
       ],
       install_requires=[
-          'scipy >= 1.7.3'
+          'scipy >= 1.7.3'         
       ],
       zip_safe=False)
```

