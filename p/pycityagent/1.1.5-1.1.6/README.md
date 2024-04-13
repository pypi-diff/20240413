# Comparing `tmp/pycityagent-1.1.5.tar.gz` & `tmp/pycityagent-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycityagent-1.1.5.tar", last modified: Fri Apr 12 05:46:22 2024, max compression
+gzip compressed data, was "pycityagent-1.1.6.tar", last modified: Sat Apr 13 11:07:36 2024, max compression
```

## Comparing `pycityagent-1.1.5.tar` & `pycityagent-1.1.6.tar`

### file list

```diff
@@ -1,77 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:22.585463 pycityagent-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 05:46:18.000000 pycityagent-1.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-12 05:46:22.585463 pycityagent-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-12 05:46:18.000000 pycityagent-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:22.573464 pycityagent-1.1.5/pycityagent/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:22.577463 pycityagent-1.1.5/pycityagent/ac/
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/ac.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/action.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/action_stream.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:22.577463 pycityagent-1.1.5/pycityagent/ac/citizen_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/citizen_actions/controled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/citizen_actions/converse.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/citizen_actions/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/citizen_actions/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/citizen_actions/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/controled.py
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/converse.py
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/hub_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)     4095 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     3845 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/sim_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/ac/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8165 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     4972 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/agent_citizen.py
--rw-r--r--   0 runner    (1001) docker     (127)     4212 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/agent_func.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:22.581463 pycityagent-1.1.5/pycityagent/brain/
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/brain.py
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/brainfc.py
--rw-r--r--   0 runner    (1001) docker     (127)    21934 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:22.581463 pycityagent-1.1.5/pycityagent/brain/persistence/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/persistence/social.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/persistence/spatial.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:22.581463 pycityagent-1.1.5/pycityagent/brain/reason/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/reason/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/reason/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/reason/social.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/reason/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/reason/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:22.581463 pycityagent-1.1.5/pycityagent/brain/retrive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/retrive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/retrive/social.py
--rw-r--r--   0 runner    (1001) docker     (127)    18492 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    28683 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/sence.py
--rw-r--r--   0 runner    (1001) docker     (127)    29081 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/brain/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:22.581463 pycityagent-1.1.5/pycityagent/cc/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/cc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/cc/cc.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/cc/conve.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/cc/idle.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/cc/shop.py
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/cc/trip.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/cc/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:22.581463 pycityagent-1.1.5/pycityagent/hubconnector/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/hubconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/hubconnector/hubconnector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:22.581463 pycityagent-1.1.5/pycityagent/image/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/image/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:22.585463 pycityagent-1.1.5/pycityagent/st/
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/st/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/st/st.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:22.585463 pycityagent-1.1.5/pycityagent/urbanllm/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/urbanllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5176 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pycityagent/urbanllm/urbanllm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 05:46:22.585463 pycityagent-1.1.5/pycityagent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-12 05:46:22.000000 pycityagent-1.1.5/pycityagent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-12 05:46:22.000000 pycityagent-1.1.5/pycityagent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 05:46:22.000000 pycityagent-1.1.5/pycityagent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-12 05:46:22.000000 pycityagent-1.1.5/pycityagent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-12 05:46:22.000000 pycityagent-1.1.5/pycityagent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-12 05:46:18.000000 pycityagent-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 05:46:22.585463 pycityagent-1.1.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.995474 pycityagent-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-13 11:07:32.000000 pycityagent-1.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-13 11:07:36.995474 pycityagent-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2024-04-13 11:07:32.000000 pycityagent-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.987474 pycityagent-1.1.6/pycityagent/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.987474 pycityagent-1.1.6/pycityagent/ac/
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2267 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/ac.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/action_stream.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.987474 pycityagent-1.1.6/pycityagent/ac/citizen_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/citizen_actions/controled.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/citizen_actions/converse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/citizen_actions/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4273 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/citizen_actions/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/citizen_actions/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/hub_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/ac/sim_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8767 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/agent_citizen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/agent_func.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.991474 pycityagent-1.1.6/pycityagent/brain/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/brain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/brainfc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22067 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.991474 pycityagent-1.1.6/pycityagent/brain/persistence/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/persistence/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/persistence/spatial.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.991474 pycityagent-1.1.6/pycityagent/brain/reason/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/reason/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/reason/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/reason/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/reason/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6412 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/reason/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.991474 pycityagent-1.1.6/pycityagent/brain/retrive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/retrive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/retrive/social.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18593 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28724 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/sence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29101 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/brain/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.991474 pycityagent-1.1.6/pycityagent/cc/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/cc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/cc/cc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/cc/conve.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/cc/idle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/cc/shop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/cc/trip.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/cc/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.991474 pycityagent-1.1.6/pycityagent/hubconnector/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/hubconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/hubconnector/hubconnector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.991474 pycityagent-1.1.6/pycityagent/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/image/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.995474 pycityagent-1.1.6/pycityagent/st/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/st/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5210 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/st/st.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.995474 pycityagent-1.1.6/pycityagent/urbanllm/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/urbanllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5221 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pycityagent/urbanllm/urbanllm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 11:07:36.995474 pycityagent-1.1.6/pycityagent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7758 2024-04-13 11:07:36.000000 pycityagent-1.1.6/pycityagent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-04-13 11:07:36.000000 pycityagent-1.1.6/pycityagent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 11:07:36.000000 pycityagent-1.1.6/pycityagent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-13 11:07:36.000000 pycityagent-1.1.6/pycityagent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-13 11:07:36.000000 pycityagent-1.1.6/pycityagent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-13 11:07:32.000000 pycityagent-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 11:07:36.995474 pycityagent-1.1.6/setup.cfg
```

### Comparing `pycityagent-1.1.5/LICENSE` & `pycityagent-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.5/PKG-INFO` & `pycityagent-1.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityagent
-Version: 1.1.5
+Version: 1.1.6
 Summary: LLM-based城市模拟器agent构建库
 Author-email: Yuwei Yan <pinkgranite86@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pycityagent-1.1.5/README.md` & `pycityagent-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.5/pycityagent/ac/ac.py` & `pycityagent-1.1.6/pycityagent/ac/ac.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""命令控制器类及其定义"""
+
 from typing import Any, Optional, Union
 from .action import Action
 from .citizen_actions.trip import TripAction
 from .citizen_actions.shop import ShopAction
 from .citizen_actions.converse import ConverseAction
 from .citizen_actions.controled import ControledAction
 from .citizen_actions.idle import IdleAction
```

### Comparing `pycityagent-1.1.5/pycityagent/ac/action.py` & `pycityagent-1.1.6/pycityagent/ac/action.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Action类及其定义"""
+
 from abc import ABC, abstractclassmethod
 from typing import Callable, Any
 
 class ActionType:
     """
     行动类型枚举 所有行动本质上为数据推送
     Action Type enumeration, all actions are essentially data push
@@ -11,14 +13,17 @@
     - Hub = 2, 用于表示与AppHub(前端)对接的行动
     - Comp = 3, 表示综合类型 (可能同时包含与Sim以及Hub的交互)
     """
     Sim = 1
     Hub = 2
     Comp = 3
 class Action:
