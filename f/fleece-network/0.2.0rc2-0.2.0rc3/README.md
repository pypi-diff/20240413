# Comparing `tmp/fleece_network-0.2.0rc2.tar.gz` & `tmp/fleece_network-0.2.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleece_network-0.2.0rc2.tar", max compression
+gzip compressed data, was "fleece_network-0.2.0rc3.tar", max compression
```

## Comparing `fleece_network-0.2.0rc2.tar` & `fleece_network-0.2.0rc3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0      327 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/README.md
--rw-r--r--   0        0        0        0 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/__init__.py
--rw-r--r--   0        0        0      349 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aioice/__init__.py
--rw-r--r--   0        0        0     4060 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aioice/candidate.py
--rw-r--r--   0        0        0    41684 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aioice/ice.py
--rw-r--r--   0        0        0     6655 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aioice/mdns.py
--rw-r--r--   0        0        0    12369 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aioice/stun.py
--rw-r--r--   0        0        0    15077 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aioice/turn.py
--rw-r--r--   0        0        0      264 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aioice/utils.py
--rw-r--r--   0        0        0     1226 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/__init__.py
--rw-r--r--   0        0        0      824 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/clock.py
--rw-r--r--   0        0        0      180 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/exceptions.py
--rw-r--r--   0        0        0    21027 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rate.py
--rw-r--r--   0        0        0     1040 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcconfiguration.py
--rw-r--r--   0        0        0     6531 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcdatachannel.py
--rw-r--r--   0        0        0    13595 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcdtlstransport.py
--rw-r--r--   0        0        0    11425 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcicetransport.py
--rw-r--r--   0        0        0    32180 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcpeerconnection.py
--rw-r--r--   0        0        0     4612 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcrtpparameters.py
--rw-r--r--   0        0        0    61599 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcsctptransport.py
--rw-r--r--   0        0        0      500 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtcsessiondescription.py
--rw-r--r--   0        0        0    24050 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/rtp.py
--rw-r--r--   0        0        0    21763 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/sdp.py
--rw-r--r--   0        0        0     2879 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/stats.py
--rw-r--r--   0        0        0      978 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/aiortc/utils.py
--rw-r--r--   0        0        0      716 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/messages.py
--rw-r--r--   0        0        0    21803 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/peer.py
--rw-r--r--   0        0        0        0 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/py.typed
--rw-r--r--   0        0        0     2144 2024-04-10 06:38:19.579817 fleece_network-0.2.0rc2/fleece_network/signaling.py
--rw-r--r--   0        0        0      479 2024-04-10 06:38:19.583817 fleece_network-0.2.0rc2/pyproject.toml
--rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 fleece_network-0.2.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      327 2024-04-12 12:24:35.837670 fleece_network-0.2.0rc3/README.md
+-rw-r--r--   0        0        0        0 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/__init__.py
+-rw-r--r--   0        0        0      349 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aioice/__init__.py
+-rw-r--r--   0        0        0     4060 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aioice/candidate.py
+-rw-r--r--   0        0        0    41823 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aioice/ice.py
+-rw-r--r--   0        0        0     6655 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aioice/mdns.py
+-rw-r--r--   0        0        0    12369 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aioice/stun.py
+-rw-r--r--   0        0        0    15077 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aioice/turn.py
+-rw-r--r--   0        0        0      264 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aioice/utils.py
+-rw-r--r--   0        0        0     1226 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/__init__.py
+-rw-r--r--   0        0        0      824 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/clock.py
+-rw-r--r--   0        0        0      180 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/exceptions.py
+-rw-r--r--   0        0        0    21027 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rate.py
+-rw-r--r--   0        0        0     1040 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcconfiguration.py
+-rw-r--r--   0        0        0     6531 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcdatachannel.py
+-rw-r--r--   0        0        0    13595 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcdtlstransport.py
+-rw-r--r--   0        0        0    11425 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcicetransport.py
+-rw-r--r--   0        0        0    32180 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcpeerconnection.py
+-rw-r--r--   0        0        0     4612 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcrtpparameters.py
+-rw-r--r--   0        0        0    61924 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcsctptransport.py
+-rw-r--r--   0        0        0      500 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtcsessiondescription.py
+-rw-r--r--   0        0        0    24050 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/rtp.py
+-rw-r--r--   0        0        0    21763 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/sdp.py
+-rw-r--r--   0        0        0     2879 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/stats.py
+-rw-r--r--   0        0        0      978 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/aiortc/utils.py
+-rw-r--r--   0        0        0      716 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/messages.py
+-rw-r--r--   0        0        0    21803 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/peer.py
+-rw-r--r--   0        0        0        0 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/py.typed
+-rw-r--r--   0        0        0     2144 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/fleece_network/signaling.py
+-rw-r--r--   0        0        0      479 2024-04-12 12:24:35.841670 fleece_network-0.2.0rc3/pyproject.toml
+-rw-r--r--   0        0        0      983 1970-01-01 00:00:00.000000 fleece_network-0.2.0rc3/PKG-INFO
```

### Comparing `fleece_network-0.2.0rc2/fleece_network/aioice/candidate.py` & `fleece_network-0.2.0rc3/fleece_network/aioice/candidate.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aioice/ice.py` & `fleece_network-0.2.0rc3/fleece_network/aioice/ice.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 logger = logging.getLogger(__name__)
 
 ICE_COMPLETED = 1
 ICE_FAILED = 2
 
 CONSENT_DELAY = 0.4
