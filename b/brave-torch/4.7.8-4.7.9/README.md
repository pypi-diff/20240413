# Comparing `tmp/brave_torch-4.7.8.tar.gz` & `tmp/brave_torch-4.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brave_torch-4.7.8.tar", max compression
+gzip compressed data, was "brave_torch-4.7.9.tar", max compression
```

## Comparing `brave_torch-4.7.8.tar` & `brave_torch-4.7.9.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1074 2024-04-11 18:47:37.313046 brave_torch-4.7.8/LICENSE
--rw-r--r--   0        0        0      853 2024-04-11 19:16:38.820857 brave_torch-4.7.8/README.md
--rw-r--r--   0        0        0      103 2024-04-11 19:16:04.253489 brave_torch-4.7.8/brave_torch/__init__.py
--rw-r--r--   0        0        0     6120 2024-04-11 19:10:27.521856 brave_torch-4.7.8/brave_torch/main.py
--rw-r--r--   0        0        0     1297 2024-04-11 19:15:16.958383 brave_torch-4.7.8/pyproject.toml
--rw-r--r--   0        0        0     1546 1970-01-01 00:00:00.000000 brave_torch-4.7.8/setup.py
--rw-r--r--   0        0        0     1871 1970-01-01 00:00:00.000000 brave_torch-4.7.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-04-11 18:47:37.313046 brave_torch-4.7.9/LICENSE
+-rw-r--r--   0        0        0     1048 2024-04-13 01:16:10.973092 brave_torch-4.7.9/README.md
+-rw-r--r--   0        0        0      103 2024-04-13 03:24:07.050681 brave_torch-4.7.9/brave_torch/__init__.py
+-rw-r--r--   0        0        0     5471 2024-04-13 03:29:45.492038 brave_torch-4.7.9/brave_torch/llm.py
+-rw-r--r--   0        0        0     8453 2024-04-13 03:23:46.470486 brave_torch-4.7.9/brave_torch/main.py
+-rw-r--r--   0        0        0     1315 2024-04-13 03:30:55.523759 brave_torch-4.7.9/pyproject.toml
+-rw-r--r--   0        0        0     1764 1970-01-01 00:00:00.000000 brave_torch-4.7.9/setup.py
+-rw-r--r--   0        0        0     2093 1970-01-01 00:00:00.000000 brave_torch-4.7.9/PKG-INFO
```

### Comparing `brave_torch-4.7.8/LICENSE` & `brave_torch-4.7.9/LICENSE`

 * *Files identical despite different names*

### Comparing `brave_torch-4.7.8/README.md` & `brave_torch-4.7.9/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 [![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)
 
 # BRAVE or Swarms of Vision Transformers
-Implementation of the paper: "BRAVE : Broadening the visual encoding of vision-language models". BRAVE achieves state-of-the-art performance on a broad range of captioning and VQA benchmarks and significantly reduces the aforementioned issues of VLMs, while requiring a smaller number of trainable parameters than existing methods and having a more compressed representation
+Implementation of the paper: "BRAVE : Broadening the visual encoding of vision-language models". BRAVE achieves state-of-the-art performance on a broad range of captioning and VQA benchmarks and significantly reduces the aforementioned issues of VLMs, while requiring a smaller number of trainable parameters than existing methods and having a more compressed representation.
 
 ## install
 `pip3 install brave-torch`
 
 
 ## usage
+
+### 
 ```python
 import torch
 from brave_torch.main import SwarmOfViTs
 
 # IMG Tensor
 x = torch.randn(1, 3, 224, 224) 
 
@@ -28,7 +30,14 @@
 # Forward
 out = model(x)
 print(out)
 ```
 
 # Citations
 
+## Todo
+- [ ] Citation link
+- [ ] Citation Bibtex
+- [ ] Diagram photo
+- [ ] Implement Andromeda Base LLM architecture
+- [ ] Provide multi-modal tokenizer
+- [ ] Train and release the model
```

### Comparing `brave_torch-4.7.8/brave_torch/main.py` & `brave_torch-4.7.9/brave_torch/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-import torch 
+import torch
 from torch import nn, Tensor
 from zeta import FeedForward
-from zeta.nn import MultiQueryAttention
-from zeta.nn.attention.cross_attention import CrossAttention
 from zeta.structs import ViTransformerWrapper, Encoder
-
+from zeta import Attention
+from brave_torch.cross_attn_new import CrossAttention
 
 class SwarmOfViTs(nn.Module):
     """
     A module that represents a swarm of Vision Transformers (ViTs).
 
     Args:
         image_size (int): The size of the input image.
@@ -25,182 +24,240 @@
         encoder_depth (int): The depth of the ViT encoder.
         encoder_heads (int): The number of attention heads in the ViT encoder.
         num_of_vits (int): The number of ViTs in the swarm.
         vits (nn.ModuleList): A list of ViTransformerWrapper instances.
         norm (nn.LayerNorm): A layer normalization module.
         proj (nn.Linear): A linear projection module.
     """
-    
+
     def __init__(
         self,
         image_size: int = 256,
         patch_size: int = 32,
         encoder_dim: int = 512,
         encoder_depth: int = 6,
-        encoder_heads: int = 8, 
+        encoder_heads: int = 8,
         num_of_vits: int = 4,
     ):
         super().__init__()
         self.image_size = image_size
         self.patch_size = patch_size
         self.encoder_dim = encoder_dim
         self.encoder_depth = encoder_depth
         self.encoder_heads = encoder_heads
         self.num_of_vits = num_of_vits
-        
+
         # Create a list of ViTransformerWrapper instances
         self.vits = nn.ModuleList(
             [
                 ViTransformerWrapper(
                     image_size=image_size,
                     patch_size=patch_size,
                     attn_layers=Encoder(
                         dim=encoder_dim,
                         depth=encoder_depth,
                         heads=encoder_heads,
-                    )
+                    ),
                 )
                 for _ in range(num_of_vits)
             ]
         )