+    """
+    - Action
+    """
     def __init__(self, agent, type:ActionType, source: str = None, before:Callable[[list], Any] = None) -> None:
         '''
         默认初始化
         
         Args:
         - agent (Agent): the related agent
         - type (ActionType)
@@ -43,13 +48,15 @@
             return None
 
     @abstractclassmethod
     async def Forward(self):
         '''接口函数'''
 
 class SimAction(Action):
+    """SimAction: 模拟器关联Action"""
     def __init__(self, agent, source: str = None, before: Callable[[list], Any] = None) -> None:
         super().__init__(agent, ActionType.Sim, source, before)
 
 class HubAction(Action):
+    """HubAction: Apphub关联Action"""
     def __init__(self, agent, source: str = None, before: Callable[[list], Any] = None) -> None:
         super().__init__(agent, ActionType.Hub, source, before)
```

### Comparing `pycityagent-1.1.5/pycityagent/ac/action_stream.py` & `pycityagent-1.1.6/pycityagent/ac/action_stream.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.5/pycityagent/ac/citizen_actions/controled.py` & `pycityagent-1.1.6/pycityagent/ac/citizen_actions/controled.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.5/pycityagent/ac/citizen_actions/converse.py` & `pycityagent-1.1.6/pycityagent/ac/citizen_actions/converse.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.5/pycityagent/ac/citizen_actions/idle.py` & `pycityagent-1.1.6/pycityagent/ac/citizen_actions/idle.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.5/pycityagent/ac/citizen_actions/shop.py` & `pycityagent-1.1.6/pycityagent/ac/citizen_actions/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.5/pycityagent/ac/citizen_actions/trip.py` & `pycityagent-1.1.6/pycityagent/ac/citizen_actions/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.5/pycityagent/ac/hub_actions.py` & `pycityagent-1.1.6/pycityagent/ac/hub_actions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""AppHub关联Action定义"""
+
 from typing import Callable, Optional, Any
 from pycitysim.apphub import AgentMessage
 from .action import HubAction
 from PIL.Image import Image
 
 class SendUserMessage(HubAction):
     """
```

### Comparing `pycityagent-1.1.5/pycityagent/ac/sim_actions.py` & `pycityagent-1.1.6/pycityagent/ac/sim_actions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Simulator相关Action定义"""
+
 import time
 from typing import Callable, Optional, Any
 from .action import SimAction
 from ..brain.scheduler import TripSchedule
 
 class SetSchedule(SimAction):
     """
```

### Comparing `pycityagent-1.1.5/pycityagent/agent.py` & `pycityagent-1.1.6/pycityagent/agent.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""智能体模板类及其定义"""
+
 from abc import ABC, abstractmethod
 from typing import Optional, Union, Callable
 import PIL.Image as Image
 from PIL.Image import Image
 import asyncio
 import time
 from pycitysim.sim import CityClient
@@ -22,15 +24,16 @@
     - Func = 2, 功能型agent——行动规则宽松——本质上模拟器无法感知到Func类型的agent
     """
     Citizen = 1
     Func = 2
 
 class Template:
     """
-    The basic template of Agent
+    - 模板基类
+    - The basic template class
     """
     def __init__(self, name, server, type:AgentType, soul:UrbanLLM=None, simulator=None) -> None:
         self._name = name
         self._client = CityClient(server)
         self._type = type
         self._soul = soul
         self._simulator = simulator
@@ -57,59 +60,70 @@
 
     @abstractmethod
     def Step(self):
         """模拟器执行接口"""
 
 class Agent(Template):
     """
-    Agent
+    - 智能体基类
+    - Agent base class
     """
     def __init__(
             self, 
             name:str, 
             server:str, 
             type:AgentType,
             soul:UrbanLLM=None, 
             simulator=None
         ) -> None:
+        """
+        初始化 Init
+
+        Args:
+        - name (str): 智能体名称; name of your agent
+        - server (str): 模拟器grpc服务地址; server address of simulator
+        - type (AgentType): 智能体类型; type of agent
+        - soul (UrbanLLM): 基础模型模块; base model
+        - simulator (Simulator): 模拟器对象; simulator
+        """
         super().__init__(name, server, type, soul, simulator)
 
         self._hub_connector = None
         """
-        HubConnector: 用于和AppHub对接——可以通过Agent.connectToHub进行绑定
-        HubConnector: the connection between agent and AppHub, you can use 'Agent.connectToHub' to create the connection
+        - HubConnector: 用于和AppHub对接——可以通过Agent.connectToHub进行绑定
+        - HubConnector: the connection between agent and AppHub, you can use 'Agent.connectToHub' to create the connection
         """
 
         self._brain = Brain(self)
         """
-        Agent的大脑
-        The Agent's Brain
+        - Agent的大脑
+        - The Agent's Brain
         """
 
         self._cc = CommandController(self)
         """
-        Agent的命令控制器
-        The Agent's CommondController
+        - Agent的命令控制器
+        - The Agent's CommondController
         """
 
         self._st = StateTransformer()
         """
-        与Agent关联的状态转移器
-        The related StateTransformer
+        - 与Agent关联的状态转移器
+        - The related StateTransformer
         """
 
         self._ac = ActionController(self)
         """
-        Agent的行为控制器
-        The Agent's ActionController
+        - Agent的行为控制器
+        - The Agent's ActionController
         """
 
         self._step_with_action = True
         """
-        Step函数是否包含action执行 —— 当有自定义action需求(特指包含没有指定source的Action)时可置该选项为False并通过自定义方法执行action操作
+        - Step函数是否包含action执行 —— 当有自定义action需求(特指包含没有指定source的Action)时可置该选项为False并通过自定义方法执行action操作
         """
     
     def ConnectToHub(self, config:dict):
         """
         与AppHub构建连接
         Connect to AppHub
 
@@ -150,65 +164,67 @@
             else:
                 print("ERROR: Wrong engine, only baidumap / googlemap are available")
         else:
             print("ERROR: Please provide a streetview engine, baidumap / googlemap")
     
     def enable_streetview(self):
         """
-        开启街景相关功能
-        Enable Streetview function
+        - 开启街景相关功能
+        - Enable Streetview function
         """
         self._brain.Sence.enable_streeview = True
 
     def disable_streetview(self):
         """
-        关闭街景相关功能
-        Disable Streetview function
+        - 关闭街景相关功能
+        - Disable Streetview function
         """
         self._brain.Sence.enable_streeview = False
 
     def enable_user_interaction(self):
         """
-        开启用户交互功能(即在OpenCity控制台中与Agent进行交互)
-        Enable User Interaction function. The User Interaction function is the ability to interact with the related agent in OpenCity website console.
+        - 开启用户交互功能(即在OpenCity控制台中与Agent进行交互)
+        - Enable User Interaction function. The User Interaction function is the ability to interact with the related agent in OpenCity website console.
         """
         self._brain.Memory.Working.enable_user_interaction = True
 
     def disable_user_interaction(self):
         """
-        关闭用户交互功能
-        Disable User Interaction function
+        - 关闭用户交互功能
+        - Disable User Interaction function
         """
         self._brain.Memory.Working.enable_user_interaction = False
 
     def set_step_with_action(self, flag:bool = None):
         """
-        默认情况置反step_with_action属性: 即True->False, False->True
-        否则根据传入的flag进行设置
+        - 默认情况置反step_with_action属性: 即True->False, False->True
+        - 否则根据传入的flag进行设置
         """
         if flag != None:
             self._step_with_action = flag
         else:
             self._step_with_action = not self._step_with_action
         
 
-    def sence_config(self, sence_content:Optional[list]=None, sence_radius:int=None):
+    def sence_config(self, sence_content:Optional[list[str]]=None, sence_radius:int=None):
         '''
         感知配置