-CONSENT_ALPHA = 0.9
+CONSENT_ALPHA = 0.8
 CONSENT_FAILURES = 3
 CONSENT_INTERVAL = 5
 
 connection_id = count()
 protocol_id = count()
 
 _mdns = threading.local()
@@ -1017,26 +1017,28 @@
                     await pair.protocol.request(
                         request,
                         pair.remote_addr,
                         integrity_key=self.remote_password.encode("utf8"),
                         retransmissions=0,
                         delay=delay * 2,
                     )
-                    end = time.time()
+                    delta = time.time() - begin
                     failures = 0
                 except stun.TransactionError:
+                    delta = 2 * delay
                     failures += 1
-                    self.__log_info("Fail with consent delay %s", delay)
+                    self.__log_info("Fail with consent delay %s, %s", delay, delta)
                 if failures >= CONSENT_FAILURES:
                     self.__log_info("Consent to send expired")
                     self._query_consent_task = None
                     return await self.close()
 
                 # adjust adaptive delay
-                delay = delay * alpha + (1 - alpha) * (end - begin)
+                delay = max(delay * alpha + (1 - alpha) * delta, CONSENT_DELAY)
+                self.__log_info("Delay %s, delta %s", delay, delta)
 
     def data_received(self, data: bytes, component: int) -> None:
         self._queue.put_nowait((data, component))
 
     def request_received(
         self,
         message: stun.Message,
```

### Comparing `fleece_network-0.2.0rc2/fleece_network/aioice/mdns.py` & `fleece_network-0.2.0rc3/fleece_network/aioice/mdns.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aioice/stun.py` & `fleece_network-0.2.0rc3/fleece_network/aioice/stun.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aioice/turn.py` & `fleece_network-0.2.0rc3/fleece_network/aioice/turn.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aiortc/__init__.py` & `fleece_network-0.2.0rc3/fleece_network/aiortc/__init__.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aiortc/clock.py` & `fleece_network-0.2.0rc3/fleece_network/aiortc/clock.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aiortc/rate.py` & `fleece_network-0.2.0rc3/fleece_network/aiortc/rate.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aiortc/rtcconfiguration.py` & `fleece_network-0.2.0rc3/fleece_network/aiortc/rtcconfiguration.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aiortc/rtcdatachannel.py` & `fleece_network-0.2.0rc3/fleece_network/aiortc/rtcdatachannel.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aiortc/rtcdtlstransport.py` & `fleece_network-0.2.0rc3/fleece_network/aiortc/rtcdtlstransport.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aiortc/rtcicetransport.py` & `fleece_network-0.2.0rc3/fleece_network/aiortc/rtcicetransport.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aiortc/rtcpeerconnection.py` & `fleece_network-0.2.0rc3/fleece_network/aiortc/rtcpeerconnection.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aiortc/rtcrtpparameters.py` & `fleece_network-0.2.0rc3/fleece_network/aiortc/rtcrtpparameters.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aiortc/rtcsctptransport.py` & `fleece_network-0.2.0rc3/fleece_network/aiortc/rtcsctptransport.py`

 * *Files 0% similar despite different names*

```diff
@@ -494,30 +494,39 @@
 }
 
 
 class InboundStream:
     def __init__(self) -> None:
         self.reassembly: List[DataChunk] = []
         self.sequence_number = 0
