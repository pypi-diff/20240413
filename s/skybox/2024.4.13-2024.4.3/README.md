# Comparing `tmp/skybox-2024.4.13.tar.gz` & `tmp/skybox-2024.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skybox-2024.4.13.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "skybox-2024.4.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skybox-2024.4.13.tar` & `skybox-2024.4.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 skybox-2024.4.13/Copyright
--rw-r--r--   0        0        0      735 2024-02-25 06:24:00.741491 skybox-2024.4.13/README.md
--rw-r--r--   0        0        0      321 2024-04-13 08:32:12.081508 skybox-2024.4.13/pyproject.toml
--rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 skybox-2024.4.13/skybox/Copyright
--rw-r--r--   0        0        0      156 2024-02-25 06:24:00.741491 skybox-2024.4.13/skybox/__init__.py
--rw-r--r--   0        0        0    13076 2024-04-13 08:31:48.882043 skybox-2024.4.13/skybox/files_hashes
--rw-r--r--   0        0        0      936 1970-01-01 00:00:00.000000 skybox-2024.4.13/PKG-INFO
+-rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 skybox-2024.4.3/Copyright
+-rw-r--r--   0        0        0      735 2024-02-25 06:24:00.741491 skybox-2024.4.3/README.md
+-rw-r--r--   0        0        0      320 2024-04-03 06:26:06.014092 skybox-2024.4.3/pyproject.toml
+-rw-r--r--   0        0        0      231 2024-02-25 03:34:44.558335 skybox-2024.4.3/skybox/Copyright
+-rw-r--r--   0        0        0      156 2024-02-25 06:24:00.741491 skybox-2024.4.3/skybox/__init__.py
+-rw-r--r--   0        0        0    12359 2024-04-03 06:25:47.716340 skybox-2024.4.3/skybox/files_hashes
+-rw-r--r--   0        0        0      935 1970-01-01 00:00:00.000000 skybox-2024.4.3/PKG-INFO
```

### Comparing `skybox-2024.4.13/README.md` & `skybox-2024.4.3/README.md`

 * *Files identical despite different names*

### Comparing `skybox-2024.4.13/skybox/files_hashes` & `skybox-2024.4.3/skybox/files_hashes`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,19 @@
     arts -2024.1.17.zip                        -info {"size": 571603, "sha-512": "327342199a59a3678a8e09e3706a7885b0ad83ebd3c3183f74b7c95ce6e5e6350dad1a26ce32cdc08c3b2fee2e7f467000c571a4e366002063a683076bbf1a39", "sha3-512": "e21b1ba2bf287a6c356b96b8c9c08c439d99dab8d877669d087991479b3906eb5f25540c674655b7e4d99ca07e9d4eac62183d0c34815dd9c5c9862be62135cf"}
     arts -2024.1.30.zip                        -info {"size": 582125, "sha-512": "f33c6f44f62871b7f3660c91d19b80b9a03fa1f93d537b461a37e479e5b4fd823a57c97d52d0c6160d92d1bf8ae0a6e61101c5d759792303c094d5c8e5ec68fb", "sha3-512": "af8bf7c9d2b342de2296756c2048e5f4b14ee09fee032559a18f05ce471a85ad56c01d72b40f13369c848a0fff136be0d700b09ffc9df4fbe104a795abac1a99"}
     arts -2024.2.13.zip                        -info {"size": 633463, "sha-512": "335fc45861fd8785c077baa2b2035702340a1e0cd815ae11db258f61979948edf55139757d2991d3800a2398e89ac225dbff8150418aae0c9df980d92c895110", "sha3-512": "d4381233c7c640d474fea34eeebfa9e7cc0d2ba07b3bfe9ea9bad81a34d83828f511b395bf7b6b7d4d474798cb4950181d569200d95091ffd08b099e181e270a"}
     arts -2024.2.25.zip                        -info {"size": 662003, "sha-512": "430648c7c3e2623f4addad65ed6897d8d70b994c65612217cccb5f106596910e9eeadf5417d5036532921a4b8161cda8d93f73d6acf5572b1089cf7084a290e2", "sha3-512": "d0f228a0e9a5c8f6fcfca392fded9abfda2ab1b82939cb50a45b4977b00bd427c81913289924d704bdda8c21bc61eb3ef22cb6b09d311b768a2d52a62eafccdc"}
     arts -2024.3.25.zip                        -info {"size": 731537, "sha-512": "ab80e3c2c0e583552c45134a01991c40f7b02379249299ce19cd01fa411b7e034cb6cc9d8078b93a183577261f20ef6fcca8a0ba05e781d492c7e8d5d2192604", "sha3-512": "0e532cac08a44498c3f001ebdd262fd21e471165a6503264bca0b26b81d63b9de869cda5d94d741b6187e12f93b5167c5bda34ea274398a9da66168538f5a565"}
     arts -2024.3.31.zip                        -info {"size": 784894, "sha-512": "d14e1defcd1845602c68dfa1e2b01f08b970eaa0c2c08426eab9f7c2acc265ed2eaee024c7f9cb935e05477fc1e078e43cd2f09b2806d57a77880542e179a570", "sha3-512": "ee6ee0dd3247be1bbacde5819d8fb8e2a35422ce7e4c4ce20fef13ac80598ed654d65182d550e0f29d4a694dfba38eef825747a6565265af954a217d9c20ab86"}
     arts -2024.3.6.zip                         -info {"size": 729443, "sha-512": "f7d02e0c59ca5da9460ef8af9ed08d2c3c2bc903a3cec85411588badc42f81b64c0df2841b5fb790d24fb3eeb6728e2e7cb363d8bfa859afd7b23b8b997cd83b", "sha3-512": "8fa2af71bcb48993cb6be156c6e07a4ad052fb83cd1d35c89fcb237d135a0a05c2f3aeea7490b5874d3f0b8f61d0e72560163cc2d0c8ff6d58cd86bc902942f8"}
-    arts -2024.4.13.zip                        -info {"size": 813929, "sha-512": "ef483a296af3c56b6d3b80f2baff07514e8cae1d386a27e98cf5d7ef21a4f57d790138670ec9bab24f3d89bb2cbaabe54f2d4ad2ccfc0599678ce372507c79ec", "sha3-512": "09d9958de1a143acc5b2b5e95dde5d64192dd3e110dc49152ff72a02d275bf380dd0bb44a678185e81ef78b2bb9bcfe556e57df5ebc9c9dd94580c5090414c27"}
     arts -2024.4.3.zip                         -info {"size": 792338, "sha-512": "7e8eab613cf52949bfa96c275571fb897bafd67cbdb4c1c94167cb6891336f8f1590853bb8fada5be5c0f227feeda2eb6dd6c2f25b9c773d0de1323d63ec9110", "sha3-512": "b3520b0c6dde6365f97b38232657c005250206cfcb5001085bae1f2610b1cb6d5c79403c4b58b1061c9d957e0e37154620869458119d15fd0cd70e13aa5227e7"}
     wss -20231220.zip                          -info {"size": 8614060, "sha-512": "473d3652c54b15af6fde766cea58974e63b66ba086d44d09b4de6b50d275d07bac4d4c4d6b632dde6e85e971d35566f958efd1b6741d6b96ae67ee6f2ee362b2", "sha3-512": "5f4c6eb204872dc7893c607afabb016ceec67561ddbe76bfb65610d91a3d7dfcce7a0a27da7c81d4f9bee442a97609bfa3d62bee15c2fd435c19ad3152693785"}
     wss -20240325.zip                          -info {"size": 8200568, "sha-512": "2539dd1162403630a705148c90d79b393e9f4a3b9eb81231bfa9fcfe31d1fe185e68c3226bf0d3ae76377c8e3465452e32497e5f470bfe07b60b6fabdd0d509c", "sha3-512": "d510ad8925838c974f2807c79b500a9a7eceddf7dc9f62169615cebfe24f4af484eddecd1ca7c7413e99b8f0a0870b2fe7b6184f475b77736bb754ccd2977f34"}
     wss -20240331.zip                          -info {"size": 8370828, "sha-512": "d644b57284a09ef8fcaeb516dad6d97a997d40cfc0dbcfa3f1f55593b8f76000d93c3708c43d5fc50e5d6255f0d8ca9e52016e618a595d32657bdd466849d772", "sha3-512": "05d33f34bdfcce247dc5ddf27ad9845f01c656711938ffef1f3d006c78c26d08b9d6a6c0f961d85a07393d26cc5c346bc7f27cb94e786d90434fbc70fc3b4284"}
     wss -20240403.zip                          -info {"size": 8472849, "sha-512": "2a21df6fa9808250f384363a0eded43ba177364c8ec67c1b535f4ad9870e9a65fd4b60624b70f20aaa94f3d24e057d463d63268e7a0412ae7819acb4d93db084", "sha3-512": "1455a2ba7e55b3784e57e036fddcd6b080661ffeb35fc6c7447d4fd6573c6130914726a11f84dc0bb584b02d7ab5be51ee8dfbfe91a26c73bf9efce2d9e994a8"}
-    wss -20240413.zip                          -info {"size": 8960665, "sha-512": "b9f57d8e1cce63d12398b7bf805c272f77fd16ea2a519ee8ec2f636d2c50d9a41d73f5ce581bedf01aa2651e6b2de14b842c290c6e5befc007f2661588b2fe23", "sha3-512": "4c1bf6de3863cf8f1ea68a343449687b3a820c6cafbee2ea616da39754c4728e9278da362b7344a55b23aca898cd820aab64dcb284d3d2772213ff1130ef49ed"}
 富文本笔记本.png                               -info {"size": 644251, "sha-512": "e8293b799d49e53501fb50e85f7025d3d1f7c83e05f8982af51cc75c309d5014a17fb2326b8476335575b6bf4f8c2d4ffe2f4de9c3c423ef92adc3766996832f", "sha3-512": "82aecb03ab4abb583a6791b32301d76dafc451a70ee2f22b0c2c71428a0f100471beae02195681b61d1f6d7d1efdeaac719ffafbce9410b2c5065fe05841b009"}
 按键行为和鼠标行为采集装置                 
     2023-09-12.zip                             -info {"size": 939254, "sha-512": "939a9ee1132c5a5ef837f3f77b2bb005caafcd4f7cbc8ea1d219f2b1a1f512c7b71faf2c7a96ab961f7f62918992f1122e497c08c435f9579ff6c5d13f00b90f", "sha3-512": "efedfc0ece0c44d2ea1fb705dac8ab5283e74faf6e3e973a91ce447ffae1cc85359f96b1b33092fe61032a1424c62ed6e37a9fb9107f9029008474f3977a4446"}
 捷鸟.jpg                                       -info {"size": 793233, "sha-512": "96da3cf6df87d85d59bbdf80ccbbf0c841fcdd52d37ca2556219020c94978c01cf648df52d51dc2733f5bc773b734d9ba5b17e9cc8056278857a9059f5c756e3", "sha3-512": "99dfdb17c8663587c7db7b18621c11743e89cb67f6ab8be395c5901adae0a3fe7838175fcba7194927deb1c3ae509c1577eb2ad4b4d3c04890c94b77b00cc311"}
 桌面APP导航栏.png                              -info {"size": 256699, "sha-512": "b5cc935b98f28f0354b401e5f6d8e9768376ba6be7be1996247155459792a2a27131fee396bf0c8384c9e504115eb84d86f713e5d229f132889fd2b03b44f1e8", "sha3-512": "64c1edea61003c4147974a0f81eb748d98de1678d5a3ec13149297219526de25656942b8eb6c21b0546a3ea2dc9af367def29f6a60e81aab01796e146fdb5f4a"}
 短视频                                     
     AI是这样画包拯的.mp4                       -info {"size": 1927086, "sha-512": "eab1c2640c96826a1e15166bbdfcd5bd0011b5561ec3548d3c067f24627060354db699e49dd700e48ecbdeddd5d1492dabaa6ad08de8a5f66554dfd18a7eb96a", "sha3-512": "357b5252450d3b530b76e208d0ac3934df007dbe80259f1e5cabe6a9f4f9b23a76da858af1725dadaafcc762dea4a2ddb7a961d1bab794c10b89f5829c39156d"}
```

### Comparing `skybox-2024.4.13/PKG-INFO` & `skybox-2024.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skybox
-Version: 2024.4.13
+Version: 2024.4.3
 Summary: 对 字符串/列表/元组/数列 等数据按固定单元长度分组
 Author-email: 江南雨上 <lcctoor@outlook.com>
 Description-Content-Type: text/markdown
 
 一个用来对 字符串/列表/元组/数列 等数据按固定单元长度分组的功能：
 
 ```python
```

