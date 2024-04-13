# Comparing `tmp/asmr_spider-0.2.1.tar.gz` & `tmp/asmr_spider-0.2.2b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asmr_spider-0.2.1.tar", max compression
+gzip compressed data, was "asmr_spider-0.2.2b1.tar", max compression
```

## Comparing `asmr_spider-0.2.1.tar` & `asmr_spider-0.2.2b1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-04-08 04:01:37.819279 asmr_spider-0.2.1/LICENSE
--rw-r--r--   0        0        0     2716 2024-04-08 04:01:37.819279 asmr_spider-0.2.1/README.md
--rw-r--r--   0        0        0     1212 2024-04-08 04:01:37.819279 asmr_spider-0.2.1/asmr_spider/__init__.py
--rw-r--r--   0        0        0      389 2024-04-08 04:01:37.819279 asmr_spider-0.2.1/asmr_spider/__main__.py
--rw-r--r--   0        0        0     1803 2024-04-08 04:01:37.819279 asmr_spider-0.2.1/asmr_spider/config.py
--rw-r--r--   0        0        0     7221 2024-04-08 04:01:37.819279 asmr_spider-0.2.1/asmr_spider/spider.py
--rw-r--r--   0        0        0     1022 2024-04-08 04:01:37.819279 asmr_spider-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     3613 1970-01-01 00:00:00.000000 asmr_spider-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-13 15:21:13.858362 asmr_spider-0.2.2b1/LICENSE
+-rw-r--r--   0        0        0     3178 2024-04-13 15:21:13.858362 asmr_spider-0.2.2b1/README.md
+-rw-r--r--   0        0        0     1377 2024-04-13 15:21:13.858362 asmr_spider-0.2.2b1/asmr_spider/__init__.py
+-rw-r--r--   0        0        0      389 2024-04-13 15:21:13.858362 asmr_spider-0.2.2b1/asmr_spider/__main__.py
+-rw-r--r--   0        0        0     1803 2024-04-13 15:21:13.858362 asmr_spider-0.2.2b1/asmr_spider/config.py
+-rw-r--r--   0        0        0     9038 2024-04-13 15:21:13.858362 asmr_spider-0.2.2b1/asmr_spider/spider.py
+-rw-r--r--   0        0        0     1029 2024-04-13 15:21:13.858362 asmr_spider-0.2.2b1/pyproject.toml
+-rw-r--r--   0        0        0     4077 1970-01-01 00:00:00.000000 asmr_spider-0.2.2b1/PKG-INFO
```

### Comparing `asmr_spider-0.2.1/LICENSE` & `asmr_spider-0.2.2b1/LICENSE`

 * *Files identical despite different names*

### Comparing `asmr_spider-0.2.1/README.md` & `asmr_spider-0.2.2b1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -20,36 +20,41 @@
 
 
 ## TODO
 
 - [x] 文件检查 (通过时长)
 - [x] 错误文件重新下载
 - [x] 支持更多格式 (通过 `ffmpeg` 和 `ffprobe`)
-- [ ] ffmpeg的分析很慢, 寻找更好的方式
+- [x] ffmpeg的分析很慢, 寻找更好的方式（检测大小或许能替代？）
 - [ ] 指定下载路径
 - [ ] 下载文件中途停止记录
-- [ ] 断点续传
+- [x] 断点续传
 - [ ] 下载自动分类配置
 
 
 ## 使用
 