+        Sence config
 
         Args:
-        - config: 配置选项——包含需要感知的数据类型
+        - sence_content: 配置选项——包含需要感知的数据类型
             - time: 时间
             - poi: 感兴趣地点
             - position: 可达地点
             - lane: 周围道路
             - person: 周围活动person
             - streetview: 街景
             - user_message: 用户交互信息
             - agent_message: 智能体交互信息
+        - sence_radius (int): 感知半径(m); sence radius
         '''
         if sence_content != None:
             self._brain._sence.set_sence(sence_content)
         if sence_radius != None:
             self._brain._sence.set_sence_radius(sence_radius)
 
     async def Run(self, round:int=1, interval:int=1, log:bool=True):
```

### Comparing `pycityagent-1.1.5/pycityagent/agent_citizen.py` & `pycityagent-1.1.6/pycityagent/agent_citizen.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,108 +1,116 @@
+"""CitizenAgent: 城市居民智能体类及其定义"""
+
 from pycityagent.urbanllm import UrbanLLM
 from .urbanllm import UrbanLLM
 from .agent import Agent, AgentType
 from .image.image import CitizenImage
 
 class CitizenAgent(Agent):
     """
-    Citizen Agent
-    城市居民智能体
+    - Citizen Agent
+    - 城市居民智能体
     """
 
     def __init__(
             self, 
             name:str, 
             server:str, 
             id:int, 
             soul:UrbanLLM=None, 
             simulator=None, 
             base=None,
             motion=None
         ) -> None:
         super().__init__(name, server, AgentType.Citizen, soul, simulator)
         self._id = id
+        """
+        - 智能体ID
+        - Agent's id 
+        """
+
         self.base = base
         """
-        Agent/Person的基本属性, Agent指被代理的Person, Person指模拟器中的背景人
-        The base attributes of Agent/Person. Agent is the Person being represented. Persons are background persons in simulator
+        - Agent/Person的基本属性, Agent指被代理的Person, Person指模拟器中的背景人
+        - The base attributes of Agent/Person. Agent is the Person being represented. Persons are background persons in simulator
         - https://cityproto.sim.fiblab.net/#city.agent.v2.Agent
         """
+
         self.motion = motion
         """
-        Agent/Person的运动信息
-        The motion information of Agent/Person
+        - Agent/Person的运动信息
+        - The motion information of Agent/Person
         - https://cityproto.sim.fiblab.net/#city.agent.v2.AgentMotion
         """
 
         self._image = CitizenImage(self)
         """
-        Agent画像
-        The Agent's Image
+        - Agent画像
+        - The Agent's Image
         """
 
         self.Scheduler.schedule_init()
         """
-        行程初始化
+        - 行程初始化
+        - Schedule Init
         """
 
     def Bind(self):
         """
-        将智能体绑定到AppHub
-        Bind Agent with AppHub
+        - 将智能体绑定到AppHub
+        - Bind Agent with AppHub
         """
         if self._hub_connector == None:
             print("ERROR: connect with apphub first")
         else:
             self._hub_connector.BindCitizenAgent()
 
 
     def enable_economy_behavior(self):
         """
-        开启经济模拟相关功能(例如购物)
-        Enable Economy function. Shopping for instance.
+        - 开启经济模拟相关功能(例如购物)
+        - Enable Economy function. Shopping for instance.
         """
         self.Brain.Memory.Working.enable_economy = True
 
     def disable_economy_behavior(self):
         """
-        关闭经济模拟相关功能
-        Disable Economy function
+        - 关闭经济模拟相关功能
+        - Disable Economy function
         """
         self.Brain.Memory.Working.enable_economy = False
 
     def enable_social_behavior(self):
         """
-        开启社交相关功能
-        Enable Social function
+        - 开启社交相关功能
+        - Enable Social function
         """
         self.Brain.Memory.Working.enable_social = True
 
     def diable_social_behavior(self):
         """
-        关闭社交相关功能
-        Disable Social function
+        - 关闭社交相关功能
+        - Disable Social function
         """
         self.Brain.Memory.Working.enable_social = False
 
     async def Pause(self):
         """
-        暂停Agent行为使Agent进入'pause'状态
-        Pause the Agent, making the agent 'pause'
-
+        - 暂停Agent行为使Agent进入'pause'状态
+        - Pause the Agent, making the agent 'pause'
         """
         req = {'person_id': self.base['id'], 'schedules': []}
         await self._client.person_service.SetSchedule(req)
         self.Scheduler.unset_schedule()
         self._st.trigger('pause')
 
     async def Active(self):
         """
-        恢复Agent行为
-        Recover from 'pause'
+        - 恢复Agent行为
+        - Recover from 'pause'
         """
         self._st.pause_back()
 
     async def Step(self, log:bool):
         """
         单步Agent执行流
         Single step entrance
@@ -129,30 +137,34 @@
                 await self._ac.Run()
         if log:
             print(f"---------------------- SIM TIME: {self._simulator.time} ----------------------")
             self.show_yourself()
     
     def show_yourself(self):
         """
-        Log信息输出
-        Pring log message
+        - Log信息输出
+        - Pring log message
         """
         print(f"【State Message】: {self.state}")
         motion_message = ''''''
         motion_message += f'''行为状态: {self.motion['status']}, '''
         if 'lane_position' in self.motion['position'].keys():
             motion_message += f'''位置信息: lane-{self.motion['position']['lane_position']['lane_id']}'''
         else:
             motion_message += f'''位置信息: aoi-{self.motion['position']['aoi_position']['aoi_id']}'''
         motion_message += f'''-[x: {self.motion['position']['xy_position']['x']}, y: {self.motion['position']['xy_position']['y']}]'''
         print(f'【Simulator Motion Message】: \n{motion_message}')
         print(self.Scheduler)
 
     @property
     def Image(self):
-        """The Agent's Image"""
+        """
+        - The Agent's Image
+        """
         return self._image
 
     @property
     def Scheduler(self):
-        """The Agent's Scheduler"""
+        """
+        - The Agent's Scheduler
+        """
         return self._brain.Memory.Working.scheduler
```

### Comparing `pycityagent-1.1.5/pycityagent/agent_func.py` & `pycityagent-1.1.6/pycityagent/agent_func.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""FuncAgent: 功能性智能体及其定义"""
+
 from pycityagent.urbanllm import UrbanLLM
 from .urbanllm import UrbanLLM
 from .agent import Agent, AgentType
 from .image.image import Image
 from .ac.hub_actions import PositionUpdate
 
 class FuncAgent(Agent):
@@ -14,24 +16,41 @@
             self, 
             name:str, 
             id: int,
             server:str, 
             soul:UrbanLLM=None, 
             simulator=None, 
         ) -> None:
+        """
+        初始化 Init
+
+        Args:
+        - name (str): 智能体名称; name of your agent
+        - id (int): 智能体Id; id of your agent
+        - server (str): 模拟器grpc服务地址; server address of simulator
+        - soul (UrbanLLM): 基础模型模块; base model
+        - simulator (Simulator): 模拟器对象; simulator
+        """
+
         super().__init__(name, server, AgentType.Func, soul, simulator)
         self._id = id
+        """
+        - 智能体Id
+        - Agent's id
+        """
+
         self._image = Image(self)
         """
-        Func Agent画像——支持自定义内容
+        - Func Agent画像——支持自定义内容
         """
 
         self.motion = {'id': id, 'position': {}, 'direction': 0}
         """
         Func Agent状态信息——与agent的sence高度相关
+        Keys:
         - id (int): 即agent id
         - position (https://cityproto.sim.fiblab.net/#city.geo.v2.Position): 即agent当前的位置描述信息
             - lane_position (dict): 当position中包含该key时表示agent当前位于lane上——与aoi_position不可同时存在
                 - lane_id (int)
                 - s (double)
             - aoi_position (dict): 当position中包含该key时表示agent当前位于aoi中——与lane_position不可同时存在
                 - aoi_id (int)
@@ -45,40 +64,40 @@
                 - y (double)
                 - z (double)
         - direction (double): 方向角
         """
 
     async def init_position_aoi(self, aoi_id:int):
         """
-        将agent的位置初始化到指定aoi
-        根据指定aoi设置aoi_position, longlat_position以及xy_position
+        - 将agent的位置初始化到指定aoi
+        - 根据指定aoi设置aoi_position, longlat_position以及xy_position
         """
         if aoi_id in self._simulator.map.aois:
             aoi = self._simulator.map.aois[aoi_id]
             self.motion['position']['aoi_position'] = {'aoi_id': aoi_id}
             self.motion['position']['longlat_position'] = {'longitude': aoi['shapely_lnglat'].centroid.coords[0][0], 'latitude': aoi['shapely_lnglat'].centroid.coords[0][1]}
             x, y = self._simulator.map.lnglat2xy(lng=self.motion['position']['longlat_position']['longitude'], 
                                                  lat=self.motion['position']['longlat_position']['latitude'])
             self.motion['position']['xy_position'] = {'x': x, 'y': y}
         pos = PositionUpdate(self)
         await pos.Forward(longlat=[self.motion['position']['longlat_position']['longitude'], self.motion['position']['longlat_position']['latitude']])
 
     def Bind(self):
         """
-        将智能体绑定到AppHub
-        Bind the Agent with AppHub
+        - 将智能体绑定到AppHub
+        - Bind the Agent with AppHub
         """
         if self._hub_connector == None:
             print("ERROR: connect with apphub first")
         else:
             self._hub_connector.InsertFuncAgent()
 
     def set_image(self, image: Image):
         """
-        设置image——支持自由扩展Image
+        - 设置image——支持自由扩展Image
         """
         self._image = image
 
     async def Step(self, log:bool):
         """
         单步Agent执行流
         Single step entrance
@@ -100,16 +119,18 @@
             await self._ac.Run()
         if log:
             print(f"---------------------- SIM TIME: {self._simulator.time} ----------------------")
             self.show_yourself()
     
     def show_yourself(self):
         """
-        Log信息输出
-        Pring log message
+        - Log信息输出
+        - Pring log message
         """
         pass
 
     @property
     def Image(self):
-        """The Agent's Image"""
+        """
+        - The Agent's Image
+        """
         return self._image
```

### Comparing `pycityagent-1.1.5/pycityagent/brain/brain.py` & `pycityagent-1.1.6/pycityagent/brain/brain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+"""大脑类"""
 from abc import ABC, abstractmethod
 from typing import Optional
 from .scheduler import Scheduler
 from .sence import Sence
 from .memory import MemoryController
 
 class Brain:
     """
-    大脑模块
-    Brain Module
+    大脑类
+    Brain Class
     """
     def __init__(self, agent) -> None:
         self._agent = agent
         self._simulator = agent._simulator
         self._sence = Sence(agent)
         """
         感知模块
```

### Comparing `pycityagent-1.1.5/pycityagent/brain/memory.py` & `pycityagent-1.1.6/pycityagent/brain/memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""记忆相关类与定义"""
+
 from typing import Any, Optional
 from abc import ABC, abstractmethod
 from enum import Enum
 import json
 from collections import defaultdict
 from .brainfc import BrainFunction
 from .scheduler import Scheduler
@@ -57,18 +59,20 @@
     def MemoryLoad(self, x):
         """
         记忆恢复
         Load Memory
         """
 
 class WMemory(Memory):
+    """WMemory: Working Memory工作记忆类"""
     def __init__(self, agent) -> None:
         super().__init__(agent, MemoryType.WM)
 
 class LTMemory(Memory):
+    """LTMemory: Long-Term Memory长时记忆类"""
     def __init__(self, agent) -> None:
         super().__init__(agent, MemoryType.LTM)
 
 class MemoryRetrive:
     """
     用于从LTM中获取对应信息
     LTM retrive: get information from LTM
```

### Comparing `pycityagent-1.1.5/pycityagent/brain/persistence/spatial.py` & `pycityagent-1.1.6/pycityagent/brain/persistence/spatial.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.5/pycityagent/brain/reason/shop.py` & `pycityagent-1.1.6/pycityagent/brain/reason/shop.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.5/pycityagent/brain/reason/social.py` & `pycityagent-1.1.6/pycityagent/brain/reason/social.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.5/pycityagent/brain/reason/trip.py` & `pycityagent-1.1.6/pycityagent/brain/reason/trip.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.5/pycityagent/brain/reason/user.py` & `pycityagent-1.1.6/pycityagent/brain/reason/user.py`

 * *Files identical despite different names*

### Comparing `pycityagent-1.1.5/pycityagent/brain/scheduler.py` & `pycityagent-1.1.6/pycityagent/brain/scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""规划器相关类及定义"""
+
 from enum import Enum
 import random
 import time as Time
 import json
 from .brainfc import BrainFunction
 from pycitysim.apphub import AgentMessage
 
@@ -17,14 +19,15 @@
         - Other: 其他规划. Other Schedule
     """
     TRIP = 1
     SHOP = 2
     OTHER = 3
 
 class Schedule:
+    """Schedule基类——为多种Schedule提供基础模板"""
     def __init__(self, type) -> None:
         '''默认初始化'''
         self.type = type
 
 class TripSchedule(Schedule):
     """
     出行规划
```

### Comparing `pycityagent-1.1.5/pycityagent/brain/sence.py` & `pycityagent-1.1.6/pycityagent/brain/sence.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""大脑感知相关类及其定义"""
+
 from typing import Optional, Union
 from datetime import datetime
 import math
 import copy
 from pycitysim.apphub import UserMessage, AgentMessage
 from citystreetview import (
     BaiduStreetView,
@@ -331,15 +333,15 @@
                     'xy': (walking_gates[i]['x'], walking_gates[i]['y']),
                     'longlat': longlat,
                     'type': 'walking'
                 })
         else:
             # agent in lane
             lane_id = self._agent.motion['position']['lane_position']['lane_id']  # 所在lane_id
-            lane = copy.deepcopy(self._agnet._simualtor.map.get_lane(lane_id))  # 获取lane信息
+            lane = copy.deepcopy(self._agent._simulator.map.get_lane(lane_id))  # 获取lane信息
             agent_s = self._agent.motion['position']['lane_position']['s']  # 所处位置——用s距离表示
             nodes = lane['center_line']['nodes']
             if agent_s == 0:
                 # 处于当前道路的首部端点位置
                 # 1. 当前道路
                 tmp_s = radius_
                 tmp_s = tmp_s if tmp_s <= lane['length'] else lane['length']
@@ -370,15 +372,15 @@
                                    'type': type}]
             elif agent_s == lane['length']:
                 # 处于当前道路的尾部端点位置
                 # 1. 当前道路
                 tmp_s = agent_s - radius_
                 tmp_s = tmp_s if tmp_s >= 0 else 0
                 x, y = get_xy_in_lane(nodes, tmp_s, 'back')
-                longlat = self._agent._simulator.map.xy2loglat(x=x, y=y)
+                longlat = self._agent._simulator.map.xy2lnglat(x=x, y=y)
                 type = self._lane_type_mapping.get(lane['type'], 'unspecified')
                 positions += [{'lane_id': lane_id, 
                                's': tmp_s, 
                                'xy': (x, y),
                                'longlat': longlat, 
                                'type': type}]
 
@@ -387,38 +389,38 @@
                 for suc_lane in suc_lanes:
                     suc_lane_id = suc_lane['id']
                     suc_lane_ = copy.deepcopy(self._agent._simulator.map.get_lane(suc_lane_id))
                     suc_lane_nodes = suc_lane_['center_line']['nodes']
                     tmp_s = radius_
                     tmp_s = tmp_s if tmp_s <= suc_lane_['length'] else suc_lane_['length']
                     x, y = get_xy_in_lane(suc_lane_nodes, tmp_s)
-                    longlat = self._agent._simulator.map.xy2loglat(x=x, y=y)
+                    longlat = self._agent._simulator.map.xy2lnglat(x=x, y=y)
                     type = self._lane_type_mapping.get(lane['type'], 'unspecified')
                     positions += [{'lane_id': suc_lane_id, 
                                    's': tmp_s, 
                                    'xy': (x, y),
                                    'longlat': longlat, 
                                    'type': type}]
             else:
                 # 非端点位置
                 neg_s = agent_s - radius_
                 neg_s = neg_s if neg_s >= 0 else 0
                 x, y = get_xy_in_lane(nodes, neg_s, 'back')
-                longlat = self._agent._simulator.map.xy2loglat(x=x, y=y)
+                longlat = self._agent._simulator.map.xy2lnglat(x=x, y=y)
                 type = self._lane_type_mapping.get(lane['type'], 'unspecified')
                 positions += [{'lans_id': lane_id, 
                                's': neg_s, 
                                'xy': (x, y),
                                'longlat': longlat, 
                                'type': type}]
 
                 pos_s = agent_s + radius_
                 pos_s = pos_s if pos_s <= lane['length'] else lane['length']
                 x, y = get_xy_in_lane(nodes, pos_s)
-                longlat = self._agent._simulator.map.xy2loglat(x=x, y=y)
+                longlat = self._agent._simulator.map.xy2lnglat(x=x, y=y)
                 type = self._lane_type_mapping.get(lane['type'], 'unspecified')
                 positions += [{'lans_id': lane_id, 
                                's': neg_s, 
                                'xy': (x, y),
                                'longlat': longlat, 
                                'type': type}]
         return positions
```

### Comparing `pycityagent-1.1.5/pycityagent/brain/static.py` & `pycityagent-1.1.6/pycityagent/brain/static.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Static Resources: Poi Type association; Type prefix.
+静态数据支持; Static Resources: Poi Type association; Type prefix.
 """
 POI_TYPE_DICT = {
     "100000": "\u7f8e\u98df",
     "101000": "\u7f8e\u98df:\u4e2d\u9910\u5385",
     "101010": "\u7f8e\u98df:\u4e2d\u9910\u5385:\u5317\u4eac\u83dc",
     "101011": "\u7f8e\u98df:\u4e2d\u9910\u5385:\u5b89\u5fbd\u83dc",
     "101012": "\u7f8e\u98df:\u4e2d\u9910\u5385:\u5c71\u897f\u83dc",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pycityagent-1.1.5/pycityagent/cc/cc.py` & `pycityagent-1.1.6/pycityagent/cc/cc.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""命令控制器定义"""
+
 from typing import Any
 from .idle import *
 from .shop import *
 from .trip import *
 from .conve import *
 from .user import *
```

### Comparing `pycityagent-1.1.5/pycityagent/hubconnector/hubconnector.py` & `pycityagent-1.1.6/pycityagent/hubconnector/hubconnector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""Apphub客户端定义"""
+
 from typing import Optional
 import geojson
 from pycitysim.apphub import AppHubClient, AgentMessage, UserMessage
 import PIL.Image as Image
 import traceback
 
 class HubConnector:
```

### Comparing `pycityagent-1.1.5/pycityagent/image/image.py` & `pycityagent-1.1.6/pycityagent/image/image.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""智能体画像类及其定义"""
+
 from typing import Optional
 import json
 from abc import ABC, abstractclassmethod
 
 
 class Image:
     """
@@ -95,14 +97,15 @@
 
         Args:
         - selfie_file (str): the path of selfie_file
         """
         print("Not Implemented")
 
 class Scratch:
+    """智能体基础信息"""
     def __init__(self, scratch: Optional[dict]=None) -> None:
         if scratch != None:
             self.forward(scratch)
 
     def forward(self, x:dict):
         """Scratch记忆更新"""
         for k in x.keys():
@@ -123,14 +126,15 @@
     def get_profile_content(self):
         text = ""
         for attr_name, attr_value in self.__dict__.items():
             text += f"{attr_name}: {attr_value}\n"
         return text
 
 class CitizenScratch(Scratch):
+    """CitizenAgent基础信息"""
     def __init__(self, scratch:Optional[dict]=None) -> None:
         super().__init__(scratch=scratch)
         self.name = None
         self.age = None
         self.education = None
         self.gender = None
         self.consumption = None
```

### Comparing `pycityagent-1.1.5/pycityagent/simulator.py` & `pycityagent-1.1.6/pycityagent/simulator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,56 +1,87 @@
-from pycitysim import *
-from pycitysim.routing import RoutingClient
-from pycitysim.sim import CityClient
+"""Simulator: 城市模拟器类及其定义"""
+
 from typing import Optional, Union
 from datetime import datetime, timedelta
 import asyncio
+from pycitysim import *
+from pycitysim.routing import RoutingClient
+from pycitysim.sim import CityClient
 from .agent_citizen import CitizenAgent
 from .agent_func import FuncAgent
 
 class SimPerceive:
     """
-    模拟器感知
-    Simulator Perceive
+    - 模拟器感知
+    - Simulator Perceive
     """
     def __init__(self, simualtor) -> None:
         self._simulator=simualtor
     
     async def PerceiveAoisByIds(self, ids:Optional[list[int]]):
         """
-        Simulator视角下的AOI感知
-        Perceive AOI from Simulator
+        - Simulator视角下的AOI感知
+        - Perceive AOI from Simulator
 
         Args:
         - ids list[int]: list of aoi id
 
         Returns:
         - https://cityproto.sim.fiblab.net/#city.map.v2.GetAoiResponse
         """
         req = {'aoi_ids': ids}
         resp = await self._simulator._client.aoi_service.GetAoi(req)
         return resp
 
 class Simulator:
     """
-    模拟器
-    Simulator
+    - 模拟器主类
+    - Simulator Class
     """
     def __init__(self, config) -> None:
         self.config = config
+        """
+        - 模拟器配置
+        - simulator config
+        """
+
         self._client = CityClient(self.config['simulator']['server'], secure=True)
+        """
+        - 模拟器grpc客户端
+        - grpc client of simulator
+        """
+
         self._perceive = SimPerceive(self)
+        """
+        - 模拟器感知
+        - Perceive of simulator
+        """
+
         self.map = map.Map(
             mongo_uri = "mongodb://sim:FiblabSim1001@mgo.db.fiblab.tech:8635/",
             mongo_db = "srt",
             mongo_coll = config['map_request']['mongo_coll'],
             cache_dir = config['map_request']['cache_dir'],
         )
+        """
+        - 模拟器地图对象
+        - Simulator map object
+        """
+
         self.routing = RoutingClient(self.config['route_request']['server'])
+        """
+        - 导航服务grpc客户端
+        - grpc client of routing service
+        """
+
         self.time = 0
+        """
+        - 模拟城市当前时间
+        - The current time of simulator
+        """
 
     # * Agent相关
     def FindAgentsByArea(self, req: dict, status=None):
         """
         通过区域范围查找agent/person
         Get agents/persons in the provided area
```

### Comparing `pycityagent-1.1.5/pycityagent/st/st.py` & `pycityagent-1.1.6/pycityagent/st/st.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""StateTransformer: 状态控制器类及其定义"""
+
 from transitions import Machine
 from abc import ABC, abstractmethod
 
 class StateTransformer:
     """
     默认State Transformer模块: 控制agent状态转移
     Default State Transformer module: used to control the transformation of agent's state
```

### Comparing `pycityagent-1.1.5/pycityagent/urbanllm/urbanllm.py` & `pycityagent-1.1.6/pycityagent/urbanllm/urbanllm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+"""UrbanLLM: 智能能力类及其定义"""
+
 from openai import OpenAI
 from http import HTTPStatus
 import dashscope
 from urllib.parse import urlparse, unquote
 from pathlib import PurePosixPath
 import requests
 from dashscope import ImageSynthesis
```

### Comparing `pycityagent-1.1.5/pycityagent.egg-info/PKG-INFO` & `pycityagent-1.1.6/pycityagent.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycityagent
-Version: 1.1.5
+Version: 1.1.6
 Summary: LLM-based城市模拟器agent构建库
 Author-email: Yuwei Yan <pinkgranite86@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 FIBLAB
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `pycityagent-1.1.5/pycityagent.egg-info/SOURCES.txt` & `pycityagent-1.1.6/pycityagent.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,21 +11,16 @@
 pycityagent.egg-info/dependency_links.txt
 pycityagent.egg-info/requires.txt
 pycityagent.egg-info/top_level.txt
 pycityagent/ac/__init__.py
 pycityagent/ac/ac.py
 pycityagent/ac/action.py
 pycityagent/ac/action_stream.py
-pycityagent/ac/controled.py
-pycityagent/ac/converse.py
 pycityagent/ac/hub_actions.py
-pycityagent/ac/idle.py
-pycityagent/ac/shop.py
 pycityagent/ac/sim_actions.py
-pycityagent/ac/trip.py
 pycityagent/ac/citizen_actions/controled.py
 pycityagent/ac/citizen_actions/converse.py
 pycityagent/ac/citizen_actions/idle.py
 pycityagent/ac/citizen_actions/shop.py
 pycityagent/ac/citizen_actions/trip.py
 pycityagent/brain/__init__.py
 pycityagent/brain/brain.py
```

### Comparing `pycityagent-1.1.5/pyproject.toml` & `pycityagent-1.1.6/pyproject.toml`

 * *Files identical despite different names*