-        
-        
+
         # Norm
         self.norm = nn.LayerNorm(encoder_dim)
-        
+
         # Projection
         self.proj = nn.Linear(encoder_dim, encoder_dim)
-
+        
     def forward(self, x: Tensor) -> Tensor:
         """
         Forward pass of the SwarmOfViTs module.
 
         Args:
             x (Tensor): The input tensor of shape (batch_size, channels, height, width).
 
         Returns:
-            Tensor: The concatenated vision embeddings of shape (batch_size, num_of_vits * encoder_dim).
+            Tensor: The concatenated vision embeddings of shape (batch_size, num_of_vits * encoder_dim, s).
 
         """
         # IMG Shape
         b, c, h, w = x.shape
-        
-        # Norm and projection
-        # x = self.norm(x)
-        
+
         # Vision Embedding list
         vision_embeddings = []
-        
+
         for vit in self.vits:
             out = vit(x, return_embeddings=True)
-            b, s, d = out.shape
-            normed = nn.LayerNorm(d)(out)
-            projected = nn.Linear(d, d)(normed)
+            normed = self.norm(out)
+            projected = self.proj(normed)
             vision_embeddings.append(projected)
-        
-        # Concat all of the tensors along S d
-        vision_embeddings = torch.cat((vision_embeddings), dim=1)
-            
-        return vision_embeddings
-            
-            
-# IMG Tensor
-x = torch.randn(1, 3, 224, 224) 
-
-# Model
-model = SwarmOfViTs(
-    image_size=224,
-    patch_size=32,
-    encoder_dim=512,
-    encoder_depth=6,
-    encoder_heads=8,
-    num_of_vits=4
-)
-
-# Forward
-out = model(x)
-print(out)
 