+### 音频大小对比模式
+支持断点续传
+
+### 音频时长分析模式
 不使用 `ffmpeg` 和 `ffprobe` 时仅支持 `mp3` `wav` `flac` 格式的音频分析  
   
 [ffmpeg Documentation](https://www.ffmpeg.org/)  
 [ffprobe Documentation](https://www.ffmpeg.org/ffprobe.html)  
   
 目前 `ffmpeg` 分析很慢, 平均一个文件3s以上  
   
   
 ### 已知问题
 
 未安装**ffmpeg**时可能会报缺少**libsndfile**等运行库,  
 仍需要另外安装相关依赖.
   
+在使用**checktime**进行时长检测部分mp3内容时,获取的时长差异过大，同时在错误状态下仍然会检测为正常状态（如RJ172342），故默认使用时长检测时仍保留重新下载的模式。
 
 <details>
   <summary>Install ffmpeg or libsndfile</summary>
   <br>
 
   **Debian/Ubuntu安装:**
   ```zsh
@@ -96,17 +101,20 @@
 
 ### Run
 
 ```bash
 #直接下载, 默认检查重复
 asmr RJ373001 RJ385913
 #或者
-asmr RJ373001 RJ385913 -a check
+asmr RJ373001 RJ385913 -a checksize
 # `asmr` 后面接RJ号, 可输入多个, 使用空格隔开
 
+#通过时长检测重复内容,目前不支持断点续传
+asmr RJ373001 RJ385913 -a checktime
+
 #禁用检查, 跳过已下载的文件
 asmr RJ373001 RJ385913 -a nocheck
 
 #强制重新下载所有文件
 asmr RJ373001 RJ385913 -a redownload
 ```
 
@@ -116,15 +124,15 @@
   <summary>Import</summary>
 
 ```python3
 from asmr_spider import dload
 
 async def demo():
     args = ['RJ373001', 'RJ385913']
-    action = 'check'  # 'check', 'redownload', 'nocheck'
+    action = 'checksize'  # 'checksize', 'checktime','redownload', 'nocheck'
     await dload(args, action)
 ```
 
 `asmr_spider.yml` 和 `Voice` 将保存在你自己的项目根路径
 
 </details>
```

#### html2text {}

```diff
@@ -1,33 +1,39 @@
 # ASMR-Spider æ¬é¡¹ç®æ¹ç¼èª [DiheChen/go-asmr-spider](https://github.com/
 DiheChen/go-asmr-spider/tree/python)
 _[_L_i_c_e_n_s_e_]_[_P_y_P_I_]_[_P_y_t_h_o_n_]
 ä¸ä¸ªç®åç
 asmr.one> ç¬è« ## TODO - [x] æä»¶æ£æ¥ (éè¿æ¶é¿) - [x]
 éè¯¯æä»¶éæ°ä¸è½½ - [x] æ¯ææ´å¤æ ¼å¼ (éè¿ `ffmpeg` å
-`ffprobe`) - [ ] ffmpegçåæå¾æ¢, å¯»æ¾æ´å¥½çæ¹å¼ - [ ]
-æå®ä¸è½½è·¯å¾ - [ ] ä¸è½½æä»¶ä¸­éåæ­¢è®°å½ - [ ] æ­ç¹ç»­ä¼  -
-[ ] ä¸è½½èªå¨åç±»éç½® ## ä½¿ç¨ ä¸ä½¿ç¨ `ffmpeg` å `ffprobe`
-æ¶ä»æ¯æ `mp3` `wav` `flac` æ ¼å¼çé³é¢åæ [ffmpeg Documentation]
-(https://www.ffmpeg.org/) [ffprobe Documentation](https://www.ffmpeg.org/
-ffprobe.html) ç®å `ffmpeg` åæå¾æ¢, å¹³åä¸ä¸ªæä»¶3sä»¥ä¸ ###
-å·²ç¥é®é¢
+`ffprobe`) - [x] ffmpegçåæå¾æ¢,
+å¯»æ¾æ´å¥½çæ¹å¼ï¼æ£æµå¤§å°æè®¸è½æ¿ä»£ï¼ï¼ - [ ]
+æå®ä¸è½½è·¯å¾ - [ ] ä¸è½½æä»¶ä¸­éåæ­¢è®°å½ - [x] æ­ç¹ç»­ä¼  -
+[ ] ä¸è½½èªå¨åç±»éç½® ## ä½¿ç¨ ### é³é¢å¤§å°å¯¹æ¯æ¨¡å¼
+æ¯ææ­ç¹ç»­ä¼  ### é³é¢æ¶é¿åææ¨¡å¼ ä¸ä½¿ç¨ `ffmpeg` å
+`ffprobe` æ¶ä»æ¯æ `mp3` `wav` `flac` æ ¼å¼çé³é¢åæ [ffmpeg
+Documentation](https://www.ffmpeg.org/) [ffprobe Documentation](https://
+www.ffmpeg.org/ffprobe.html) ç®å `ffmpeg` åæå¾æ¢,
+å¹³åä¸ä¸ªæä»¶3sä»¥ä¸ ### å·²ç¥é®é¢
 æªå®è£**ffmpeg**æ¶å¯è½ä¼æ¥ç¼ºå°**libsndfile**ç­è¿è¡åº,
-ä»éè¦å¦å¤å®è£ç¸å³ä¾èµ. Install ffmpeg or libsndfile
+ä»éè¦å¦å¤å®è£ç¸å³ä¾èµ.
+å¨ä½¿ç¨**checktime**è¿è¡æ¶é¿æ£æµé¨åmp3åå®¹æ¶,è·åçæ¶é¿å·®å¼è¿å¤§ï¼åæ¶å¨éè¯¯ç¶æä¸ä»ç¶ä¼æ£æµä¸ºæ­£å¸¸ç¶æï¼å¦RJ172342ï¼ï¼æé»è®¤ä½¿ç¨æ¶é¿æ£æµæ¶ä»ä¿çéæ°ä¸è½½çæ¨¡å¼ã
+Install ffmpeg or libsndfile
 **Debian/Ubuntuå®è£:** ```zsh apt update && apt install ffmpeg ```
 **æè**: ```zsh apt update && apt install libsndfile1 ```
 **ArchLinuxå®è£:** ```zsh pacman -Syu ffmpeg ``` **æè**: ```zsh pacman -
 Syu libsndfile ```
 **Macå®è£:** ```zsh brew install ffmpeg ```
 **Windowså®è£:** è¯·åè [ffmpeg Documentation](https://www.ffmpeg.org/
 ) èªè¡è§£å³ ### Install ```bash pip install -U asmr-spider ``` ### Run
 ```bash #ç´æ¥ä¸è½½, é»è®¤æ£æ¥éå¤ asmr RJ373001 RJ385913 #æè asmr
-RJ373001 RJ385913 -a check # `asmr` åé¢æ¥RJå·, å¯è¾å¥å¤ä¸ª,
-ä½¿ç¨ç©ºæ ¼éå¼ #ç¦ç¨æ£æ¥, è·³è¿å·²ä¸è½½çæä»¶ asmr RJ373001
-RJ385913 -a nocheck #å¼ºå¶éæ°ä¸è½½æææä»¶ asmr RJ373001 RJ385913 -
-a redownload ``` éç½®æä»¶ `asmr_spider.yml` å é³é¢ç®å½ `Voice`
-ä¿å­å¨å½ä»¤æ§è¡æ¶æå¨çè·¯å¾ Import ```python3 from asmr_spider
-import dload async def demo(): args = ['RJ373001', 'RJ385913'] action = 'check'
-# 'check', 'redownload', 'nocheck' await dload(args, action) ```
-`asmr_spider.yml` å `Voice` å°ä¿å­å¨ä½ èªå·±çé¡¹ç®æ ¹è·¯å¾ ## è´è°¢
-- æè°¢ [å°æ²³é±](https://github.com/DiheChen), å°æ²³é±yydsð¤ - æè°¢
+RJ373001 RJ385913 -a checksize # `asmr` åé¢æ¥RJå·, å¯è¾å¥å¤ä¸ª,
+ä½¿ç¨ç©ºæ ¼éå¼ #éè¿æ¶é¿æ£æµéå¤åå®¹,ç®åä¸æ¯ææ­ç¹ç»­ä¼ 
+asmr RJ373001 RJ385913 -a checktime #ç¦ç¨æ£æ¥, è·³è¿å·²ä¸è½½çæä»¶
+asmr RJ373001 RJ385913 -a nocheck #å¼ºå¶éæ°ä¸è½½æææä»¶ asmr RJ373001
+RJ385913 -a redownload ``` éç½®æä»¶ `asmr_spider.yml` å é³é¢ç®å½
+`Voice` ä¿å­å¨å½ä»¤æ§è¡æ¶æå¨çè·¯å¾ Import ```python3 from
+asmr_spider import dload async def demo(): args = ['RJ373001', 'RJ385913']
+action = 'checksize' # 'checksize', 'checktime','redownload', 'nocheck' await
+dload(args, action) ``` `asmr_spider.yml` å `Voice`
+å°ä¿å­å¨ä½ èªå·±çé¡¹ç®æ ¹è·¯å¾ ## è´è°¢ - æè°¢ [å°æ²³é±](https://
+github.com/DiheChen), å°æ²³é±yydsð¤ - æè°¢
 asmr.one>, ç°å¨æ¯å¤©é½æä¸åçå¥³å­©å­éªæç¡è§ã
```

### Comparing `asmr_spider-0.2.1/asmr_spider/config.py` & `asmr_spider-0.2.2b1/asmr_spider/config.py`

 * *Files identical despite different names*

### Comparing `asmr_spider-0.2.1/asmr_spider/spider.py` & `asmr_spider-0.2.2b1/asmr_spider/spider.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,170 +1,198 @@
-import asyncio, soundfile, os
+import asyncio
+import os
 from typing import Any, Dict, List
 try:
     import ujson as json
 except ImportError:
     import json
 from pathlib import Path
 from httpx import AsyncClient
 
 from .config import config, progress, logger
-from pydub import AudioSegment
 
 
 timeout: int = 120
 semaphore: int = 16
 default_audio_exts: tuple = ('.wav', '.flac', '.mp3')
-ffmpeg_audio_exts: tuple = ('.wma', '.ogg', '.m4a', '.ape', '.opus', '.aac', '.mka')
+ffmpeg_audio_exts: tuple = ('.wma', '.ogg', '.m4a',
+                            '.ape', '.opus', '.aac', '.mka')
+
 
 class ASMRSpider:
 
     def __init__(self, support_ffmpeg) -> None:
         self.name = config.username
         self.password = config.password
         self.headers = {
             "Referer": "https://www.asmr.one/",
             "User-Agent": config.user_agent,
         }
         self.support_ffmpeg = support_ffmpeg
 
-
     async def login(self) -> None:
         resp = await self.client.post(
             "https://api.asmr.one/api/auth/me",
             json={"name": self.name, "password": self.password},
             headers=self.headers,
-            timeout=timeout
-        )
+            timeout=timeout)
         self.headers |= {
             "Authorization": f"Bearer {(resp.json())['token']}",
         }
 
-
     async def get_voice_info(self, voice_id: str) -> Dict[str, Any]:
         resp = await self.client.get(
             f"https://api.asmr.one/api/work/{voice_id}",
             headers=self.headers,
-            timeout=timeout
-        )
+            timeout=timeout)
         return resp.json()
 
-
     async def get_voice_tracks(self, voice_id):
         resp = await self.client.get(
             f"https://api.asmr.one/api/tracks/{voice_id}",
             headers=self.headers,
-            timeout=timeout
-        )
+            timeout=timeout)
         return resp.json()
 
