# Comparing `tmp/nonebot-plugin-fishing-0.2.3a1.tar.gz` & `tmp/nonebot-plugin-fishing-0.2.3a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot-plugin-fishing-0.2.3a1.tar", last modified: Tue Apr  9 14:32:26 2024, max compression
+gzip compressed data, was "nonebot-plugin-fishing-0.2.3a2.tar", last modified: Sat Apr 13 01:33:13 2024, max compression
```

## Comparing `nonebot-plugin-fishing-0.2.3a1.tar` & `nonebot-plugin-fishing-0.2.3a2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:32:26.035735 nonebot-plugin-fishing-0.2.3a1/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-09 14:32:26.035735 nonebot-plugin-fishing-0.2.3a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:32:26.035735 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/data_source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:32:26.035735 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/migrations/68463f3e5f33_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/migrations/da5a91612ef2_init_db.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 14:32:26.035735 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-04-09 14:32:26.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-04-09 14:32:26.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 14:32:26.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-09 14:32:26.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-09 14:32:26.000000 nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-09 14:32:21.000000 nonebot-plugin-fishing-0.2.3a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-09 14:32:26.035735 nonebot-plugin-fishing-0.2.3a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:33:13.770884 nonebot-plugin-fishing-0.2.3a2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-13 01:33:13.770884 nonebot-plugin-fishing-0.2.3a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:33:13.766884 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/data_source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:33:13.770884 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/migrations/68463f3e5f33_update_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/migrations/7609e6d106dd_init_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 01:33:13.770884 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3448 2024-04-13 01:33:13.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-13 01:33:13.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 01:33:13.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-13 01:33:13.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-13 01:33:13.000000 nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-13 01:33:10.000000 nonebot-plugin-fishing-0.2.3a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 01:33:13.770884 nonebot-plugin-fishing-0.2.3a2/setup.cfg
```

### Comparing `nonebot-plugin-fishing-0.2.3a1/LICENSE` & `nonebot-plugin-fishing-0.2.3a2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fishing-0.2.3a1/PKG-INFO` & `nonebot-plugin-fishing-0.2.3a2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fishing
-Version: 0.2.3a1
+Version: 0.2.3a2
 Summary: 你甚至可以电子钓鱼
 Author-email: C14H22O <160833462+C14H22O@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2>=2.2.1
@@ -85,15 +85,29 @@
 
 | 配置项 | 必填 | 说明 |
 |:-----:|:----:|:----:|
 | fishes | 否 | 配置鱼塘内鱼们的名称、权重、等待时间和价格 |
 | fishing_limit | 否 | 填入每次钓鱼后，限制钓鱼的秒数 |
 | fishing_coin_name | 否 | 填入卖鱼获取的货币名称 |
 
+其中 `fishes` 配置项说明如下：
+
+```dotenv
+{
+    "name": "小鱼", # 鱼的名称
+    "frequency": 2, # 鱼上钩的时间
+    "weight": 100, # 权重
+    "price": 2 # 价格
+}
+```
+
+
+
 ## 🎉 使用