+        # Concat all of the tensors along S dimension
+        # vision_embeddings = torch.concat(vision_embeddings, dim=1)
+        # vision_embeddings.unsqueeze(1)
+        vision_embeddings = torch.stack(vision_embeddings, dim=1)
+
+        return vision_embeddings
 
 
 class MeQFormer(nn.Module):
     def __init__(
         self,
         dim: int,
         mult: int,
         depth: int = 1,
         dropout: float = 0.1,
         heads: int = 8,
     ):
         """
         Multi-Query Transformer module that combines MultiQueryAttention, CrossAttention, and FeedForward layers.
-        
+
         Args:
             dim (int): Dimension of the input and output tensors.
             mult (int): Multiplier for the dimension of the intermediate hidden layer in the FeedForward layer.
             depth (int, optional): Number of layers in the Multi-Query Transformer. Defaults to 1.
             dropout (float, optional): Dropout rate. Defaults to 0.1.
             heads (int, optional): Number of attention heads. Defaults to 8.
         """
         super().__init__()
         self.dim = dim
         self.mult = mult
         self.depth = depth
         self.dropout = dropout
-        
-        # Initialize Attn
-        self.attn = MultiQueryAttention(
+
+        # Attention
+        self.self_attn = Attention(
             dim,
             heads,
+            causal=True,
+            dropout=dropout,
+            qk_norm=True,
+            kv_heads=4,
         )
-        
+
         # FeedForward
         self.ffn = FeedForward(
             dim,
             dim,
             mult,
             swish=True,
             post_act_ln=True,
-            dropout=dropout
-        )
-        
-        # CrossAttention
-        self.cross_attn = CrossAttention(
-            dim,
             dropout=dropout,
-            heads=heads,
         )
-        
+
+
         # Learnable queries
         self.queries = nn.Parameter(torch.randn(1, heads, dim))
-        
+
         # Learnable keys
         self.keys = nn.Parameter(torch.randn(1, heads, dim))
-        
+
     def forward(self, x: Tensor, img: Tensor) -> Tensor:
         """
         Forward pass of the Multi-Query Transformer.
-        
+
         Args:
             x (Tensor): Input tensor.
             img (Tensor): Image tensor.
-        
+
         Returns:
             Tensor: Concatenated output tensor from the FeedForward and MultiQueryAttention layers.
         """
         # Attn
-        attn_out = self.attn(x, self.queries, x)
+        # attn_out = self.attn(x, self.queries, x)
+        attn_out, _ = self.self_attn(x, self.queries)
         print(attn_out.shape)
-        
+
         # Cross Attention on the output of the MultiQueryAttention
-        cross_attn_out = self.cross_attn(attn_out,  img)
-        
+        cross_attn_out, _ = self.self_attn(attn_out, img)
+        print(cross_attn_out.shape)
+
         # Feedforward
         feeded = self.ffn(cross_attn_out)
-        
+        print(feeded.shape)
+
         # Feeded
-        texted_ffn = self.ffn(x)
-        
+        # texted_ffn = self.ffn(x)
+
         # Concatenate
-        return torch.cat((feeded, texted_ffn), dim=1)
-    
-    
+        # return torch.cat((feeded, texted_ffn), dim=1)
+        return feeded
+
+
+class BraveMultiModalFusion(nn.Module):
+    """
+    A module for performing multi-modal fusion using Brave ViT Swarm and MEQ Former.
+
+    Args:
+        dim (int): The dimension of the input.
+        mult (int): The multiplier for the dimension of the input.
+        depth (int, optional): The depth of the MEQ Former. Defaults to 1.
+        dropout (float, optional): The dropout rate. Defaults to 0.1.
+        heads (int, optional): The number of attention heads. Defaults to 8.
+        image_size (int, optional): The size of the input image. Defaults to 256.
+        patch_size (int, optional): The size of each patch in the image. Defaults to 32.
+        encoder_dim (int, optional): The dimension of the encoder in the Brave ViT Swarm. Defaults to 512.
+        encoder_depth (int, optional): The depth of the encoder in the Brave ViT Swarm. Defaults to 6.
+        encoder_heads (int, optional): The number of attention heads in the encoder of the Brave ViT Swarm. Defaults to 8.
+        num_of_vits (int, optional): The number of ViTs in the Brave ViT Swarm. Defaults to 4.
+    """
+
+    def __init__(
+        self,
+        dim: int,
+        mult: int,
+        depth: int = 1,
+        dropout: float = 0.1,
+        heads: int = 8,
+        image_size: int = 256,
+        patch_size: int = 32,
+        encoder_dim: int = 512,
+        encoder_depth: int = 6,
+        encoder_heads: int = 8,
+        num_of_vits: int = 4,
+    ):
+        super().__init__()
+        self.dim = dim
+        self.mult = mult
+        self.depth = depth
+        self.dropout = dropout
+        self.heads = heads
+        self.image_size = image_size
+        self.patch_size = patch_size
+        self.encoder_dim = encoder_dim
+        self.encoder_depth = encoder_depth
+        self.encoder_heads = encoder_heads
+        self.num_of_vits = num_of_vits
+
+        # Vision
+        self.vision = SwarmOfViTs(
+            image_size=image_size,
+            patch_size=patch_size,
+            encoder_dim=encoder_dim,
+            encoder_depth=encoder_depth,
+            encoder_heads=encoder_heads,
+            num_of_vits=num_of_vits,
+        )
+
+        # MEQ Former
+        self.meq = MeQFormer(
+            dim,
+            mult,
+            depth,
+            dropout,
+            heads,
+        )
+
+    def forward(self, x: Tensor, img: Tensor) -> Tensor:
+        # Vision -- apply the swarms of vision transformers
+        vision_out = self.vision(img)[0]
+        print(f"Vision out shape: {vision_out.shape}")
+
+        # Text -- apply the MEQ Former
+        text_out = self.meq(x, vision_out)
+        t_b, t_s, t_d = text_out.shape
+
+        text_out = nn.Linear(t_d, self.dim)(text_out)
+
+        return text_out
+
+
```

### Comparing `brave_torch-4.7.8/pyproject.toml` & `brave_torch-4.7.9/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "brave-torch"
-version = "4.7.8"
+version = "4.7.9"
 description = "Swarms - Pytorch"
 license = "MIT"
 authors = ["Kye Gomez <kye@apac.ai>"]
 homepage = "https://github.com/kyegomez/BRAVE-ViT-Swarm"
 documentation = "https://swarms.apac.ai"  
 readme = "README.md" 
 repository = "https://github.com/kyegomez/BRAVE-ViT-Swarm"
@@ -24,14 +24,15 @@
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 torch = ">=2.1.1,<3.0"
 zetascale = "*"
 einops = "*"
+einops_exts = "*"
 
 [tool.poetry.dev-dependencies]
 black = "23.3.0"
 
 [tool.poetry.group.lint.dependencies]
 ruff = ">=0.0.249,<0.3.5"
 types-toml = "^0.10.8.1"
```

### Comparing `brave_torch-4.7.8/setup.py` & `brave_torch-4.7.9/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 packages = \
 ['brave_torch']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['einops', 'torch>=2.1.1,<3.0', 'zetascale']
+['einops', 'einops_exts', 'torch>=2.1.1,<3.0', 'zetascale']
 
 setup_kwargs = {
     'name': 'brave-torch',
-    'version': '4.7.8',
+    'version': '4.7.9',
     'description': 'Swarms - Pytorch',
-    'long_description': '[![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)\n\n# BRAVE or Swarms of Vision Transformers\nImplementation of the paper: "BRAVE : Broadening the visual encoding of vision-language models". BRAVE achieves state-of-the-art performance on a broad range of captioning and VQA benchmarks and significantly reduces the aforementioned issues of VLMs, while requiring a smaller number of trainable parameters than existing methods and having a more compressed representation\n\n## install\n`pip3 install brave-torch`\n\n\n## usage\n```python\nimport torch\nfrom brave_torch.main import SwarmOfViTs\n\n# IMG Tensor\nx = torch.randn(1, 3, 224, 224) \n\n# Model\nmodel = SwarmOfViTs(\n    image_size=224,\n    patch_size=32,\n    encoder_dim=512,\n    encoder_depth=6,\n    encoder_heads=8,\n    num_of_vits=4\n)\n\n# Forward\nout = model(x)\nprint(out)\n```\n\n# Citations\n\n',
+    'long_description': '[![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)\n\n# BRAVE or Swarms of Vision Transformers\nImplementation of the paper: "BRAVE : Broadening the visual encoding of vision-language models". BRAVE achieves state-of-the-art performance on a broad range of captioning and VQA benchmarks and significantly reduces the aforementioned issues of VLMs, while requiring a smaller number of trainable parameters than existing methods and having a more compressed representation.\n\n## install\n`pip3 install brave-torch`\n\n\n## usage\n\n### \n```python\nimport torch\nfrom brave_torch.main import SwarmOfViTs\n\n# IMG Tensor\nx = torch.randn(1, 3, 224, 224) \n\n# Model\nmodel = SwarmOfViTs(\n    image_size=224,\n    patch_size=32,\n    encoder_dim=512,\n    encoder_depth=6,\n    encoder_heads=8,\n    num_of_vits=4\n)\n\n# Forward\nout = model(x)\nprint(out)\n```\n\n# Citations\n\n## Todo\n- [ ] Citation link\n- [ ] Citation Bibtex\n- [ ] Diagram photo\n- [ ] Implement Andromeda Base LLM architecture\n- [ ] Provide multi-modal tokenizer\n- [ ] Train and release the model ',
     'author': 'Kye Gomez',
     'author_email': 'kye@apac.ai',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/kyegomez/BRAVE-ViT-Swarm',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `brave_torch-4.7.8/PKG-INFO` & `brave_torch-4.7.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: brave-torch
-Version: 4.7.8
+Version: 4.7.9
 Summary: Swarms - Pytorch
 Home-page: https://github.com/kyegomez/BRAVE-ViT-Swarm
 License: MIT
 Keywords: artificial intelligence,deep learning,optimizers,Prompt Engineering,swarms,agents
 Author: Kye Gomez
 Author-email: kye@apac.ai
 Requires-Python: >=3.9,<4.0
@@ -14,30 +14,33 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Requires-Dist: einops
+Requires-Dist: einops_exts
 Requires-Dist: torch (>=2.1.1,<3.0)
 Requires-Dist: zetascale
 Project-URL: Documentation, https://swarms.apac.ai
 Project-URL: Repository, https://github.com/kyegomez/BRAVE-ViT-Swarm
 Description-Content-Type: text/markdown
 
 [![Multi-Modality](agorabanner.png)](https://discord.gg/qUtxnK2NMf)
 
 # BRAVE or Swarms of Vision Transformers
-Implementation of the paper: "BRAVE : Broadening the visual encoding of vision-language models". BRAVE achieves state-of-the-art performance on a broad range of captioning and VQA benchmarks and significantly reduces the aforementioned issues of VLMs, while requiring a smaller number of trainable parameters than existing methods and having a more compressed representation
+Implementation of the paper: "BRAVE : Broadening the visual encoding of vision-language models". BRAVE achieves state-of-the-art performance on a broad range of captioning and VQA benchmarks and significantly reduces the aforementioned issues of VLMs, while requiring a smaller number of trainable parameters than existing methods and having a more compressed representation.
 
 ## install
 `pip3 install brave-torch`
 
 
 ## usage
+
+### 
 ```python
 import torch
 from brave_torch.main import SwarmOfViTs
 
 # IMG Tensor
 x = torch.randn(1, 3, 224, 224) 
 
@@ -54,8 +57,14 @@
 # Forward
 out = model(x)
 print(out)
 ```
 
 # Citations
 
-
+## Todo
+- [ ] Citation link
+- [ ] Citation Bibtex
+- [ ] Diagram photo
+- [ ] Implement Andromeda Base LLM architecture
+- [ ] Provide multi-modal tokenizer
+- [ ] Train and release the model
```