-
-    def is_bad_file(self, file, file_time):
+    async def check_file_time(self, file_path, file_time):
         try:
             is_bad = False
             duration = 0.0
-            #ffmpeg 查看时长很慢, 所以能使用其他库就不用ffmpeg
-            if os.path.splitext(file)[-1].lower() in default_audio_exts:
-                data = soundfile.SoundFile(file)
+            # ffmpeg 查看时长很慢, 所以能使用其他库就不用ffmpeg
+            if os.path.splitext(file_path)[-1].lower() in default_audio_exts:
+                import soundfile  # 尝试需要时再进行导入
+                data = soundfile.SoundFile(file_path)
                 duration = data.frames/data.samplerate
 
-            elif self.support_ffmpeg and os.path.splitext(file)[-1].lower() in ffmpeg_audio_exts:
-                sound = AudioSegment.from_file(file)
+            elif self.support_ffmpeg and os.path.splitext(file_path)[-1].lower() in ffmpeg_audio_exts:
+                from pydub import AudioSegment
+                sound = AudioSegment.from_file(file_path)
                 duration = sound.duration_seconds
 
             else:
-                logger.info(f := (f"文件跳过检测: {file}"))
+                logger.info(f := (f"文件跳过检测: {file_path}"))
                 progress.console.log(f)
                 return False
 
