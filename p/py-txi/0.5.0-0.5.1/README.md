# Comparing `tmp/py-txi-0.5.0.tar.gz` & `tmp/py-txi-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-txi-0.5.0.tar", last modified: Tue Mar  5 03:32:29 2024, max compression
+gzip compressed data, was "py-txi-0.5.1.tar", last modified: Sat Apr 13 09:10:16 2024, max compression
```

## Comparing `py-txi-0.5.0.tar` & `py-txi-0.5.1.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 03:32:29.659366 py-txi-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-05 03:32:29.659366 py-txi-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-03-05 03:32:16.000000 py-txi-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 03:32:29.659366 py-txi-0.5.0/py_txi/
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-05 03:32:16.000000 py-txi-0.5.0/py_txi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6246 2024-03-05 03:32:16.000000 py-txi-0.5.0/py_txi/docker_inference_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-03-05 03:32:16.000000 py-txi-0.5.0/py_txi/text_embedding_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)     3468 2024-03-05 03:32:16.000000 py-txi-0.5.0/py_txi/text_generation_inference.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-03-05 03:32:16.000000 py-txi-0.5.0/py_txi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 03:32:29.659366 py-txi-0.5.0/py_txi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-03-05 03:32:29.000000 py-txi-0.5.0/py_txi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-03-05 03:32:29.000000 py-txi-0.5.0/py_txi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 03:32:29.000000 py-txi-0.5.0/py_txi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-05 03:32:29.000000 py-txi-0.5.0/py_txi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-05 03:32:29.000000 py-txi-0.5.0/py_txi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      367 2024-03-05 03:32:16.000000 py-txi-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 03:32:29.659366 py-txi-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      978 2024-03-05 03:32:16.000000 py-txi-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:10:16.663463 py-txi-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-13 09:10:04.000000 py-txi-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-13 09:10:16.663463 py-txi-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-13 09:10:04.000000 py-txi-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:10:16.663463 py-txi-0.5.1/py_txi/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-13 09:10:04.000000 py-txi-0.5.1/py_txi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6615 2024-04-13 09:10:04.000000 py-txi-0.5.1/py_txi/inference_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2202 2024-04-13 09:10:04.000000 py-txi-0.5.1/py_txi/text_embedding_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2024-04-13 09:10:04.000000 py-txi-0.5.1/py_txi/text_generation_inference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-13 09:10:04.000000 py-txi-0.5.1/py_txi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 09:10:16.663463 py-txi-0.5.1/py_txi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-04-13 09:10:16.000000 py-txi-0.5.1/py_txi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-13 09:10:16.000000 py-txi-0.5.1/py_txi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 09:10:16.000000 py-txi-0.5.1/py_txi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-13 09:10:16.000000 py-txi-0.5.1/py_txi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-13 09:10:16.000000 py-txi-0.5.1/py_txi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      367 2024-04-13 09:10:04.000000 py-txi-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 09:10:16.663463 py-txi-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-13 09:10:04.000000 py-txi-0.5.1/setup.py
```

### Comparing `py-txi-0.5.0/PKG-INFO` & `py-txi-0.5.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: py-txi
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python wrapper around TGI and TEI servers
 Home-page: https://github.com/IlyasMoutawwakil/py-txi
 Author: Ilyas Moutawwakil
 Author-email: ilyas.moutawwakil@gmail.com
 Keywords: tgi,llm,tei,embedding,huggingface,docker,python
 Platform: linux
 Platform: windows
 Platform: macos
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 Provides-Extra: quality
 Provides-Extra: testing
