# Comparing `tmp/sae_lens-0.1.0.tar.gz` & `tmp/sae_lens-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-0.1.0.tar", max compression
+gzip compressed data, was "sae_lens-0.2.0.tar", max compression
```

## Comparing `sae_lens-0.1.0.tar` & `sae_lens-0.2.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1069 2024-04-06 14:44:03.134906 sae_lens-0.1.0/LICENSE
--rw-r--r--   0        0        0    14614 2024-04-06 14:44:03.134906 sae_lens-0.1.0/README.md
--rw-r--r--   0        0        0     1559 2024-04-06 14:44:04.134900 sae_lens-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      905 2024-04-06 14:44:04.134900 sae_lens-0.1.0/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15365 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0    19086 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0     2103 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/analysis/toolkit.py
--rw-r--r--   0        0        0    18275 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0        0 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/__init__.py
--rw-r--r--   0        0        0    16379 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     2837 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0     8258 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/config.py
--rw-r--r--   0        0        0     5760 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     1493 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     3675 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/optim.py
--rw-r--r--   0        0        0     6282 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     3464 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    11579 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3276 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    17362 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    16778 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     4888 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0     1543 2024-04-06 14:44:03.146906 sae_lens-0.1.0/sae_lens/training/utils.py
--rw-r--r--   0        0        0    15856 1970-01-01 00:00:00.000000 sae_lens-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-13 12:36:56.283827 sae_lens-0.2.0/LICENSE
+-rw-r--r--   0        0        0    14571 2024-04-13 12:36:56.283827 sae_lens-0.2.0/README.md
+-rw-r--r--   0        0        0     1585 2024-04-13 12:36:57.259824 sae_lens-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      943 2024-04-13 12:36:57.259824 sae_lens-0.2.0/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15355 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0      301 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    19076 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     4251 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0        0 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0    16559 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     2804 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0     8745 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/training/config.py
+-rw-r--r--   0        0        0     5732 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     1527 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     3675 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     7187 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2132 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    13294 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3276 2024-04-13 12:36:56.295827 sae_lens-0.2.0/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    17362 2024-04-13 12:36:56.299827 sae_lens-0.2.0/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    17227 2024-04-13 12:36:56.299827 sae_lens-0.2.0/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     4888 2024-04-13 12:36:56.299827 sae_lens-0.2.0/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0     1628 2024-04-13 12:36:56.299827 sae_lens-0.2.0/sae_lens/training/utils.py
+-rw-r--r--   0        0        0    15857 1970-01-01 00:00:00.000000 sae_lens-0.2.0/PKG-INFO
```

### Comparing `sae_lens-0.1.0/LICENSE` & `sae_lens-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-0.1.0/README.md` & `sae_lens-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 <img width="1308" alt="Screenshot 2024-03-21 at 3 08 28 pm" src="https://github.com/jbloomAus/mats_sae_training/assets/69127271/209012ec-a779-4036-b4be-7b7739ea87f6">
 
 # SAE Lens 