-            is_bad = (file_time - duration)>0.1
-            logger.info(f :=f"检测文件: {file}, 文件是否完全下载: {not is_bad}\n"
-                                    f"获取时长: {file_time}, 本地时长: {duration}")
+            is_bad = (file_time - duration) > 0.1
+            logger.info(f := f"检测文件: {file_path}, 文件是否完全下载: {not is_bad}\n"
+                        f"获取时长: {file_time}, 本地时长: {duration}")
             progress.console.log(f)
             return is_bad
 
         except Exception as e:
-                print(str(e))
-                logger.exception(e)
-                raise e
-
+            print(str(e))
+            logger.exception(e)
+            raise e
+
+    async def check_file_size(self, url: str, file_size, file_name):
+        is_bad = False
+        temp_headers = self.headers.copy()
+
+        d = {"Accept-Encoding": "identity"}
+        temp_headers.update(d)
+        # 单独获取一次长度
+        async with self.client.stream("HEAD",
+                                      url=url,
+                                      headers=self.headers,
+                                      timeout=timeout) as resp_get_length:
+            if resp_get_length.status_code != 200:
+                return
+            remote_size = -1
+            if resp_get_length.headers.get('Content-Length'):
+                remote_size = int(
+                    resp_get_length.headers.get('Content-Length'))
+            elif resp_get_length.headers.get('x-content-length'):
+                remote_size = int(
+                    resp_get_length.headers.get('x-content-length'))
+
+            is_bad = (remote_size - file_size) > 0 or remote_size == -1
+            logger.info(f := f"检测文件: {file_name}, 文件是否完全下载: {not is_bad}\n"
+                        f"获取大小长: {remote_size}, 本地大小: {file_size}")
+            progress.console.log(f)
+            return is_bad
 