+License-File: LICENSE
 
 # Py-TXI (previously Py-TGI)
 
 [![PyPI version](https://badge.fury.io/py/py-txi.svg)](https://badge.fury.io/py/py-txi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-txi)](https://pypi.org/project/py-txi/)
 [![PyPI - Format](https://img.shields.io/pypi/format/py-txi)](https://pypi.org/project/py-txi/)
 [![Downloads](https://pepy.tech/badge/py-txi)](https://pepy.tech/project/py-txi)
 [![PyPI - License](https://img.shields.io/pypi/l/py-txi)](https://pypi.org/project/py-txi/)
-[![Tests](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/tests.yaml/badge.svg)](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/tests.yaml)
+[![Test](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/test.yaml/badge.svg)](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/tests.yaml)
 
 Py-TXI is a Python wrapper around [Text-Generation-Inference](https://github.com/huggingface/text-generation-inference) and [Text-Embedding-Inference](https://github.com/huggingface/text-embeddings-inference) that enables creating and running TGI/TEI instances through the awesome `docker-py` in a similar style to Transformers API.
 
 ## Installation
 
 ```bash
 pip install py-txi
@@ -35,26 +36,26 @@
 Py-TXI is designed to be used in a similar way to Transformers API. We use `docker-py` (instead of a dirty `subprocess` solution) so that the containers you run are linked to the main process and are stopped automatically when your code finishes or fails.
 
 ## Usage
 
 Here's an example of how to use it:
 
 ```python
-from py_txi import TGI, is_nvidia_system, is_rocm_system
+from py_txi import TGI, TGIConfig
 
 llm = TGI(config=TGIConfig(sharded="false"))
 output = llm.generate(["Hi, I'm a language model", "I'm fine, how are you?"])
 print("LLM:", output)
 llm.close()
 ```
 
 Output: ```LLM: ["er. I'm a language modeler. I'm a language modeler. I'm a language", " I'm fine, how are you? I'm fine, how are you? I'm fine,"]```
 
 ```python
-from py_txi import TEI, is_nvidia_system
+from py_txi import TEI, TEIConfig
 
 embed = TEI(config=TEIConfig(pooling="cls"))
 output = embed.encode(["Hi, I'm an embedding model", "I'm fine, how are you?"])
 print("Embed:", output)
 embed.close()
 ```
```

### Comparing `py-txi-0.5.0/README.md` & `py-txi-0.5.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Py-TXI (previously Py-TGI)
 
 [![PyPI version](https://badge.fury.io/py/py-txi.svg)](https://badge.fury.io/py/py-txi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-txi)](https://pypi.org/project/py-txi/)
 [![PyPI - Format](https://img.shields.io/pypi/format/py-txi)](https://pypi.org/project/py-txi/)
 [![Downloads](https://pepy.tech/badge/py-txi)](https://pepy.tech/project/py-txi)
 [![PyPI - License](https://img.shields.io/pypi/l/py-txi)](https://pypi.org/project/py-txi/)
-[![Tests](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/tests.yaml/badge.svg)](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/tests.yaml)
+[![Test](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/test.yaml/badge.svg)](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/tests.yaml)
 
 Py-TXI is a Python wrapper around [Text-Generation-Inference](https://github.com/huggingface/text-generation-inference) and [Text-Embedding-Inference](https://github.com/huggingface/text-embeddings-inference) that enables creating and running TGI/TEI instances through the awesome `docker-py` in a similar style to Transformers API.
 
 ## Installation
 
 ```bash
 pip install py-txi
@@ -18,26 +18,26 @@
 Py-TXI is designed to be used in a similar way to Transformers API. We use `docker-py` (instead of a dirty `subprocess` solution) so that the containers you run are linked to the main process and are stopped automatically when your code finishes or fails.
 
 ## Usage
 
 Here's an example of how to use it:
 
 ```python
-from py_txi import TGI, is_nvidia_system, is_rocm_system
+from py_txi import TGI, TGIConfig
 
 llm = TGI(config=TGIConfig(sharded="false"))
 output = llm.generate(["Hi, I'm a language model", "I'm fine, how are you?"])
 print("LLM:", output)
 llm.close()
 ```
 
 Output: ```LLM: ["er. I'm a language modeler. I'm a language modeler. I'm a language", " I'm fine, how are you? I'm fine, how are you? I'm fine,"]```
 
 ```python
-from py_txi import TEI, is_nvidia_system
+from py_txi import TEI, TEIConfig
 
 embed = TEI(config=TEIConfig(pooling="cls"))
 output = embed.encode(["Hi, I'm an embedding model", "I'm fine, how are you?"])
 print("Embed:", output)
 embed.close()
 ```
```

### Comparing `py-txi-0.5.0/py_txi/docker_inference_server.py` & `py-txi-0.5.1/py_txi/inference_server.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 from huggingface_hub import AsyncInferenceClient
 
 from .utils import get_free_port
 
 basicConfig(level=INFO)
 
 DOCKER = docker.from_env()
-LOGGER = getLogger("docker-inference-server")
+LOGGER = getLogger("Inference-Server")
 
 
 @dataclass
-class DockerInferenceServerConfig:
+class InferenceServerConfig:
     # Image to use for the container
     image: str
     # Shared memory size for the container
     shm_size: str = "1g"
     # List of custom devices to forward to the container e.g. ["/dev/kfd", "/dev/dri"] for ROCm
     devices: Optional[List[str]] = None
     # NVIDIA-docker GPU device options e.g. "all" (all) or "0,1,2,3" (ids) or 4 (count)
@@ -40,28 +40,29 @@
         metadata={"help": "Dictionary of volumes to mount inside the container."},
     )
     environment: Dict[str, str] = field(
         default_factory=lambda: {"HUGGINGFACE_HUB_TOKEN": os.environ.get("HUGGINGFACE_HUB_TOKEN", "")},
         metadata={"help": "Dictionary of environment variables to forward to the container."},
     )
 
+    max_concurrent_requests: Optional[int] = None
     timeout: int = 60
 
     def __post_init__(self) -> None:
         if self.ports["80/tcp"][1] == 0:
             LOGGER.info("\t+ Getting a free port for the server")
             self.ports["80/tcp"] = (self.ports["80/tcp"][0], get_free_port())
 
 
-class DockerInferenceServer(ABC):
-    NAME: str = "Docker-Inference-Server"
+class InferenceServer(ABC):
+    NAME: str = "Inference-Server"
     SUCCESS_SENTINEL: str = "Success"
     FAILURE_SENTINEL: str = "Failure"
 
-    def __init__(self, config: DockerInferenceServerConfig) -> None:
+    def __init__(self, config: InferenceServerConfig) -> None:
         self.config = config
 
         try:
             LOGGER.info(f"\t+ Checking if {self.NAME} image is available locally")
             DOCKER.images.get(self.config.image)
             LOGGER.info(f"\t+ {self.NAME} image found locally")
         except docker.errors.ImageNotFound:
@@ -84,21 +85,21 @@
         else:
             LOGGER.info("\t+ Not using any GPU(s)")
             self.device_requests = None
 
         LOGGER.info(f"\t+ Building {self.NAME} command")
         self.command = []
         for k, v in asdict(self.config).items():
-            if k in DockerInferenceServerConfig.__annotations__:
+            if k in InferenceServerConfig.__annotations__:
                 continue
             elif v is not None:
                 if isinstance(v, bool):
                     self.command.append(f"--{k.replace('_', '-')}")
                 else:
-                    self.command.append(f"--{k.replace('_', '-')}={v}")
+                    self.command.append(f"--{k.replace('_', '-')}={str(v).lower()}")
 
         address, port = self.config.ports["80/tcp"]
         self.url = f"http://{address}:{port}"
 
         LOGGER.info(f"\t+ Running {self.NAME} container")
         self.container = DOCKER.containers.run(
             image=self.config.image,
@@ -121,14 +122,21 @@
                 break
             elif self.FAILURE_SENTINEL.lower() in log.lower():
                 LOGGER.info(f"\t {log}")
                 raise Exception(f"{self.NAME} server failed to start")
             else:
                 LOGGER.info(f"\t {log}")
 
+        try:
+            asyncio.set_event_loop(asyncio.get_event_loop())
+        except RuntimeError:
+            asyncio.set_event_loop(asyncio.new_event_loop())
+
+        self.semaphore = asyncio.Semaphore(self.config.max_concurrent_requests)
+
         LOGGER.info(f"\t+ Waiting for {self.NAME} server to be ready")
         start_time = time.time()
         while time.time() - start_time < self.config.timeout:
             try:
                 if not hasattr(self, "client"):
                     self.client = AsyncInferenceClient(model=self.url)
 
@@ -149,12 +157,16 @@
         if hasattr(self, "container"):
             LOGGER.info("\t+ Stoping Docker container")
             self.container.stop()
             self.container.wait()
             LOGGER.info("\t+ Docker container stopped")
             del self.container
 
+        if hasattr(self, "semaphore"):
+            self.semaphore
+            del self.semaphore
+
         if hasattr(self, "client"):
             del self.client
 
     def __del__(self) -> None:
         self.close()
```

### Comparing `py-txi-0.5.0/py_txi/text_embedding_inference.py` & `py-txi-0.5.1/py_txi/text_embedding_inference.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,56 +1,58 @@
 import asyncio
 from dataclasses import dataclass
 from logging import getLogger
 from typing import List, Literal, Optional, Union
 
 import numpy as np
 
-from .docker_inference_server import DockerInferenceServer, DockerInferenceServerConfig
+from .inference_server import InferenceServer, InferenceServerConfig
 from .utils import is_nvidia_system
 
-LOGGER = getLogger("TEI")
+LOGGER = getLogger("Text-Embedding-Inference")
 
 
 Pooling_Literal = Literal["cls", "mean"]
 DType_Literal = Literal["float32", "float16"]
 
 
-@dataclass(order=False)
-class TEIConfig(DockerInferenceServerConfig):
+@dataclass
+class TEIConfig(InferenceServerConfig):
     # Docker options
     image: str = "ghcr.io/huggingface/text-embeddings-inference:cpu-latest"
     # Launcher options
     model_id: str = "bert-base-uncased"
     revision: str = "main"
     dtype: Optional[DType_Literal] = None
     pooling: Optional[Pooling_Literal] = None
-    tokenization_workers: Optional[int] = None
+    # Concurrency options
+    max_concurrent_requests: int = 512
 
     def __post_init__(self) -> None:
         super().__post_init__()
 
         if is_nvidia_system() and "cpu" in self.image:
             LOGGER.warning(
                 "Your system has NVIDIA GPU, but you are using a CPU image."
                 "Consider using a GPU image for better performance."
             )
 
 
-class TEI(DockerInferenceServer):
+class TEI(InferenceServer):
     NAME: str = "Text-Embedding-Inference"
     SUCCESS_SENTINEL: str = "Ready"
     FAILURE_SENTINEL: str = "Error"
 
     def __init__(self, config: TEIConfig) -> None:
         super().__init__(config)
 
     async def single_client_call(self, text: str, **kwargs) -> np.ndarray:
-        output = await self.client.feature_extraction(text=text, **kwargs)
-        return output
+        async with self.semaphore:
+            output = await self.client.feature_extraction(text=text, **kwargs)
+            return output
 
     async def batch_client_call(self, text: List[str], **kwargs) -> List[np.ndarray]:
         output = await asyncio.gather(*[self.single_client_call(t, **kwargs) for t in text])
         return output
 
     def encode(self, text: Union[str, List[str]], **kwargs) -> Union[np.ndarray, List[np.ndarray]]:
         if isinstance(text, str):
```

### Comparing `py-txi-0.5.0/py_txi.egg-info/PKG-INFO` & `py-txi-0.5.1/py_txi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 Metadata-Version: 2.1
 Name: py-txi
-Version: 0.5.0
+Version: 0.5.1
 Summary: A Python wrapper around TGI and TEI servers
 Home-page: https://github.com/IlyasMoutawwakil/py-txi
 Author: Ilyas Moutawwakil
 Author-email: ilyas.moutawwakil@gmail.com
 Keywords: tgi,llm,tei,embedding,huggingface,docker,python
 Platform: linux
 Platform: windows
 Platform: macos
 Classifier: Programming Language :: Python :: 3
 Classifier: Natural Language :: English
 Description-Content-Type: text/markdown
 Provides-Extra: quality
 Provides-Extra: testing
+License-File: LICENSE
 
 # Py-TXI (previously Py-TGI)
 
 [![PyPI version](https://badge.fury.io/py/py-txi.svg)](https://badge.fury.io/py/py-txi)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/py-txi)](https://pypi.org/project/py-txi/)
 [![PyPI - Format](https://img.shields.io/pypi/format/py-txi)](https://pypi.org/project/py-txi/)
 [![Downloads](https://pepy.tech/badge/py-txi)](https://pepy.tech/project/py-txi)
 [![PyPI - License](https://img.shields.io/pypi/l/py-txi)](https://pypi.org/project/py-txi/)
-[![Tests](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/tests.yaml/badge.svg)](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/tests.yaml)
+[![Test](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/test.yaml/badge.svg)](https://github.com/IlyasMoutawwakil/py-txi/actions/workflows/tests.yaml)
 
 Py-TXI is a Python wrapper around [Text-Generation-Inference](https://github.com/huggingface/text-generation-inference) and [Text-Embedding-Inference](https://github.com/huggingface/text-embeddings-inference) that enables creating and running TGI/TEI instances through the awesome `docker-py` in a similar style to Transformers API.
 
 ## Installation
 
 ```bash
 pip install py-txi
@@ -35,26 +36,26 @@
 Py-TXI is designed to be used in a similar way to Transformers API. We use `docker-py` (instead of a dirty `subprocess` solution) so that the containers you run are linked to the main process and are stopped automatically when your code finishes or fails.
 
 ## Usage
 
 Here's an example of how to use it:
 
 ```python
-from py_txi import TGI, is_nvidia_system, is_rocm_system
+from py_txi import TGI, TGIConfig
 
 llm = TGI(config=TGIConfig(sharded="false"))
 output = llm.generate(["Hi, I'm a language model", "I'm fine, how are you?"])
 print("LLM:", output)
 llm.close()
 ```
 
 Output: ```LLM: ["er. I'm a language modeler. I'm a language modeler. I'm a language", " I'm fine, how are you? I'm fine, how are you? I'm fine,"]```
 
 ```python
-from py_txi import TEI, is_nvidia_system
+from py_txi import TEI, TEIConfig
 
 embed = TEI(config=TEIConfig(pooling="cls"))
 output = embed.encode(["Hi, I'm an embedding model", "I'm fine, how are you?"])
 print("Embed:", output)
 embed.close()
 ```
```

### Comparing `py-txi-0.5.0/setup.py` & `py-txi-0.5.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
-PY_TXI_VERSION = "0.5.0"
+PY_TXI_VERSION = "0.5.1"
 
 common_setup_kwargs = {
     "author": "Ilyas Moutawwakil",
     "author_email": "ilyas.moutawwakil@gmail.com",
     "description": "A Python wrapper around TGI and TEI servers",
     "keywords": ["tgi", "llm", "tei", "embedding", "huggingface", "docker", "python"],
     "url": "https://github.com/IlyasMoutawwakil/py-txi",
```