+
 ### 指令表
 | 指令 | 范围 | 说明 |
 |:-----:|:----:|:----:|
 | 钓鱼 | 所有 | 放下鱼竿 |
 | 统计信息 | 所有 | 查看钓鱼次数 |
 | 背包 | 所有 | 查看背包 |
 | 卖鱼 | 所有 | 卖鱼 |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.3a1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.3a2 Summary:
 ä½ çè³å¯ä»¥çµå­éé±¼ Author-email: C14H22O
 <160833462+C14H22O@users.noreply.github.com> License: MIT Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: nonebot2>=2.2.1 Requires-Dist: pydantic>=1.10 Requires-Dist: nonebot-
 plugin-localstore>=0.6.0 Requires-Dist: sqlalchemy>=2.0.27 Requires-Dist:
 aiosqlite>=0.20.0 Requires-Dist: nonebot-plugin-orm>=0.7.1
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
@@ -19,16 +19,19 @@
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot_plugin_fishing"] æ³¨æï¼å®è£è¿åï¼éå¨æ§å¶å°è¾å¥ `nb
 orm upgrade` æä»¤ä»¥åå§åæ°æ®åºã ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 è¯´æ | |:-----:|:----:|:----:| | fishes | å¦ |
 éç½®é±¼å¡åé±¼ä»¬çåç§°ãæéãç­å¾æ¶é´åä»·æ ¼ | |
 fishing_limit | å¦ | å¡«å¥æ¯æ¬¡éé±¼åï¼éå¶éé±¼çç§æ° | |
-fishing_coin_name | å¦ | å¡«å¥åé±¼è·åçè´§å¸åç§° | ## ð ä½¿ç¨
-### æä»¤è¡¨ | æä»¤ | èå´ | è¯´æ | |:-----:|:----:|:----:| | éé±¼ |
-ææ | æ¾ä¸é±¼ç«¿ | | ç»è®¡ä¿¡æ¯ | ææ | æ¥çéé±¼æ¬¡æ° | | èå
-| ææ | æ¥çèå | | åé±¼ | ææ | åé±¼ | ## ð Todo - [x]
-éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨ [nonebot/plugin-orm](https://github.com/
-nonebot/plugin-orm)ï¼ - [x] å¢å ç³»ç»ååºï¼ååºéå°çé±¼ä»¬ - [ ]
-èµåæ¾ç [#4](https://github.com/C14H22O/nonebot-plugin-fishing/issues/4) -
-[ ] ä¸ºé±¼ç«¿å¢å èä¹åº¦ï¼èä¹åº¦ä¸º0æ¶ééæ°è´­ä¹°é±¼ç«¿ - [ ]
+fishing_coin_name | å¦ | å¡«å¥åé±¼è·åçè´§å¸åç§° | å¶ä¸­ `fishes`
+éç½®é¡¹è¯´æå¦ä¸ï¼ ```dotenv { "name": "å°é±¼", # é±¼çåç§°
+"frequency": 2, # é±¼ä¸é©çæ¶é´ "weight": 100, # æé "price": 2 #
+ä»·æ ¼ } ``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | èå´ | è¯´æ | |:-----:
+|:----:|:----:| | éé±¼ | ææ | æ¾ä¸é±¼ç«¿ | | ç»è®¡ä¿¡æ¯ | ææ |
+æ¥çéé±¼æ¬¡æ° | | èå | ææ | æ¥çèå | | åé±¼ | ææ |
+åé±¼ | ## ð Todo - [x] éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨ [nonebot/
+plugin-orm](https://github.com/nonebot/plugin-orm)ï¼ - [x]
+å¢å ç³»ç»ååºï¼ååºéå°çé±¼ä»¬ - [ ] èµåæ¾ç [#4](https://
+github.com/C14H22O/nonebot-plugin-fishing/issues/4) - [ ]
+ä¸ºé±¼ç«¿å¢å èä¹åº¦ï¼èä¹åº¦ä¸º0æ¶ééæ°è´­ä¹°é±¼ç«¿ - [ ]
 ä¸ºéé±¼èåæ·»å æåº - [ ] æ·»å æå°±ç³»ç»
```

### Comparing `nonebot-plugin-fishing-0.2.3a1/README.md` & `nonebot-plugin-fishing-0.2.3a2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -69,15 +69,29 @@
 
 | 配置项 | 必填 | 说明 |
 |:-----:|:----:|:----:|
 | fishes | 否 | 配置鱼塘内鱼们的名称、权重、等待时间和价格 |
 | fishing_limit | 否 | 填入每次钓鱼后，限制钓鱼的秒数 |
 | fishing_coin_name | 否 | 填入卖鱼获取的货币名称 |
 
+其中 `fishes` 配置项说明如下：
+
+```dotenv
+{
+    "name": "小鱼", # 鱼的名称
+    "frequency": 2, # 鱼上钩的时间
+    "weight": 100, # 权重
+    "price": 2 # 价格
+}
+```
+
+
+
 ## 🎉 使用
+
 ### 指令表
 | 指令 | 范围 | 说明 |
 |:-----:|:----:|:----:|
 | 钓鱼 | 所有 | 放下鱼竿 |
 | 统计信息 | 所有 | 查看钓鱼次数 |
 | 背包 | 所有 | 查看背包 |
 | 卖鱼 | 所有 | 卖鱼 |
```

#### html2text {}

```diff
@@ -12,16 +12,19 @@
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot_plugin_fishing"] æ³¨æï¼å®è£è¿åï¼éå¨æ§å¶å°è¾å¥ `nb
 orm upgrade` æä»¤ä»¥åå§åæ°æ®åºã ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 è¯´æ | |:-----:|:----:|:----:| | fishes | å¦ |
 éç½®é±¼å¡åé±¼ä»¬çåç§°ãæéãç­å¾æ¶é´åä»·æ ¼ | |
 fishing_limit | å¦ | å¡«å¥æ¯æ¬¡éé±¼åï¼éå¶éé±¼çç§æ° | |
-fishing_coin_name | å¦ | å¡«å¥åé±¼è·åçè´§å¸åç§° | ## ð ä½¿ç¨
-### æä»¤è¡¨ | æä»¤ | èå´ | è¯´æ | |:-----:|:----:|:----:| | éé±¼ |
-ææ | æ¾ä¸é±¼ç«¿ | | ç»è®¡ä¿¡æ¯ | ææ | æ¥çéé±¼æ¬¡æ° | | èå
-| ææ | æ¥çèå | | åé±¼ | ææ | åé±¼ | ## ð Todo - [x]
-éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨ [nonebot/plugin-orm](https://github.com/
-nonebot/plugin-orm)ï¼ - [x] å¢å ç³»ç»ååºï¼ååºéå°çé±¼ä»¬ - [ ]
-èµåæ¾ç [#4](https://github.com/C14H22O/nonebot-plugin-fishing/issues/4) -
-[ ] ä¸ºé±¼ç«¿å¢å èä¹åº¦ï¼èä¹åº¦ä¸º0æ¶ééæ°è´­ä¹°é±¼ç«¿ - [ ]
+fishing_coin_name | å¦ | å¡«å¥åé±¼è·åçè´§å¸åç§° | å¶ä¸­ `fishes`
+éç½®é¡¹è¯´æå¦ä¸ï¼ ```dotenv { "name": "å°é±¼", # é±¼çåç§°
+"frequency": 2, # é±¼ä¸é©çæ¶é´ "weight": 100, # æé "price": 2 #
+ä»·æ ¼ } ``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | èå´ | è¯´æ | |:-----:
+|:----:|:----:| | éé±¼ | ææ | æ¾ä¸é±¼ç«¿ | | ç»è®¡ä¿¡æ¯ | ææ |
+æ¥çéé±¼æ¬¡æ° | | èå | ææ | æ¥çèå | | åé±¼ | ææ |
+åé±¼ | ## ð Todo - [x] éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨ [nonebot/
+plugin-orm](https://github.com/nonebot/plugin-orm)ï¼ - [x]
+å¢å ç³»ç»ååºï¼ååºéå°çé±¼ä»¬ - [ ] èµåæ¾ç [#4](https://
+github.com/C14H22O/nonebot-plugin-fishing/issues/4) - [ ]
+ä¸ºé±¼ç«¿å¢å èä¹åº¦ï¼èä¹åº¦ä¸º0æ¶ééæ°è´­ä¹°é±¼ç«¿ - [ ]
 ä¸ºéé±¼èåæ·»å æåº - [ ] æ·»å æå°±ç³»ç»
```

### Comparing `nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/__init__.py` & `nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/config.py` & `nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/config.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/data_source.py` & `nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/data_source.py`

 * *Files identical despite different names*

### Comparing `nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing/migrations/68463f3e5f33_.py` & `nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing/migrations/7609e6d106dd_init_db.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,47 +1,44 @@
-"""empty message
+"""init db
 
-迁移 ID: 68463f3e5f33
-父迁移: da5a91612ef2
-创建时间: 2024-04-09 14:24:27.354048
+迁移 ID: 7609e6d106dd
+父迁移: 
+创建时间: 2024-04-05 19:08:58.835014
 
 """
 from __future__ import annotations
 
 from collections.abc import Sequence
 
 from alembic import op
 import sqlalchemy as sa
 
 
-revision: str = '68463f3e5f33'
-down_revision: str | Sequence[str] | None = 'da5a91612ef2'
-branch_labels: str | Sequence[str] | None = None
+revision: str = '7609e6d106dd'
+down_revision: str | Sequence[str] | None = None
+branch_labels: str | Sequence[str] | None = ('nonebot_plugin_fishing',)
 depends_on: str | Sequence[str] | None = None
 
 
 def upgrade(name: str = "") -> None:
     if name:
         return
     # ### commands auto generated by Alembic - please adjust! ###
-    with op.batch_alter_table('nonebot_plugin_fishing_fishingrecord', schema=None) as batch_op:
-        batch_op.add_column(sa.Column('coin', sa.Integer(), nullable=False))
-        batch_op.alter_column('fishes',
-               existing_type=sa.VARCHAR(),
-               type_=sa.TEXT(),
-               existing_nullable=False)
-
+    op.create_table('nonebot_plugin_fishing_fishingrecord',
+    sa.Column('id', sa.Integer(), nullable=False),
+    sa.Column('user_id', sa.String(length=32), nullable=False),
+    sa.Column('time', sa.Integer(), nullable=False),
+    sa.Column('frequency', sa.Integer(), nullable=False),
+    sa.Column('fishes', sa.TEXT(), nullable=False),
+    sa.Column('coin', sa.Integer(), nullable=False),
+    sa.PrimaryKeyConstraint('id', name=op.f('pk_nonebot_plugin_fishing_fishingrecord')),
+    info={'bind_key': 'nonebot_plugin_fishing'}
+    )
     # ### end Alembic commands ###
 
 
 def downgrade(name: str = "") -> None:
     if name:
         return
     # ### commands auto generated by Alembic - please adjust! ###
-    with op.batch_alter_table('nonebot_plugin_fishing_fishingrecord', schema=None) as batch_op:
-        batch_op.alter_column('fishes',
-               existing_type=sa.TEXT(),
-               type_=sa.VARCHAR(),
-               existing_nullable=False)
-        batch_op.drop_column('coin')
-
-    # ### end Alembic commands ###
+    op.drop_table('nonebot_plugin_fishing_fishingrecord')
+    # ### end Alembic commands ###
```

### Comparing `nonebot-plugin-fishing-0.2.3a1/nonebot_plugin_fishing.egg-info/PKG-INFO` & `nonebot-plugin-fishing-0.2.3a2/nonebot_plugin_fishing.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-fishing
-Version: 0.2.3a1
+Version: 0.2.3a2
 Summary: 你甚至可以电子钓鱼
 Author-email: C14H22O <160833462+C14H22O@users.noreply.github.com>
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2>=2.2.1
@@ -85,15 +85,29 @@
 
 | 配置项 | 必填 | 说明 |
 |:-----:|:----:|:----:|
 | fishes | 否 | 配置鱼塘内鱼们的名称、权重、等待时间和价格 |
 | fishing_limit | 否 | 填入每次钓鱼后，限制钓鱼的秒数 |
 | fishing_coin_name | 否 | 填入卖鱼获取的货币名称 |
 
+其中 `fishes` 配置项说明如下：
+
+```dotenv
+{
+    "name": "小鱼", # 鱼的名称
+    "frequency": 2, # 鱼上钩的时间
+    "weight": 100, # 权重
+    "price": 2 # 价格
+}
+```
+
+
+
 ## 🎉 使用
+
 ### 指令表
 | 指令 | 范围 | 说明 |
 |:-----:|:----:|:----:|
 | 钓鱼 | 所有 | 放下鱼竿 |
 | 统计信息 | 所有 | 查看钓鱼次数 |
 | 背包 | 所有 | 查看背包 |
 | 卖鱼 | 所有 | 卖鱼 |
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.3a1 Summary:
+Metadata-Version: 2.1 Name: nonebot-plugin-fishing Version: 0.2.3a2 Summary:
 ä½ çè³å¯ä»¥çµå­éé±¼ Author-email: C14H22O
 <160833462+C14H22O@users.noreply.github.com> License: MIT Requires-Python:
 >=3.8 Description-Content-Type: text/markdown License-File: LICENSE Requires-
 Dist: nonebot2>=2.2.1 Requires-Dist: pydantic>=1.10 Requires-Dist: nonebot-
 plugin-localstore>=0.6.0 Requires-Dist: sqlalchemy>=2.0.27 Requires-Dist:
 aiosqlite>=0.20.0 Requires-Dist: nonebot-plugin-orm>=0.7.1
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
@@ -19,16 +19,19 @@
 `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
 ["nonebot_plugin_fishing"] æ³¨æï¼å®è£è¿åï¼éå¨æ§å¶å°è¾å¥ `nb
 orm upgrade` æä»¤ä»¥åå§åæ°æ®åºã ## âï¸ éç½® å¨ nonebot2
 é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 è¯´æ | |:-----:|:----:|:----:| | fishes | å¦ |
 éç½®é±¼å¡åé±¼ä»¬çåç§°ãæéãç­å¾æ¶é´åä»·æ ¼ | |
 fishing_limit | å¦ | å¡«å¥æ¯æ¬¡éé±¼åï¼éå¶éé±¼çç§æ° | |
-fishing_coin_name | å¦ | å¡«å¥åé±¼è·åçè´§å¸åç§° | ## ð ä½¿ç¨
-### æä»¤è¡¨ | æä»¤ | èå´ | è¯´æ | |:-----:|:----:|:----:| | éé±¼ |
-ææ | æ¾ä¸é±¼ç«¿ | | ç»è®¡ä¿¡æ¯ | ææ | æ¥çéé±¼æ¬¡æ° | | èå
-| ææ | æ¥çèå | | åé±¼ | ææ | åé±¼ | ## ð Todo - [x]
-éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨ [nonebot/plugin-orm](https://github.com/
-nonebot/plugin-orm)ï¼ - [x] å¢å ç³»ç»ååºï¼ååºéå°çé±¼ä»¬ - [ ]
-èµåæ¾ç [#4](https://github.com/C14H22O/nonebot-plugin-fishing/issues/4) -
-[ ] ä¸ºé±¼ç«¿å¢å èä¹åº¦ï¼èä¹åº¦ä¸º0æ¶ééæ°è´­ä¹°é±¼ç«¿ - [ ]
+fishing_coin_name | å¦ | å¡«å¥åé±¼è·åçè´§å¸åç§° | å¶ä¸­ `fishes`
+éç½®é¡¹è¯´æå¦ä¸ï¼ ```dotenv { "name": "å°é±¼", # é±¼çåç§°
+"frequency": 2, # é±¼ä¸é©çæ¶é´ "weight": 100, # æé "price": 2 #
+ä»·æ ¼ } ``` ## ð ä½¿ç¨ ### æä»¤è¡¨ | æä»¤ | èå´ | è¯´æ | |:-----:
+|:----:|:----:| | éé±¼ | ææ | æ¾ä¸é±¼ç«¿ | | ç»è®¡ä¿¡æ¯ | ææ |
+æ¥çéé±¼æ¬¡æ° | | èå | ææ | æ¥çèå | | åé±¼ | ææ |
+åé±¼ | ## ð Todo - [x] éåæ°æ®åºé»è¾ï¼æ¹ä¸ºä½¿ç¨ [nonebot/
+plugin-orm](https://github.com/nonebot/plugin-orm)ï¼ - [x]
+å¢å ç³»ç»ååºï¼ååºéå°çé±¼ä»¬ - [ ] èµåæ¾ç [#4](https://
+github.com/C14H22O/nonebot-plugin-fishing/issues/4) - [ ]
+ä¸ºé±¼ç«¿å¢å èä¹åº¦ï¼èä¹åº¦ä¸º0æ¶ééæ°è´­ä¹°é±¼ç«¿ - [ ]
 ä¸ºéé±¼èåæ·»å æåº - [ ] æ·»å æå°±ç³»ç»
```