-    async def download_file(self, sem, url: str, save_path: Path, file_name: str, file_time: float) -> None:
-        file_name = file_name.translate(str.maketrans(r'/\:*?"<>|', "_________"))
+    async def download_file(self, sem, url: str, save_path: Path,
+                            file_name: str, file_time) -> None:
+        file_name = file_name.translate(
+            str.maketrans(r'/\:*?"<>|', "_________"))
         file_path = save_path / file_name
-        #筛选是否重新下载
+        temp_headers = self.headers.copy()
+
+        # 本地已经下载的文件大小
+        file_size = (0 if not os.path.exists(file_path) else
+                     os.path.getsize(file_path))
+
+        # 筛选是否重新下载
         is_checked_not_pass = True
+        file_option = 'wb'
         if file_path.exists():
-            if self.checkAction == 'check':
-                is_checked_not_pass = self.is_bad_file(file_path, file_time)
+            if self.checkAction == 'checksize':
+                is_checked_not_pass = await self.check_file_size(url, file_size, file_name)
+                d = {"Range": "bytes=%d-" % file_size}
+                temp_headers.update(d)
+                file_option = 'ab'
+            elif self.checkAction == 'checktime':
+                is_checked_not_pass = await self.check_file_time(file_path, file_time)
             elif self.checkAction == 'nocheck':
-                    is_checked_not_pass = False
+                is_checked_not_pass = False
             elif self.checkAction == 'redownload':
-                    is_checked_not_pass = True
-
-        if not file_path.exists() or is_checked_not_pass:
+                is_checked_not_pass = True
+        if file_size == 0 or is_checked_not_pass:
             async with sem:
-                async with self.client.stream(
-                    "GET", url=url,
-                    headers=self.headers, timeout=timeout
-                ) as resp:
-                    if resp.status_code != 200:
+                async with self.client.stream("GET",
+                                              url=url,
+                                              headers=temp_headers,
+                                              timeout=timeout) as resp:
+                    if resp.status_code != 200 and resp.status_code != 206:
                         logger.error(f := f"{file_path}: {resp.status_code}")
                         progress.console.log(f, style='bold yellow on black')
                         return
 
                     total = resp.headers.get("Content-Length")
                     task_id = progress.add_task(  # 进度条
                         "download",
                         start=True,
                         total=int(total) if total else None,
-                        filename = (
-                            file_name[:4] + "..." + file_name[-4:]
-                            if len(file_name) > 12
-                            else file_name
-                        )
-                    )
+                        filename=(file_name[:4] + "..." + file_name[-4:]
+                                  if len(file_name) > 12 else file_name))
 
-                    with open(file_path, 'wb') as fd:  # 写入文件
+                    with open(file_path, file_option) as fd:  # 写入文件
                         async for chunk in resp.aiter_bytes(1024):
-                            fd.write(chunk)
-                            progress.update(
-                                task_id,
-                                advance=len(chunk),
-                            )
+                            if chunk:
+                                fd.write(chunk)
+                                progress.update(
+                                    task_id,
+                                    advance=len(chunk),
+                                )
+                            else:
+                                break
 
                     await asyncio.to_thread(progress.remove_task, task_id)
                     logger.success(f := f"{file_path}: Success.")
                     progress.console.log(f)
 
-
-    async def ensure_dir(self, tracks: List[Dict[str, Any]], root_path: Path) -> None:
+    async def ensure_dir(self, tracks: List[Dict[str, Any]],
+                         root_path: Path) -> None:
         folders: list = [i for i in tracks if i["type"] == "folder"]
         files: list = [i for i in tracks if i["type"] != "folder"]
 
         sem = asyncio.Semaphore(semaphore)
         down: list = []
         for file in files:
-            if "duration" in file:
-                down.append(
-                    self.download_file(sem, file["mediaDownloadUrl"], root_path, file["title"], file["duration"])
-                )
-            else:
-                  down.append(
-                    self.download_file(sem, file["mediaDownloadUrl"], root_path, file["title"], 0)
-                )
+            down.append(
+                self.download_file(sem, file["mediaDownloadUrl"], root_path, file["title"], file_time=file.get("duration")))
         with progress:
             await asyncio.gather(*down)
 
         for folder in folders:
             new_path: Path = root_path / folder["title"]
             new_path.mkdir(parents=True, exist_ok=True)
             await self.ensure_dir(folder["children"], new_path)
 
-
     async def download(self, voice_id: str, action) -> None:
         self.checkAction = action
         voice_id = voice_id.strip().split("RJ")[-1]
         voice_info = await self.get_voice_info(voice_id)
 
         if err := (voice_info.get("errors") or voice_info.get("error")):
             err = json.dumps(err, ensure_ascii=False, indent=2)
@@ -187,16 +215,14 @@
         root.mkdir(parents=True, exist_ok=True)
         (root / f"RJ{voice_id}.json").write_text(
             json.dumps(voice_info, ensure_ascii=False, indent=4), 'utf-8')
 
         tracks = await self.get_voice_tracks(voice_id)
         await self.ensure_dir(tracks, root)
 
-
     async def __aenter__(self) -> "ASMRSpider":
         self.client = AsyncClient(proxies=config.proxy or None)
         await self.login()
         return self
 
-
     async def __aexit__(self, *args) -> None:
         await self.client.aclose()
```

### Comparing `asmr_spider-0.2.1/pyproject.toml` & `asmr_spider-0.2.2b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asmr-spider"
-version = "0.2.1"
+version = "0.2.2-beta.1"
 description = "asmr.one 音声下载器"
 authors = ["月ヶ瀬"]
 license = "GPL-3.0"
 readme = "README.md"
 packages = [
     { include = "asmr_spider" },
 ]
```

### Comparing `asmr_spider-0.2.1/PKG-INFO` & `asmr_spider-0.2.2b1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asmr-spider
-Version: 0.2.1
+Version: 0.2.2b1
 Summary: asmr.one 音声下载器
 Home-page: https://github.com/tkgs0/asmr-spider
 License: GPL-3.0
 Keywords: ASMR,ASMR Downloader
 Author: 月ヶ瀬
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -45,36 +45,41 @@
 
 
 ## TODO
 
 - [x] 文件检查 (通过时长)
 - [x] 错误文件重新下载
 - [x] 支持更多格式 (通过 `ffmpeg` 和 `ffprobe`)
-- [ ] ffmpeg的分析很慢, 寻找更好的方式
+- [x] ffmpeg的分析很慢, 寻找更好的方式（检测大小或许能替代？）
 - [ ] 指定下载路径
 - [ ] 下载文件中途停止记录
-- [ ] 断点续传
+- [x] 断点续传
 - [ ] 下载自动分类配置
 
 
 ## 使用
 