+        self.has_last = False
+    
+    def check_last(self, flags: int): 
+        if flags & SCTP_DATA_LAST_FRAG: 
+            self.has_last = True 
 
     def add_chunk(self, chunk: DataChunk) -> None:
         if not self.reassembly or uint32_gt(chunk.tsn, self.reassembly[-1].tsn):
+            self.check_last(chunk.flags)
             self.reassembly.append(chunk)
             return
 
         for i, rchunk in enumerate(self.reassembly):
             # should never happen, the chunk should have been eliminated
             # as a duplicate when _mark_received() is called
             assert rchunk.tsn != chunk.tsn, "duplicate chunk in reassembly"
 
             if uint32_gt(rchunk.tsn, chunk.tsn):
+                self.check_last(chunk.flags)
                 self.reassembly.insert(i, chunk)
                 break
 
     def pop_messages(self) -> Iterator[Tuple[int, int, bytes]]:
+        if not self.has_last: 
+            return 
         pos = 0
         start_pos = None
         while pos < len(self.reassembly):
             chunk = self.reassembly[pos]
             if start_pos is None:
                 ordered = not (chunk.flags & SCTP_DATA_UNORDERED)
                 if not (chunk.flags & SCTP_DATA_FIRST_FRAG):
@@ -549,14 +558,16 @@
                     self.sequence_number = uint16_add(self.sequence_number, 1)
                 pos = start_pos
                 yield (chunk.stream_id, chunk.protocol, user_data)
             else:
                 pos += 1
 
             expected_tsn = tsn_plus_one(expected_tsn)
+        
+        self.has_last = False
 
     def prune_chunks(self, tsn: int) -> int:
         """
         Prune chunks up to the given TSN.
         """
         pos = -1
         size = 0
```

### Comparing `fleece_network-0.2.0rc2/fleece_network/aiortc/rtp.py` & `fleece_network-0.2.0rc3/fleece_network/aiortc/rtp.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aiortc/sdp.py` & `fleece_network-0.2.0rc3/fleece_network/aiortc/sdp.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aiortc/stats.py` & `fleece_network-0.2.0rc3/fleece_network/aiortc/stats.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/aiortc/utils.py` & `fleece_network-0.2.0rc3/fleece_network/aiortc/utils.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/messages.py` & `fleece_network-0.2.0rc3/fleece_network/messages.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/peer.py` & `fleece_network-0.2.0rc3/fleece_network/peer.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/fleece_network/signaling.py` & `fleece_network-0.2.0rc3/fleece_network/signaling.py`

 * *Files identical despite different names*

### Comparing `fleece_network-0.2.0rc2/PKG-INFO` & `fleece_network-0.2.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fleece-network
-Version: 0.2.0rc2
+Version: 0.2.0rc3
 Summary: P2P socket built on aiortc.
 Author: Linyu Wu
 Author-email: celve03@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