+[![PyPI](https://img.shields.io/pypi/v/sae-lens?color=blue)](https://pypi.org/project/sae-lens/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![build](https://github.com/jbloomAus/mats_sae_training/actions/workflows/build.yml/badge.svg)](https://github.com/jbloomAus/mats_sae_training/actions/workflows/build.yml)
-[![Deploy Docs](https://github.com/jbloomAus/mats_sae_training/actions/workflows/deploy_docs.yml/badge.svg)](https://github.com/jbloomAus/mats_sae_training/actions/workflows/deploy_docs.yml)
-[![codecov](https://codecov.io/gh/jbloomAus/mats_sae_training/graph/badge.svg?token=N83NGH8CGE)](https://codecov.io/gh/jbloomAus/mats_sae_training)
+[![build](https://github.com/jbloomAus/SAELens/actions/workflows/build.yml/badge.svg)](https://github.com/jbloomAus/SAELens/actions/workflows/build.yml)
+[![Deploy Docs](https://github.com/jbloomAus/SAELens/actions/workflows/deploy_docs.yml/badge.svg)](https://github.com/jbloomAus/SAELens/actions/workflows/deploy_docs.yml)
+[![codecov](https://codecov.io/gh/jbloomAus/SAELens/graph/badge.svg?token=N83NGH8CGE)](https://codecov.io/gh/jbloomAus/SAELens)
 
 SAELens exists to help researchers:
 - Train sparse autoencoders.
 - Analyse sparse autoencoders / research mechanistic interpretability. 
 - Generate insights which make it easier to create safe and aligned AI systems.
 
 ## Quick Start
 
 ### Set Up
 
-This project uses [Poetry](https://python-poetry.org/) for dependency management. Ensure Poetry is installed, then to install the dependencies, run:
+This package is available on PyPI. You can install it via pip:
 
 ```
-poetry install
+pip install sae-lens
 ```
 
 ### Loading Sparse Autoencoders from Huggingface
 
 [Previously trained sparse autoencoders](https://huggingface.co/jbloom/GPT2-Small-SAEs) can be loaded from huggingface with close to single line of code. For more details and performance metrics for these sparse autoencoder, read my [blog post](https://www.alignmentforum.org/posts/f9EgfLSurAiqRJySD/open-source-sparse-autoencoders-for-all-residual-stream). 
 
 ```python
```

### Comparing `sae_lens-0.1.0/pyproject.toml` & `sae_lens-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "0.1.0"
+version = "0.2.0"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -23,25 +23,27 @@
 sae-vis = "0.2.6"
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.5.15"
 mkdocs-autorefs = "^1.0.1"
 mkdocs-section-index = "^0.3.8"
 mkdocstrings = "^0.24.1"
 mkdocstrings-python = "^1.9.0"
+safetensors = "^0.4.2"
 
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.2.0"
 pytest = "^8.0.2"
 pytest-cov = "^4.1.0"
 pre-commit = "^3.6.2"
 flake8 = "^7.0.0"
 isort = "^5.13.2"
 pyright = "^1.1.351"
 
+
 [tool.isort]
 profile = "black"
 
 [tool.pyright]
 typeCheckingMode = "strict"
 reportMissingTypeStubs = "none"
 reportUnknownMemberType = "none"
@@ -50,19 +52,20 @@
 reportUntypedFunctionDecorator = "none"
 reportUnnecessaryIsInstance = "none"
 reportUnnecessaryComparison = "none"
 reportConstantRedefinition = "none"
 reportUnknownLambdaType = "none"
 reportPrivateUsage = "none"
 
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.semantic_release]
 version_variables = [
     "sae_lens/__init__.py:__version__",
     "pyproject.toml:version",
 ]
 branch = "main"
-build_command = "pip install poetry && poetry build"
+build_command = "pip install poetry && poetry build"
```

### Comparing `sae_lens-0.1.0/sae_lens/__init__.py` & `sae_lens-0.2.0/sae_lens/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-__version__ = "0.1.0"
+__version__ = "0.2.0"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import cache_activations_runner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
-from .training.sae_group import SAEGroup
+from .training.sae_group import SparseAutoencoderDictionary
 from .training.session_loader import LMSparseAutoencoderSessionloader
 from .training.sparse_autoencoder import SparseAutoencoder
 from .training.train_sae_on_language_model import train_sae_group_on_language_model
 
 __all__ = [
     "LanguageModelSAERunnerConfig",
     "CacheActivationsRunnerConfig",
     "LMSparseAutoencoderSessionloader",
     "SparseAutoencoder",
-    "SAEGroup",
+    "SparseAutoencoderDictionary",
     "run_evals",
     "language_model_sae_runner",
     "cache_activations_runner",
     "ActivationsStore",
     "train_sae_group_on_language_model",
 ]
```

### Comparing `sae_lens-0.1.0/sae_lens/analysis/dashboard_runner.py` & `sae_lens-0.2.0/sae_lens/analysis/dashboard_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,17 +130,17 @@
         return dashboard_folder_name
 
     def init_sae_session(self):
         (
             self.model,
             sae_group,
             self.activation_store,
-        ) = LMSparseAutoencoderSessionloader.load_session_from_pretrained(self.sae_path)
+        ) = LMSparseAutoencoderSessionloader.load_pretrained_sae(self.sae_path)
         # TODO: handle multiple autoencoders
-        self.sparse_autoencoder = sae_group.autoencoders[0]
+        self.sparse_autoencoder = next(iter(sae_group))[1]
 
     def get_tokens(
         self, n_batches_to_sample_from: int = 2**12, n_prompts_to_select: int = 4096 * 6
     ):
         """
         Get the tokens needed for dashboard generation.
         """
```

### Comparing `sae_lens-0.1.0/sae_lens/analysis/feature_statistics.py` & `sae_lens-0.2.0/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.1.0/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-0.2.0/sae_lens/analysis/neuronpedia_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,17 +90,17 @@
         return dashboard_folder_name
 
     def init_sae_session(self):
         (
             self.model,
             sae_group,
             self.activation_store,
-        ) = LMSparseAutoencoderSessionloader.load_session_from_pretrained(self.sae_path)
+        ) = LMSparseAutoencoderSessionloader.load_pretrained_sae(self.sae_path)
         # TODO: handle multiple autoencoders
-        self.sparse_autoencoder = sae_group.autoencoders[0]
+        self.sparse_autoencoder = next(iter(sae_group))[1]
 
     def get_tokens(
         self, n_batches_to_sample_from: int = 2**12, n_prompts_to_select: int = 4096 * 6
     ):
         all_tokens_list = []
         pbar = tqdm(range(n_batches_to_sample_from))
         for _ in pbar:
```

### Comparing `sae_lens-0.1.0/sae_lens/analysis/tsea.py` & `sae_lens-0.2.0/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.1.0/sae_lens/training/activations_store.py` & `sae_lens-0.2.0/sae_lens/training/activations_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,22 +29,23 @@
     """
 
     model: HookedTransformer
     dataset: HfDataset
     cached_activations_path: str | None
     tokens_column: Literal["tokens", "input_ids", "text"]
     hook_point_head_index: int | None
+    _dataloader: Iterator[Any] | None = None
+    _storage_buffer: torch.Tensor | None = None
 
     @classmethod
     def from_config(
         cls,
         model: HookedTransformer,
         cfg: LanguageModelSAERunnerConfig | CacheActivationsRunnerConfig,
         dataset: HfDataset | None = None,
-        create_dataloader: bool = True,
     ) -> "ActivationsStore":
         cached_activations_path = cfg.cached_activations_path
         # set cached_activations_path to None if we're not using cached activations
         if (
             isinstance(cfg, LanguageModelSAERunnerConfig)
             and not cfg.use_cached_activations
         ):
@@ -61,15 +62,14 @@
             total_training_tokens=cfg.total_training_tokens,
             store_batch_size=cfg.store_batch_size,
             train_batch_size=cfg.train_batch_size,
             prepend_bos=cfg.prepend_bos,
             device=cfg.device,
             dtype=cfg.dtype,
             cached_activations_path=cached_activations_path,
-            create_dataloader=create_dataloader,
         )
 
     def __init__(
         self,
         model: HookedTransformer,
         dataset: HfDataset | str,
         hook_point: str,
@@ -79,17 +79,16 @@
         d_in: int,
         n_batches_in_buffer: int,
         total_training_tokens: int,
         store_batch_size: int,
         train_batch_size: int,
         prepend_bos: bool,
         device: str | torch.device,
-        dtype: torch.dtype,
+        dtype: str | torch.dtype,
         cached_activations_path: str | None = None,
-        create_dataloader: bool = True,
     ):
         self.model = model
         self.dataset = (
             load_dataset(dataset, split="train", streaming=True)
             if isinstance(dataset, str)
             else dataset
         )
@@ -147,18 +146,25 @@
             n_activations_on_disk = buffer_size_on_disk * n_buffers_on_disk
             assert (
                 n_activations_on_disk > self.total_training_tokens
             ), f"Only {n_activations_on_disk/1e6:.1f}M activations on disk, but total_training_tokens is {self.total_training_tokens/1e6:.1f}M."
 
             # TODO add support for "mixed loading" (ie use cache until you run out, then switch over to streaming from HF)
 
-        if create_dataloader:
-            # fill buffer half a buffer, so we can mix it with a new buffer
-            self.storage_buffer = self.get_buffer(self.n_batches_in_buffer // 2)
-            self.dataloader = self.get_data_loader()
+    @property
+    def storage_buffer(self) -> torch.Tensor:
+        if self._storage_buffer is None:
+            self._storage_buffer = self.get_buffer(self.n_batches_in_buffer // 2)
+        return self._storage_buffer
+
+    @property
+    def dataloader(self) -> Iterator[Any]:
+        if self._dataloader is None:
+            self._dataloader = self.get_data_loader()
+        return self._dataloader
 
     def get_batch_tokens(self):
         """
         Streams a batch of tokens from a dataset.
         """
 
         batch_size = self.store_batch_size
@@ -255,28 +261,28 @@
             ]
 
         # Stack along a new dimension to keep separate layers distinct
         stacked_activations = torch.stack(activations_list, dim=2)
 
         return stacked_activations
 
-    def get_buffer(self, n_batches_in_buffer: int):
+    def get_buffer(self, n_batches_in_buffer: int) -> torch.Tensor:
         context_size = self.context_size
         batch_size = self.store_batch_size
         d_in = self.d_in
         total_size = batch_size * n_batches_in_buffer
         num_layers = len(self.hook_point_layers)  # Number of hook points or layers
 
         if self.cached_activations_path is not None:
             # Load the activations from disk
             buffer_size = total_size * context_size
             # Initialize an empty tensor with an additional dimension for layers
             new_buffer = torch.zeros(
                 (buffer_size, num_layers, d_in),
-                dtype=self.dtype,
+                dtype=self.dtype,  # type: ignore
                 device=self.device,
             )
             n_tokens_filled = 0
 
             # Assume activations for different layers are stored separately and need to be combined
             while n_tokens_filled < buffer_size:
                 if not os.path.exists(
@@ -319,15 +325,15 @@
 
             return new_buffer
 
         refill_iterator = range(0, batch_size * n_batches_in_buffer, batch_size)
         # Initialize empty tensor buffer of the maximum required size with an additional dimension for layers
         new_buffer = torch.zeros(
             (total_size, context_size, num_layers, d_in),
-            dtype=self.dtype,
+            dtype=self.dtype,  # type: ignore
             device=self.device,
         )
 
         for refill_batch_idx_start in refill_iterator:
             refill_batch_tokens = self.get_batch_tokens()
             refill_activations = self.get_activations(refill_batch_tokens)
             new_buffer[
@@ -359,15 +365,15 @@
             [self.get_buffer(self.n_batches_in_buffer // 2), self.storage_buffer],
             dim=0,
         )
 
         mixing_buffer = mixing_buffer[torch.randperm(mixing_buffer.shape[0])]
 
         # 2.  put 50 % in storage
-        self.storage_buffer = mixing_buffer[: mixing_buffer.shape[0] // 2]
+        self._storage_buffer = mixing_buffer[: mixing_buffer.shape[0] // 2]
 
         # 3. put other 50 % in a dataloader
         dataloader = iter(
             DataLoader(
                 # TODO: seems like a typing bug?
                 cast(Any, mixing_buffer[mixing_buffer.shape[0] // 2 :]),
                 batch_size=batch_size,
@@ -383,15 +389,15 @@
         If the DataLoader is exhausted, refill the buffer and create a new DataLoader.
         """
         try:
             # Try to get the next batch
             return next(self.dataloader)
         except StopIteration:
             # If the DataLoader is exhausted, create a new one
-            self.dataloader = self.get_data_loader()
+            self._dataloader = self.get_data_loader()
             return next(self.dataloader)
 
     def _get_next_dataset_tokens(self) -> torch.Tensor:
         device = self.device
         if not self.is_dataset_tokenized:
             s = next(self.iterable_dataset)[self.tokens_column]
             tokens = self.model.to_tokens(
```

### Comparing `sae_lens-0.1.0/sae_lens/training/cache_activations_runner.py` & `sae_lens-0.2.0/sae_lens/training/cache_activations_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 
 def cache_activations_runner(cfg: CacheActivationsRunnerConfig):
     model = HookedTransformer.from_pretrained(cfg.model_name)
     model.to(cfg.device)
     activations_store = ActivationsStore.from_config(
         model,
         cfg,
-        create_dataloader=False,
     )
 
     # if the activations directory exists and has files in it, raise an exception
     assert activations_store.cached_activations_path is not None
     if os.path.exists(activations_store.cached_activations_path):
         if len(os.listdir(activations_store.cached_activations_path)) > 0:
             raise Exception(
```

### Comparing `sae_lens-0.1.0/sae_lens/training/config.py` & `sae_lens-0.2.0/sae_lens/training/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from dataclasses import dataclass
 from typing import Any, Optional, cast
 
 import torch
 
 import wandb
 
+DTYPE_MAP = {
+    "torch.float32": torch.float32,
+    "torch.float64": torch.float64,
+    "torch.float16": torch.float16,
+    "torch.bfloat16": torch.bfloat16,
+}
+
 
 @dataclass
 class LanguageModelSAERunnerConfig:
     """
     Configuration for training a sparse autoencoder on a language model.
     """
 
@@ -33,15 +40,15 @@
     total_training_tokens: int = 2_000_000
     store_batch_size: int = 32
     train_batch_size: int = 4096
 
     # Misc
     device: str | torch.device = "cpu"
     seed: int = 42
-    dtype: torch.dtype = torch.float32
+    dtype: str | torch.dtype = "float32"  # type: ignore #
     prepend_bos: bool = True
 
     # SAE Parameters
     b_dec_init_method: str = "geometric_median"
     expansion_factor: int | list[int] = 4
     from_pretrained_path: Optional[str] = None
     d_sae: Optional[int] = None
@@ -105,14 +112,21 @@
                 f"b_dec_init_method must be geometric_median, mean, or zeros. Got {self.b_dec_init_method}"
             )
         if self.b_dec_init_method == "zeros":
             print(
                 "Warning: We are initializing b_dec to zeros. This is probably not what you want."
             )
 
+        if isinstance(self.dtype, str) and self.dtype not in DTYPE_MAP:
+            raise ValueError(
+                f"dtype must be one of {list(DTYPE_MAP.keys())}. Got {self.dtype}"
+            )
+        elif isinstance(self.dtype, str):
+            self.dtype: torch.dtype = DTYPE_MAP[self.dtype]
+
         self.device: str | torch.device = torch.device(self.device)
 
         if self.lr_end is None:
             if isinstance(self.lr, list):
                 self.lr_end = [lr / 10 for lr in self.lr]
             else:
                 self.lr_end = self.lr / 10
@@ -191,15 +205,15 @@
     total_training_tokens: int = 2_000_000
     store_batch_size: int = 32
     train_batch_size: int = 4096
 
     # Misc
     device: str | torch.device = "cpu"
     seed: int = 42
-    dtype: torch.dtype = torch.float32
+    dtype: str | torch.dtype = "float32"
     prepend_bos: bool = True
 
     # Activation caching stuff
     shuffle_every_n_buffers: int = 10
     n_shuffles_with_last_section: int = 10
     n_shuffles_in_entire_dir: int = 10
     n_shuffles_final: int = 100
```

### Comparing `sae_lens-0.1.0/sae_lens/training/evals.py` & `sae_lens-0.2.0/sae_lens/training/evals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from functools import partial
 from typing import Any, Mapping, cast
 
 import pandas as pd
 import torch
-from tqdm import tqdm
 from transformer_lens import HookedTransformer
 from transformer_lens.utils import get_act_name
 
 import wandb
 from sae_lens.training.activations_store import ActivationsStore
 from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 
@@ -88,15 +87,15 @@
 def recons_loss_batched(
     sparse_autoencoder: SparseAutoencoder,
     model: HookedTransformer,
     activation_store: ActivationsStore,
     n_batches: int = 100,
 ):
     losses = []
-    for _ in tqdm(range(n_batches)):
+    for _ in range(n_batches):
         batch_tokens = activation_store.get_batch_tokens()
         score, loss, recons_loss, zero_abl_loss = get_recons_loss(
             sparse_autoencoder, model, batch_tokens
         )
         losses.append(
             (
                 score.mean().item(),
```

### Comparing `sae_lens-0.1.0/sae_lens/training/geometric_median.py` & `sae_lens-0.2.0/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.1.0/sae_lens/training/lm_runner.py` & `sae_lens-0.2.0/sae_lens/training/lm_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,21 +12,23 @@
     """ """
 
     if cfg.from_pretrained_path is not None:
         (
             model,
             sparse_autoencoder,
             activations_loader,
-        ) = LMSparseAutoencoderSessionloader.load_session_from_pretrained(
+        ) = LMSparseAutoencoderSessionloader.load_pretrained_sae(
             cfg.from_pretrained_path
         )
         cfg = sparse_autoencoder.cfg
     else:
         loader = LMSparseAutoencoderSessionloader(cfg)
-        model, sparse_autoencoder, activations_loader = loader.load_session()
+        model, sparse_autoencoder, activations_loader = (
+            loader.load_sae_training_group_session()
+        )
 
     if cfg.log_to_wandb:
         wandb.init(project=cfg.wandb_project, config=cast(Any, cfg), name=cfg.run_name)
 
     # train SAE
     sparse_autoencoder = train_sae_on_language_model(
         model,
```

### Comparing `sae_lens-0.1.0/sae_lens/training/optim.py` & `sae_lens-0.2.0/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.1.0/sae_lens/training/session_loader.py` & `sae_lens-0.2.0/sae_lens/training/session_loader.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,102 +1,70 @@
 from typing import Tuple
 
 from transformer_lens import HookedTransformer
 
 from sae_lens.training.activations_store import ActivationsStore
 from sae_lens.training.config import LanguageModelSAERunnerConfig
-from sae_lens.training.sae_group import SAEGroup
+from sae_lens.training.sae_group import SparseAutoencoderDictionary
 from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 
 
 class LMSparseAutoencoderSessionloader:
     """
     Responsible for loading all required
     artifacts and files for training
     a sparse autoencoder on a language model
     or analysing a pretraining autoencoder
     """
 
     def __init__(self, cfg: LanguageModelSAERunnerConfig):
         self.cfg = cfg
 
-    def load_session(
+    def load_sae_training_group_session(
         self,
-    ) -> Tuple[HookedTransformer, SAEGroup, ActivationsStore]:
+    ) -> Tuple[HookedTransformer, SparseAutoencoderDictionary, ActivationsStore]:
         """
         Loads a session for training a sparse autoencoder on a language model.
         """
 
         model = self.get_model(self.cfg.model_name)
         model.to(self.cfg.device)
-        activations_loader = self.get_activations_loader(self.cfg, model)
-        sparse_autoencoder = self.initialize_sparse_autoencoder(self.cfg)
+        activations_loader = ActivationsStore.from_config(
+            model,
+            self.cfg,
+        )
 
-        return model, sparse_autoencoder, activations_loader
+        sae_group = SparseAutoencoderDictionary(self.cfg)
+
+        return model, sae_group, activations_loader
 
     @classmethod
-    def load_session_from_pretrained(
+    def load_pretrained_sae(
         cls, path: str
-    ) -> Tuple[HookedTransformer, SAEGroup, ActivationsStore]:
+    ) -> Tuple[HookedTransformer, SparseAutoencoderDictionary, ActivationsStore]:
         """
-        Loads a session for analysing a pretrained sparse autoencoder group.
+        Loads a session for analysing a pretrained sparse autoencoder.
         """
-        # if torch.backends.mps.is_available():
-        #     cfg = torch.load(path, map_location="mps")["cfg"]
-        #     cfg.device = "mps"
-        # elif torch.cuda.is_available():
-        #     cfg = torch.load(path, map_location="cuda")["cfg"]
-        # else:
-        #     cfg = torch.load(path, map_location="cpu")["cfg"]
-
-        sparse_autoencoders = SAEGroup.load_from_pretrained(path)
-
-        # hacky code to deal with old SAE saves
-        if type(sparse_autoencoders) is dict:
-            sparse_autoencoder = SparseAutoencoder(cfg=sparse_autoencoders["cfg"])
-            sparse_autoencoder.load_state_dict(sparse_autoencoders["state_dict"])
-            model, sparse_autoencoders, activations_loader = cls(
-                sparse_autoencoder.cfg
-            ).load_session()
-            sparse_autoencoders.autoencoders[0] = sparse_autoencoder
-        elif type(sparse_autoencoders) is SAEGroup:
-            model, _, activations_loader = cls(sparse_autoencoders.cfg).load_session()
-        else:
-            raise ValueError(
-                "The loaded sparse_autoencoders object is neither an SAE dict nor a SAEGroup"
-            )
 
-        return model, sparse_autoencoders, activations_loader
+        # load the SAE
+        sparse_autoencoder = SparseAutoencoder.load_from_pretrained(path)
+
+        # load the model, SAE and activations loader with it.
+        session_loader = cls(sparse_autoencoder.cfg)
+        model, sae_group, activations_loader = (
+            session_loader.load_sae_training_group_session()
+        )
+
+        return model, sae_group, activations_loader
 
     def get_model(self, model_name: str):
         """
-        Loads a model from transformer lens
+        Loads a model from transformer lens.
+
+        Abstracted to allow for easy modification.
         """
 
         # Todo: add check that model_name is valid
 
         model = HookedTransformer.from_pretrained(model_name)
 
         return model
-
-    def initialize_sparse_autoencoder(self, cfg: LanguageModelSAERunnerConfig):
-        """
-        Initializes a sparse autoencoder group, which contains multiple sparse autoencoders
-        """
-
-        sparse_autoencoder = SAEGroup(cfg)
-
-        return sparse_autoencoder
-
-    def get_activations_loader(
-        self, cfg: LanguageModelSAERunnerConfig, model: HookedTransformer
-    ):
-        """
-        Loads a DataLoaderBuffer for the activations of a language model.
-        """
-
-        activations_loader = ActivationsStore.from_config(
-            model,
-            cfg,
-        )
-
-        return activations_loader
```

### Comparing `sae_lens-0.1.0/sae_lens/training/sparse_autoencoder.py` & `sae_lens-0.2.0/sae_lens/training/sparse_autoencoder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 """Most of this is just copied over from Arthur's code and slightly simplified:
 https://github.com/ArthurConmy/sae/blob/main/sae/model.py
 """
 
 import gzip
+import json
 import os
 import pickle
-from typing import NamedTuple
+from typing import NamedTuple, Optional
 
 import einops
 import torch
+from safetensors import safe_open
+from safetensors.torch import save_file
 from torch import nn
 from transformer_lens.hook_points import HookedRootModule, HookPoint
 
 from sae_lens.training.config import LanguageModelSAERunnerConfig
+from sae_lens.training.utils import BackwardsCompatiblePickleClass
 
 
 class ForwardOutput(NamedTuple):
     sae_out: torch.Tensor
     feature_acts: torch.Tensor
     loss: torch.Tensor
     mse_loss: torch.Tensor
@@ -196,56 +200,77 @@
         )
         self.W_dec.grad -= einops.einsum(
             parallel_component,
             self.W_dec.data,
             "d_sae, d_sae d_in -> d_sae d_in",
         )
 
-    def save_model(self, path: str):
+    def save_model_legacy(self, path: str):
         """
         Basic save function for the model. Saves the model's state_dict and the config used to train it.
         """
 
         # check if path exists
         folder = os.path.dirname(path)
         os.makedirs(folder, exist_ok=True)
 
         state_dict = {"cfg": self.cfg, "state_dict": self.state_dict()}
 
         if path.endswith(".pt"):
             torch.save(state_dict, path)
-        elif path.endswith(".pkl"):
-            with open(path, "wb") as f:
-                pickle.dump(state_dict, f)
-        elif path.endswith("pkl.gz"):
-            with gzip.open(path, "wb") as f:
-                pickle.dump(state_dict, f)
         else:
             raise ValueError(
                 f"Unexpected file extension: {path}, supported extensions are .pt and .pkl.gz"
             )
 
         print(f"Saved model to {path}")
 
+    def save_model(self, path: str, sparsity: Optional[torch.Tensor] = None):
+
+        if not os.path.exists(path):
+            os.mkdir(path)
+
+        # generate the weights
+        save_file(self.state_dict(), f"{path}/sae_weights.safetensors")
+
+        # save the config
+        config = {
+            **self.cfg.__dict__,
+            # some args may not be serializable by default
+            "dtype": str(self.cfg.dtype),
+            "device": str(self.cfg.device),
+        }
+
+        with open(f"{path}/cfg.json", "w") as f:
+            json.dump(config, f)
+
+        if sparsity is not None:
+            sparsity_in_dict = {"sparsity": sparsity}
+            save_file(sparsity_in_dict, f"{path}/sparsity.safetensors")  # type: ignore
+
     @classmethod
-    def load_from_pretrained(cls, path: str):
+    def load_from_pretrained_legacy(cls, path: str):
         """
         Load function for the model. Loads the model's state_dict and the config used to train it.
         This method can be called directly on the class, without needing an instance.
         """
 
         # Ensure the file exists
         if not os.path.isfile(path):
             raise FileNotFoundError(f"No file found at specified path: {path}")
 
         # Load the state dictionary
         if path.endswith(".pt"):
             try:
                 if torch.backends.mps.is_available():
-                    state_dict = torch.load(path, map_location="mps")
+                    state_dict = torch.load(
+                        path,
+                        map_location="mps",
+                        pickle_module=BackwardsCompatiblePickleClass,
+                    )
                     state_dict["cfg"].device = "mps"
                 else:
                     state_dict = torch.load(path)
             except Exception as e:
                 raise IOError(f"Error loading the state dictionary from .pt file: {e}")
 
         elif path.endswith(".pkl.gz"):
@@ -275,14 +300,39 @@
 
         # Create an instance of the class using the loaded configuration
         instance = cls(cfg=state_dict["cfg"])
         instance.load_state_dict(state_dict["state_dict"])
 
         return instance
 
+    @classmethod
+    def load_from_pretrained(cls, path: str, device: str = "cpu"):
+
+        config_path = os.path.join(path, "cfg.json")
+        weight_path = os.path.join(path, "sae_weights.safetensors")
+
+        with open(config_path, "r") as f:
+            config = json.load(f)
+
+        var_names = LanguageModelSAERunnerConfig.__init__.__code__.co_varnames
+        # filter config for varnames
+        config = {k: v for k, v in config.items() if k in var_names}
+        config["verbose"] = False
+        config["device"] = device
+        config = LanguageModelSAERunnerConfig(**config)
+        sae = SparseAutoencoder(config)
+
+        tensors = {}
+        with safe_open(weight_path, framework="pt", device=device) as f:  # type: ignore
+            for k in f.keys():
+                tensors[k] = f.get_tensor(k)
+        sae.load_state_dict(tensors)
+
+        return sae
+
     def get_name(self):
         sae_name = f"sparse_autoencoder_{self.cfg.model_name}_{self.cfg.hook_point}_{self.cfg.d_sae}"
         return sae_name
 
     def calculate_ghost_grad_loss(
         self,
         x: torch.Tensor,
@@ -322,8 +372,10 @@
     """
     Calculate MSE loss per item in the batch, without taking a mean.
     Then, normalizes by the L2 norm of the centered target.
     This normalization seems to improve performance.
     """
     target_centered = target - target.mean(dim=0, keepdim=True)
     normalization = target_centered.norm(dim=-1, keepdim=True)
-    return torch.nn.functional.mse_loss(preds, target, reduction="none") / normalization
+    return torch.nn.functional.mse_loss(preds, target, reduction="none") / (
+        normalization + 1e-6
+    )
```

### Comparing `sae_lens-0.1.0/sae_lens/training/toy_model_runner.py` & `sae_lens-0.2.0/sae_lens/training/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.1.0/sae_lens/training/toy_models.py` & `sae_lens-0.2.0/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.1.0/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-0.2.0/sae_lens/training/train_sae_on_language_model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,33 @@
+import os
 from dataclasses import dataclass
-from typing import Any, NamedTuple, cast
+from typing import Any, cast
 
 import torch
+from safetensors.torch import save_file
 from torch.optim import Adam, Optimizer
 from torch.optim.lr_scheduler import LRScheduler
 from tqdm import tqdm
 from transformer_lens import HookedTransformer
 
 import wandb
 from sae_lens.training.activations_store import ActivationsStore
 from sae_lens.training.evals import run_evals
 from sae_lens.training.geometric_median import compute_geometric_median
 from sae_lens.training.optim import get_scheduler
-from sae_lens.training.sae_group import SAEGroup
+from sae_lens.training.sae_group import SparseAutoencoderDictionary
 from sae_lens.training.sparse_autoencoder import SparseAutoencoder
 
 
+def _log_feature_sparsity(
+    feature_sparsity: torch.Tensor, eps: float = 1e-10
+) -> torch.Tensor:
+    return torch.log10(feature_sparsity + eps).detach().cpu()
+
+
 @dataclass
 class SAETrainContext:
     """
     Context to track during training for a single SAE
     """
 
     act_freq_scores: torch.Tensor
@@ -28,33 +36,37 @@
     optimizer: Optimizer
     scheduler: LRScheduler
 
     @property
     def feature_sparsity(self) -> torch.Tensor:
         return self.act_freq_scores / self.n_frac_active_tokens
 
+    @property
+    def log_feature_sparsity(self) -> torch.Tensor:
+        return _log_feature_sparsity(self.feature_sparsity)
+
 
 @dataclass
 class TrainSAEGroupOutput:
-    sae_group: SAEGroup
+    sae_group: SparseAutoencoderDictionary
     checkpoint_paths: list[str]
-    log_feature_sparsities: list[torch.Tensor]
+    log_feature_sparsities: dict[str, torch.Tensor]
 
 
 def train_sae_on_language_model(
     model: HookedTransformer,
-    sae_group: SAEGroup,
+    sae_group: SparseAutoencoderDictionary,
     activation_store: ActivationsStore,
     batch_size: int = 1024,
     n_checkpoints: int = 0,
     feature_sampling_window: int = 1000,  # how many training steps between resampling the features / considiring neurons dead
     dead_feature_threshold: float = 1e-8,  # how infrequently a feature has to be active to be considered dead
     use_wandb: bool = False,
     wandb_log_frequency: int = 50,
-) -> SAEGroup:
+) -> SparseAutoencoderDictionary:
     """
     @deprecated Use `train_sae_group_on_language_model` instead. This method is kept for backward compatibility.
     """
     return train_sae_group_on_language_model(
         model,
         sae_group,
         activation_store,
@@ -64,15 +76,15 @@
         use_wandb,
         wandb_log_frequency,
     ).sae_group
 
 
 def train_sae_group_on_language_model(
     model: HookedTransformer,
-    sae_group: SAEGroup,
+    sae_group: SparseAutoencoderDictionary,
     activation_store: ActivationsStore,
     batch_size: int = 1024,
     n_checkpoints: int = 0,
     feature_sampling_window: int = 1000,  # how many training steps between resampling the features / considiring neurons dead
     use_wandb: bool = False,
     wandb_log_frequency: int = 50,
 ) -> TrainSAEGroupOutput:
@@ -87,33 +99,33 @@
             range(0, total_training_tokens, total_training_tokens // n_checkpoints)
         )[1:]
 
     all_layers = sae_group.cfg.hook_point_layer
     if not isinstance(all_layers, list):
         all_layers = [all_layers]
 
-    train_contexts = [
-        _build_train_context(sae, total_training_steps) for sae in sae_group
-    ]
+    train_contexts = {
+        name: _build_train_context(sae, total_training_steps)
+        for name, sae in sae_group.autoencoders.items()
+    }
+
     _init_sae_group_b_decs(sae_group, activation_store, all_layers)
 
     pbar = tqdm(total=total_training_tokens, desc="Training SAE")
     checkpoint_paths: list[str] = []
     while n_training_tokens < total_training_tokens:
         # Do a training step.
         layer_acts = activation_store.next_batch()
         n_training_tokens += batch_size
 
         mse_losses: list[torch.Tensor] = []
         l1_losses: list[torch.Tensor] = []
 
-        for (
-            sparse_autoencoder,
-            ctx,
-        ) in zip(sae_group, train_contexts):
+        for name, sparse_autoencoder in sae_group.autoencoders.items():
+            ctx = train_contexts[name]
             wandb_suffix = _wandb_log_suffix(sae_group.cfg, sparse_autoencoder.cfg)
             step_output = _train_step(
                 sparse_autoencoder=sparse_autoencoder,
                 layer_acts=layer_acts,
                 ctx=ctx,
                 feature_sampling_window=feature_sampling_window,
                 use_wandb=use_wandb,
@@ -152,15 +164,15 @@
 
         # checkpoint if at checkpoint frequency
         if checkpoint_thresholds and n_training_tokens > checkpoint_thresholds[0]:
             checkpoint_path = _save_checkpoint(
                 sae_group,
                 train_contexts=train_contexts,
                 checkpoint_name=n_training_tokens,
-            ).path
+            )
             checkpoint_paths.append(checkpoint_path)
             checkpoint_thresholds.pop(0)
 
         ###############
 
         n_training_steps += 1
         pbar.set_description(
@@ -171,20 +183,24 @@
     # save final sae group to checkpoints folder
     final_checkpoint = _save_checkpoint(
         sae_group,
         train_contexts=train_contexts,
         checkpoint_name="final",
         wandb_aliases=["final_model"],
     )
-    checkpoint_paths.append(final_checkpoint.path)
+    checkpoint_paths.append(final_checkpoint)
+
+    log_feature_sparsities = {
+        name: ctx.log_feature_sparsity for name, ctx in train_contexts.items()
+    }
 
     return TrainSAEGroupOutput(
         sae_group=sae_group,
         checkpoint_paths=checkpoint_paths,
-        log_feature_sparsities=final_checkpoint.log_feature_sparsities,
+        log_feature_sparsities=log_feature_sparsities,
     )
 
 
 def _wandb_log_suffix(cfg: Any, hyperparams: Any):
     # Create a mapping from cfg list keys to their corresponding hyperparams attributes
     key_mapping = {
         "hook_point_layer": "layer",
@@ -251,21 +267,23 @@
         n_frac_active_tokens=n_frac_active_tokens,
         optimizer=optimizer,
         scheduler=scheduler,
     )
 
 
 def _init_sae_group_b_decs(
-    sae_group: SAEGroup, activation_store: ActivationsStore, all_layers: list[int]
+    sae_group: SparseAutoencoderDictionary,
+    activation_store: ActivationsStore,
+    all_layers: list[int],
 ) -> None:
     """
     extract all activations at a certain layer and use for sae b_dec initialization
     """
     geometric_medians = {}
-    for sae in sae_group:
+    for _, sae in sae_group:
         hyperparams = sae.cfg
         sae_layer_id = all_layers.index(sae.hook_point_layer)
         if hyperparams.b_dec_init_method == "geometric_median":
             layer_acts = activation_store.storage_buffer.detach()[:, sae_layer_id, :]
             # get geometric median of the activations if we're using those.
             if sae_layer_id not in geometric_medians:
                 median = compute_geometric_median(
@@ -420,53 +438,46 @@
         f"sparsity/mean_passes_since_fired{wandb_suffix}": ctx.n_forward_passes_since_fired.mean().item(),
         f"sparsity/dead_features{wandb_suffix}": ghost_grad_neuron_mask.sum().item(),
         f"details/current_learning_rate{wandb_suffix}": current_learning_rate,
         "details/n_training_tokens": n_training_tokens,
     }
 
 
-class SaveCheckpointOutput(NamedTuple):
-    path: str
-    log_feature_sparsity_path: str
-    log_feature_sparsities: list[torch.Tensor]
-
-
 def _save_checkpoint(
-    sae_group: SAEGroup,
-    train_contexts: list[SAETrainContext],
+    sae_group: SparseAutoencoderDictionary,
+    train_contexts: dict[str, SAETrainContext],
     checkpoint_name: int | str,
     wandb_aliases: list[str] | None = None,
-) -> SaveCheckpointOutput:
-    path = (
-        f"{sae_group.cfg.checkpoint_path}/{checkpoint_name}_{sae_group.get_name()}.pt"
-    )
-    for sae in sae_group:
+) -> str:
+
+    checkpoint_path = f"{sae_group.cfg.checkpoint_path}/{checkpoint_name}"
+    os.makedirs(checkpoint_path, exist_ok=True)
+    for name, sae in sae_group.autoencoders.items():
+
+        ctx = train_contexts[name]
+        path = f"{checkpoint_path}/{name}"
         sae.set_decoder_norm_to_unit_norm()
-    sae_group.save_model(path)
-    log_feature_sparsity_path = f"{sae_group.cfg.checkpoint_path}/{checkpoint_name}_{sae_group.get_name()}_log_feature_sparsity.pt"
-    log_feature_sparsities = [
-        _log_feature_sparsity(ctx.feature_sparsity) for ctx in train_contexts
-    ]
-    torch.save(log_feature_sparsities, log_feature_sparsity_path)
-    if sae_group.cfg.log_to_wandb:
-        model_artifact = wandb.Artifact(
-            f"{sae_group.get_name()}",
-            type="model",
-            metadata=dict(sae_group.cfg.__dict__),
-        )
-        model_artifact.add_file(path)
-        wandb.log_artifact(model_artifact, aliases=wandb_aliases)
+        sae.save_model(path)
+        log_feature_sparsities = {"sparsity": ctx.log_feature_sparsity}
 
-        sparsity_artifact = wandb.Artifact(
-            f"{sae_group.get_name()}_log_feature_sparsity",
-            type="log_feature_sparsity",
-            metadata=dict(sae_group.cfg.__dict__),
-        )
-        sparsity_artifact.add_file(log_feature_sparsity_path)
-        wandb.log_artifact(sparsity_artifact)
-    return SaveCheckpointOutput(path, log_feature_sparsity_path, log_feature_sparsities)
+        log_feature_sparsity_path = f"{path}/sparsity.safetensors"
+        save_file(log_feature_sparsities, log_feature_sparsity_path)
 
+        if sae_group.cfg.log_to_wandb and os.path.exists(log_feature_sparsity_path):
+            model_artifact = wandb.Artifact(
+                f"{sae_group.get_name()}",
+                type="model",
+                metadata=dict(sae_group.cfg.__dict__),
+            )
+            model_artifact.add_file(f"{path}/sae_weights.safetensors")
+            model_artifact.add_file(f"{path}/cfg.json")
+            wandb.log_artifact(model_artifact, aliases=wandb_aliases)
+
+            sparsity_artifact = wandb.Artifact(
+                f"{sae_group.get_name()}_log_feature_sparsity",
+                type="log_feature_sparsity",
+                metadata=dict(sae_group.cfg.__dict__),
+            )
+            sparsity_artifact.add_file(log_feature_sparsity_path)
+            wandb.log_artifact(sparsity_artifact)
 
-def _log_feature_sparsity(
-    feature_sparsity: torch.Tensor, eps: float = 1e-10
-) -> torch.Tensor:
-    return torch.log10(feature_sparsity + eps).detach().cpu()
+    return checkpoint_path
```

### Comparing `sae_lens-0.1.0/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-0.2.0/sae_lens/training/train_sae_on_toy_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.1.0/sae_lens/training/utils.py` & `sae_lens-0.2.0/sae_lens/training/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,14 +10,18 @@
     """
 
     def find_class(self, module: str, name: str):
         module = module.replace("sae_training", "sae_lens.training")
         return super().find_class(module, name)
 
 
+class BackwardsCompatiblePickleClass:
+    Unpickler = BackwardsCompatibleUnpickler
+
+
 def shuffle_activations_pairwise(datapath: str, buffer_idx_range: Tuple[int, int]):
     """
     Shuffles two buffers on disk.
     """
     assert (
         buffer_idx_range[0] < buffer_idx_range[1] - 1
     ), "buffer_idx_range[0] must be smaller than buffer_idx_range[1] by at least 1"
```

### Comparing `sae_lens-0.1.0/PKG-INFO` & `sae_lens-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 0.1.0
+Version: 0.2.0
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
@@ -21,39 +21,41 @@
 Requires-Dist: mkdocstrings (>=0.24.1,<0.25.0)
 Requires-Dist: mkdocstrings-python (>=1.9.0,<2.0.0)
 Requires-Dist: nbformat (>=5.9.2,<6.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: plotly (>=5.19.0,<6.0.0)
 Requires-Dist: plotly-express (>=0.4.1,<0.5.0)
 Requires-Dist: sae-vis (==0.2.6)
+Requires-Dist: safetensors (>=0.4.2,<0.5.0)
 Requires-Dist: transformer-lens (>=1.14.0,<2.0.0)
 Requires-Dist: transformers (>=4.38.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 <img width="1308" alt="Screenshot 2024-03-21 at 3 08 28 pm" src="https://github.com/jbloomAus/mats_sae_training/assets/69127271/209012ec-a779-4036-b4be-7b7739ea87f6">
 
 # SAE Lens 
+[![PyPI](https://img.shields.io/pypi/v/sae-lens?color=blue)](https://pypi.org/project/sae-lens/)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
-[![build](https://github.com/jbloomAus/mats_sae_training/actions/workflows/build.yml/badge.svg)](https://github.com/jbloomAus/mats_sae_training/actions/workflows/build.yml)
-[![Deploy Docs](https://github.com/jbloomAus/mats_sae_training/actions/workflows/deploy_docs.yml/badge.svg)](https://github.com/jbloomAus/mats_sae_training/actions/workflows/deploy_docs.yml)
-[![codecov](https://codecov.io/gh/jbloomAus/mats_sae_training/graph/badge.svg?token=N83NGH8CGE)](https://codecov.io/gh/jbloomAus/mats_sae_training)
+[![build](https://github.com/jbloomAus/SAELens/actions/workflows/build.yml/badge.svg)](https://github.com/jbloomAus/SAELens/actions/workflows/build.yml)
+[![Deploy Docs](https://github.com/jbloomAus/SAELens/actions/workflows/deploy_docs.yml/badge.svg)](https://github.com/jbloomAus/SAELens/actions/workflows/deploy_docs.yml)
+[![codecov](https://codecov.io/gh/jbloomAus/SAELens/graph/badge.svg?token=N83NGH8CGE)](https://codecov.io/gh/jbloomAus/SAELens)
 
 SAELens exists to help researchers:
 - Train sparse autoencoders.
 - Analyse sparse autoencoders / research mechanistic interpretability. 
 - Generate insights which make it easier to create safe and aligned AI systems.
 
 ## Quick Start
 
 ### Set Up
 
-This project uses [Poetry](https://python-poetry.org/) for dependency management. Ensure Poetry is installed, then to install the dependencies, run:
+This package is available on PyPI. You can install it via pip:
 
 ```
-poetry install
+pip install sae-lens
 ```
 
 ### Loading Sparse Autoencoders from Huggingface
 
 [Previously trained sparse autoencoders](https://huggingface.co/jbloom/GPT2-Small-SAEs) can be loaded from huggingface with close to single line of code. For more details and performance metrics for these sparse autoencoder, read my [blog post](https://www.alignmentforum.org/posts/f9EgfLSurAiqRJySD/open-source-sparse-autoencoders-for-all-residual-stream). 
 
 ```python
```