+### 音频大小对比模式
+支持断点续传
+
+### 音频时长分析模式
 不使用 `ffmpeg` 和 `ffprobe` 时仅支持 `mp3` `wav` `flac` 格式的音频分析  
   
 [ffmpeg Documentation](https://www.ffmpeg.org/)  
 [ffprobe Documentation](https://www.ffmpeg.org/ffprobe.html)  
   
 目前 `ffmpeg` 分析很慢, 平均一个文件3s以上  
   
   
 ### 已知问题
 
 未安装**ffmpeg**时可能会报缺少**libsndfile**等运行库,  
 仍需要另外安装相关依赖.
   
+在使用**checktime**进行时长检测部分mp3内容时,获取的时长差异过大，同时在错误状态下仍然会检测为正常状态（如RJ172342），故默认使用时长检测时仍保留重新下载的模式。
 
 <details>
   <summary>Install ffmpeg or libsndfile</summary>
   <br>
 
   **Debian/Ubuntu安装:**
   ```zsh
@@ -121,17 +126,20 @@
 
 ### Run
 
 ```bash
 #直接下载, 默认检查重复
 asmr RJ373001 RJ385913
 #或者
-asmr RJ373001 RJ385913 -a check
+asmr RJ373001 RJ385913 -a checksize
 # `asmr` 后面接RJ号, 可输入多个, 使用空格隔开
 
+#通过时长检测重复内容,目前不支持断点续传
+asmr RJ373001 RJ385913 -a checktime
+
 #禁用检查, 跳过已下载的文件
 asmr RJ373001 RJ385913 -a nocheck
 
 #强制重新下载所有文件
 asmr RJ373001 RJ385913 -a redownload
 ```
 
@@ -141,15 +149,15 @@
   <summary>Import</summary>
 
 ```python3
 from asmr_spider import dload
 
 async def demo():
     args = ['RJ373001', 'RJ385913']
-    action = 'check'  # 'check', 'redownload', 'nocheck'
+    action = 'checksize'  # 'checksize', 'checktime','redownload', 'nocheck'
     await dload(args, action)
 ```
 
 `asmr_spider.yml` 和 `Voice` 将保存在你自己的项目根路径
 
 </details>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: asmr-spider Version: 0.2.1 Summary: asmr.one
+Metadata-Version: 2.1 Name: asmr-spider Version: 0.2.2b1 Summary: asmr.one
 é³å£°ä¸è½½å¨ Home-page: https://github.com/tkgs0/asmr-spider License: GPL-
 3.0 Keywords: ASMR,ASMR Downloader Author: æã¶ç¬ Requires-Python:
 >=3.9,<4.0 Classifier: License :: OSI Approved :: GNU General Public License v3
 (GPLv3) Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Requires-Dist: PyYAML (>=6.0) Requires-Dist: httpx
@@ -12,34 +12,40 @@
 github.com/tkgs0/asmr-spider Description-Content-Type: text/markdown # ASMR-
 Spider æ¬é¡¹ç®æ¹ç¼èª [DiheChen/go-asmr-spider](https://github.com/
 DiheChen/go-asmr-spider/tree/python)
 _[_L_i_c_e_n_s_e_]_[_P_y_P_I_]_[_P_y_t_h_o_n_]
 ä¸ä¸ªç®åç
 asmr.one> ç¬è« ## TODO - [x] æä»¶æ£æ¥ (éè¿æ¶é¿) - [x]
 éè¯¯æä»¶éæ°ä¸è½½ - [x] æ¯ææ´å¤æ ¼å¼ (éè¿ `ffmpeg` å
-`ffprobe`) - [ ] ffmpegçåæå¾æ¢, å¯»æ¾æ´å¥½çæ¹å¼ - [ ]
-æå®ä¸è½½è·¯å¾ - [ ] ä¸è½½æä»¶ä¸­éåæ­¢è®°å½ - [ ] æ­ç¹ç»­ä¼  -
-[ ] ä¸è½½èªå¨åç±»éç½® ## ä½¿ç¨ ä¸ä½¿ç¨ `ffmpeg` å `ffprobe`
-æ¶ä»æ¯æ `mp3` `wav` `flac` æ ¼å¼çé³é¢åæ [ffmpeg Documentation]
-(https://www.ffmpeg.org/) [ffprobe Documentation](https://www.ffmpeg.org/
-ffprobe.html) ç®å `ffmpeg` åæå¾æ¢, å¹³åä¸ä¸ªæä»¶3sä»¥ä¸ ###
-å·²ç¥é®é¢
+`ffprobe`) - [x] ffmpegçåæå¾æ¢,
+å¯»æ¾æ´å¥½çæ¹å¼ï¼æ£æµå¤§å°æè®¸è½æ¿ä»£ï¼ï¼ - [ ]
+æå®ä¸è½½è·¯å¾ - [ ] ä¸è½½æä»¶ä¸­éåæ­¢è®°å½ - [x] æ­ç¹ç»­ä¼  -
+[ ] ä¸è½½èªå¨åç±»éç½® ## ä½¿ç¨ ### é³é¢å¤§å°å¯¹æ¯æ¨¡å¼
+æ¯ææ­ç¹ç»­ä¼  ### é³é¢æ¶é¿åææ¨¡å¼ ä¸ä½¿ç¨ `ffmpeg` å
+`ffprobe` æ¶ä»æ¯æ `mp3` `wav` `flac` æ ¼å¼çé³é¢åæ [ffmpeg
+Documentation](https://www.ffmpeg.org/) [ffprobe Documentation](https://
+www.ffmpeg.org/ffprobe.html) ç®å `ffmpeg` åæå¾æ¢,
+å¹³åä¸ä¸ªæä»¶3sä»¥ä¸ ### å·²ç¥é®é¢
 æªå®è£**ffmpeg**æ¶å¯è½ä¼æ¥ç¼ºå°**libsndfile**ç­è¿è¡åº,
-ä»éè¦å¦å¤å®è£ç¸å³ä¾èµ. Install ffmpeg or libsndfile
+ä»éè¦å¦å¤å®è£ç¸å³ä¾èµ.
+å¨ä½¿ç¨**checktime**è¿è¡æ¶é¿æ£æµé¨åmp3åå®¹æ¶,è·åçæ¶é¿å·®å¼è¿å¤§ï¼åæ¶å¨éè¯¯ç¶æä¸ä»ç¶ä¼æ£æµä¸ºæ­£å¸¸ç¶æï¼å¦RJ172342ï¼ï¼æé»è®¤ä½¿ç¨æ¶é¿æ£æµæ¶ä»ä¿çéæ°ä¸è½½çæ¨¡å¼ã
+Install ffmpeg or libsndfile
 **Debian/Ubuntuå®è£:** ```zsh apt update && apt install ffmpeg ```
 **æè**: ```zsh apt update && apt install libsndfile1 ```
 **ArchLinuxå®è£:** ```zsh pacman -Syu ffmpeg ``` **æè**: ```zsh pacman -
 Syu libsndfile ```
 **Macå®è£:** ```zsh brew install ffmpeg ```
 **Windowså®è£:** è¯·åè [ffmpeg Documentation](https://www.ffmpeg.org/
 ) èªè¡è§£å³ ### Install ```bash pip install -U asmr-spider ``` ### Run
 ```bash #ç´æ¥ä¸è½½, é»è®¤æ£æ¥éå¤ asmr RJ373001 RJ385913 #æè asmr
-RJ373001 RJ385913 -a check # `asmr` åé¢æ¥RJå·, å¯è¾å¥å¤ä¸ª,
-ä½¿ç¨ç©ºæ ¼éå¼ #ç¦ç¨æ£æ¥, è·³è¿å·²ä¸è½½çæä»¶ asmr RJ373001
-RJ385913 -a nocheck #å¼ºå¶éæ°ä¸è½½æææä»¶ asmr RJ373001 RJ385913 -
-a redownload ``` éç½®æä»¶ `asmr_spider.yml` å é³é¢ç®å½ `Voice`
-ä¿å­å¨å½ä»¤æ§è¡æ¶æå¨çè·¯å¾ Import ```python3 from asmr_spider
-import dload async def demo(): args = ['RJ373001', 'RJ385913'] action = 'check'
-# 'check', 'redownload', 'nocheck' await dload(args, action) ```
-`asmr_spider.yml` å `Voice` å°ä¿å­å¨ä½ èªå·±çé¡¹ç®æ ¹è·¯å¾ ## è´è°¢
-- æè°¢ [å°æ²³é±](https://github.com/DiheChen), å°æ²³é±yydsð¤ - æè°¢
+RJ373001 RJ385913 -a checksize # `asmr` åé¢æ¥RJå·, å¯è¾å¥å¤ä¸ª,
+ä½¿ç¨ç©ºæ ¼éå¼ #éè¿æ¶é¿æ£æµéå¤åå®¹,ç®åä¸æ¯ææ­ç¹ç»­ä¼ 
+asmr RJ373001 RJ385913 -a checktime #ç¦ç¨æ£æ¥, è·³è¿å·²ä¸è½½çæä»¶
+asmr RJ373001 RJ385913 -a nocheck #å¼ºå¶éæ°ä¸è½½æææä»¶ asmr RJ373001
+RJ385913 -a redownload ``` éç½®æä»¶ `asmr_spider.yml` å é³é¢ç®å½
+`Voice` ä¿å­å¨å½ä»¤æ§è¡æ¶æå¨çè·¯å¾ Import ```python3 from
+asmr_spider import dload async def demo(): args = ['RJ373001', 'RJ385913']
+action = 'checksize' # 'checksize', 'checktime','redownload', 'nocheck' await
+dload(args, action) ``` `asmr_spider.yml` å `Voice`
+å°ä¿å­å¨ä½ èªå·±çé¡¹ç®æ ¹è·¯å¾ ## è´è°¢ - æè°¢ [å°æ²³é±](https://
+github.com/DiheChen), å°æ²³é±yydsð¤ - æè°¢
 asmr.one>, ç°å¨æ¯å¤©é½æä¸åçå¥³å­©å­éªæç¡è§ã
```

