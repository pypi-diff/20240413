# Comparing `tmp/paperplotlib-0.0.2.tar.gz` & `tmp/paperplotlib-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paperplotlib-0.0.2.tar", max compression
+gzip compressed data, was "paperplotlib-0.0.3.tar", max compression
```

## Comparing `paperplotlib-0.0.2.tar` & `paperplotlib-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2024-03-24 12:11:55.505650 paperplotlib-0.0.2/LICENSE
--rw-r--r--   0        0        0       90 2024-03-31 09:00:50.490081 paperplotlib-0.0.2/paperplotlib/__init__.py
--rw-r--r--   0        0        0     2919 2024-04-01 13:21:16.836152 paperplotlib-0.0.2/paperplotlib/bar_graph.py
--rw-r--r--   0        0        0      518 2024-04-01 13:22:28.733641 paperplotlib-0.0.2/paperplotlib/color.css
--rw-r--r--   0        0        0     2849 2024-04-01 13:19:56.767956 paperplotlib-0.0.2/paperplotlib/color.py
--rw-r--r--   0        0        0     2664 2024-04-01 13:04:44.432619 paperplotlib-0.0.2/paperplotlib/graph.py
--rw-r--r--   0        0        0      114 2024-03-26 11:56:54.539725 paperplotlib-0.0.2/paperplotlib/line_graph.py
--rw-r--r--   0        0        0      502 2024-04-01 13:57:08.467884 paperplotlib-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1425 2024-04-01 13:53:07.741280 paperplotlib-0.0.2/README.md
--rw-r--r--   0        0        0     2296 1970-01-01 00:00:00.000000 paperplotlib-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-03-24 12:11:55.505650 paperplotlib-0.0.3/LICENSE
+-rw-r--r--   0        0        0       90 2024-03-31 09:00:50.490081 paperplotlib-0.0.3/paperplotlib/__init__.py
+-rw-r--r--   0        0        0     3173 2024-04-07 07:22:50.969770 paperplotlib-0.0.3/paperplotlib/bar_graph.py
+-rw-r--r--   0        0        0     1473 2024-04-13 10:25:33.708630 paperplotlib-0.0.3/paperplotlib/color.css
+-rw-r--r--   0        0        0     2786 2024-04-13 12:54:45.036361 paperplotlib-0.0.3/paperplotlib/color.py
+-rw-r--r--   0        0        0     3042 2024-04-13 04:58:37.445484 paperplotlib-0.0.3/paperplotlib/graph.py
+-rw-r--r--   0        0        0     2422 2024-04-13 05:26:36.822103 paperplotlib-0.0.3/paperplotlib/line_graph.py
+-rw-r--r--   0        0        0      502 2024-04-13 13:50:48.603481 paperplotlib-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1517 2024-04-13 02:55:33.703225 paperplotlib-0.0.3/README.md
+-rw-r--r--   0        0        0     2388 1970-01-01 00:00:00.000000 paperplotlib-0.0.3/PKG-INFO
```

### Comparing `paperplotlib-0.0.2/LICENSE` & `paperplotlib-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paperplotlib-0.0.2/paperplotlib/bar_graph.py` & `paperplotlib-0.0.3/paperplotlib/bar_graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,76 +1,78 @@
 from typing import List, Union
 from .graph import Graph
 from .color import COLOR
 import numpy as np
 
 
 class BarGraph(Graph):
-    def __init__(self) -> None:
-        super().__init__()
+    def __init__(self, style_id: int = 1) -> None:
+        super().__init__(style_id=style_id)
 
         self._bar_width = 0.3  # 柱状图宽度 [0-1] (default 0.8)
         self._group_threshold = 0.15  # 组间距
 
     def plot(self, x_data: List[Union[str, int]], y_data: List[float]):
         """
         绘制一维柱状图
 
         ## Parameters
         x_data: x 轴数据
         y_data: y 轴数据
         """
         # x 轴坐标等距
         x_ticks = range(len(x_data))
-
-        self.ax.bar(x_ticks, y_data, width=self._bar_width, color=COLOR.get_colors(1))
-
+        self.ax.bar(x_ticks, y_data, width=self._bar_width, color=COLOR.get_colors(1, self.style_id))
         # x 轴标签和位置的映射
         self.ax.set_xticks(x_ticks, x_data)
 
     def plot_2d(
         self, data: List[List[float]], group_names: List[str], column_names: List[str], emphasize_index: int = -1
     ):
         """
         绘制二维柱状图
 
         ## Parameters
         data: 二维列表,每个元素为一组数据
         group_names: 每个组的名称
         column_names: 每一列的名称
+        emphasize_index: 高亮的列索引
         """
         assert np.shape(data) == (len(group_names), len(column_names)), "二维数据应为二维列表"
+
+        group_len = len(group_names)
+        column_len = len(column_names)
+
         if emphasize_index != -1:
             assert (
                 type(emphasize_index) == int and emphasize_index < len(column_names) and emphasize_index >= 0
             ), f"emphasize_index应在[0, {len(column_names)})之间"
 
-        group_len = len(group_names)
-        column_len = len(column_names)
-
         # 如果列数很多, 考虑到组间距, 所以重新计算一下柱状图宽度
         if column_len >= 3:
             self._bar_width = (0.5 - self._group_threshold) / column_len * 2
 
-        colors = COLOR.get_colors(column_len, emphasize_index)
+        colors = COLOR.get_colors(column_len, self.style_id, emphasize_index)
         for i in range(column_len):
             bar_pos = -column_len + 2 * i + 1
             x_ticks = [j + bar_pos / 2 * self._bar_width for j in range(group_len)]
             bar_data = [data[j][i] for j in range(group_len)]
             self._bars = self.ax.bar(
                 x_ticks, bar_data, width=self._bar_width, color=colors[i], edgecolor="black", linewidth=0.5
             )
         self.ax.set_xticks(range(group_len), group_names)
+        self.ax.tick_params(bottom=False)
 
         # https://matplotlib.org/stable/api/legend_api.html#module-matplotlib.legend
-        self.ax.legend(
+        self.legend = self.ax.legend(
             column_names,
             loc="upper center",  # 居中置顶
             ncols=column_len,  # 横向排布
             bbox_to_anchor=(0.5, 1.15),  # 置于图外侧
             handlelength=1,  # 图例长宽, 修改为正方形
             handleheight=1,  # 图例长宽, 修改为正方形
             handletextpad=0.4,  # 缩短文字和图例的间距
+            fontsize="x-small" if column_len >= 7 else "medium",  # 图例文字大小
         )
 
     def add_line(self, y: int, line_style="-"):
         self.ax.axhline(y, linestyle=line_style, linewidth=0.5, color="black")
```

### Comparing `paperplotlib-0.0.2/paperplotlib/color.py` & `paperplotlib-0.0.3/paperplotlib/color.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,58 +1,50 @@
 import re
 import os
 import numpy as np
 import matplotlib.colors as mcolors
-from typing import List, Dict, Tuple
+from typing import List, Dict
 
 
 class Color:
 
     def __init__(self) -> None:
-        self.colors: Dict[str, List[List[str]]] = {}
-        self.key_map = {
-            1: "one",
-            2: "two",
-            3: "three",
-            4: "four",
-            5: "five",
-            6: "six",
-            7: "seven",
-        }
+        self.colors: Dict[str, Dict[int, List[str]]] = {}
 
     def add(self, name: str, hex_groups: List[List[str]]):
-        self.colors[name[1:]] = hex_groups
+        self.colors[name] = {}
+        for hex_group in hex_groups:
+            self.colors[name][len(hex_group)] = hex_group
 
-    def get_colors(self, color_num: int, emphasize_index: int = -1) -> List[str]:
-        
+    def get_colors(self, color_num: int, style_id: int = 1, emphasize_index: int = -1) -> List[str]:
         if emphasize_index != -1:
             return self.get_emphasize(emphasize_index, color_num)
-        
         # 对于更多颜色的情况, 采用渐变
-        if color_num > 7:
-            return generate_color_gradient(self.colors["cold"][0][0], self.colors["cold"][0][1], color_num)
-        else:
-            return self.colors[self.key_map[color_num]][0]
+        colors = self.colors[f"style-{style_id}"].get(color_num)
+        # 如果没有该数量的颜色, 采用渐变
+        if colors is None:
+            colors = generate_color_gradient(self.colors["cold"][2][0], self.colors["cold"][2][1], color_num)
+        return colors
 
     def get_emphasize(self, index, color_num: int) -> List[str]:
-        emphasized_color = self.colors["warm"][0][0]
-        colors = generate_color_gradient(self.colors["cold"][0][0], self.colors["cold"][0][1], color_num)
+        emphasized_color = "#ffc000"
+        colors = generate_color_gradient(self.colors["cold"][2][0], self.colors["cold"][2][1], color_num)
         colors.insert(index, emphasized_color)
         return colors
 
 
 def parse_colors() -> Color:
     """
     从 color.css 中解析颜色
     """
     with open(os.path.join(os.path.dirname(__file__), "color.css")) as f:
         content = f.read()
 
     plot_color = Color()
-    css_classes = re.finditer(r"(.*?) \{(.*?)\}", content, re.DOTALL)
+    css_classes = re.finditer(r"\.(.*?) \{(.*?)\}", content, re.DOTALL)
     for css_class in css_classes:
         color_name = css_class.group(1).strip()
         color_values = css_class.group(2).split("\n")
         hex_groups: List[List[str]] = []
         for color_value in color_values:
             if len(color_value) == 0:
                 continue
```

### Comparing `paperplotlib-0.0.2/README.md` & `paperplotlib-0.0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 # paperplotlib
 
 > 本项目还处于早期开发阶段, 欢迎反馈建议
 
 paperplotlib 是基于 matplotlib 的论文实验数据绘图库, 意在快速绘制论文实验结果部分中常见的柱状图/折线图
 
-本库提供了一组 **论文实验数据图的默认样式**, 以及一组相对简洁的 API 调用
-
-一些绘制的示例代码和结果图见: [paperplotlib 示例](https://luzhixing12345.github.io/paperplotlib/articles/md-docs/使用示例/)
+本库提供了一组 **论文实验数据图的默认样式**, 以及一组相对**简洁的 API 调用**
 
 ## 安装
 
 ```bash
 pip install paperplotlib
 ```
 
@@ -21,27 +19,34 @@
 import numpy as np
 
 # 随机生成一个 5 x 7 的数据
 a = 5
 b = 7
 y = np.random.randint(10, 100, size=(a, b))
 
+# 初始化一个对象
+graph = ppl.BarGraph()
+
+# 传入数据/组/列的文字信息
 group_names = [f"group {i}" for i in range(a)]
 column_names = [f"column {i}" for i in range(b)]
-
-graph = ppl.BarGraph()
 graph.plot_2d(y, group_names, column_names)
+
+# 调整x/y轴文字
 graph.x_label = "The number of data"
 graph.y_label = "Throughput (Mbps)"
+
+# 保存图片
 graph.save()
 ```
 
 ![](./images/paperplotlib/result.png)
 
-使用文档: [paperplotlib document](https://luzhixing12345.github.io/paperplotlib/)
+更多使用说明请参考: [paperplotlib 使用文档](https://luzhixing12345.github.io/paperplotlib/)
 
 ## 参考
 
 - [matplotlib](https://matplotlib.org/stable/users/index.html)
 - [matplotlib.pyplot的使用总结大全](https://www.zhihu.com/tardis/zm/art/139052035?source_id=1003)
 - [matplotlib.pyplot常用函数讲解大全(一)](https://zhuanlan.zhihu.com/p/139475633)
 - [matplotlib.pyplot常用函数讲解大全(二)](https://zhuanlan.zhihu.com/p/139946399)
+- [Presentation练习_科研论文中插图的配色原理与方案](https://www.bilibili.com/video/BV1cJ4m1j7No/)
```

### Comparing `paperplotlib-0.0.2/PKG-INFO` & `paperplotlib-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paperplotlib
-Version: 0.0.2
+Version: 0.0.3
 Summary: 论文实验数据绘图
 Home-page: https://github.com/luzhixing12345/paperplotlib
 License: MIT
 Author: luzhixing12345
 Author-email: luzhixing12345@163.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -22,17 +22,15 @@
 
 # paperplotlib
 
 > 本项目还处于早期开发阶段, 欢迎反馈建议
 
 paperplotlib 是基于 matplotlib 的论文实验数据绘图库, 意在快速绘制论文实验结果部分中常见的柱状图/折线图
 
-本库提供了一组 **论文实验数据图的默认样式**, 以及一组相对简洁的 API 调用
-
-一些绘制的示例代码和结果图见: [paperplotlib 示例](https://luzhixing12345.github.io/paperplotlib/articles/md-docs/使用示例/)
+本库提供了一组 **论文实验数据图的默认样式**, 以及一组相对**简洁的 API 调用**
 
 ## 安装
 
 ```bash
 pip install paperplotlib
 ```
 
@@ -43,28 +41,34 @@
 import numpy as np
 
 # 随机生成一个 5 x 7 的数据
 a = 5
 b = 7
 y = np.random.randint(10, 100, size=(a, b))
 
+# 初始化一个对象
+graph = ppl.BarGraph()
+
+# 传入数据/组/列的文字信息
 group_names = [f"group {i}" for i in range(a)]
 column_names = [f"column {i}" for i in range(b)]
-
-graph = ppl.BarGraph()
 graph.plot_2d(y, group_names, column_names)
+
+# 调整x/y轴文字
 graph.x_label = "The number of data"
 graph.y_label = "Throughput (Mbps)"
+
+# 保存图片
 graph.save()
 ```
 
 ![](./images/paperplotlib/result.png)
 
-使用文档: [paperplotlib document](https://luzhixing12345.github.io/paperplotlib/)
+更多使用说明请参考: [paperplotlib 使用文档](https://luzhixing12345.github.io/paperplotlib/)
 
 ## 参考
 
 - [matplotlib](https://matplotlib.org/stable/users/index.html)
 - [matplotlib.pyplot的使用总结大全](https://www.zhihu.com/tardis/zm/art/139052035?source_id=1003)
 - [matplotlib.pyplot常用函数讲解大全(一)](https://zhuanlan.zhihu.com/p/139475633)
 - [matplotlib.pyplot常用函数讲解大全(二)](https://zhuanlan.zhihu.com/p/139946399)
-
+- [Presentation练习_科研论文中插图的配色原理与方案](https://www.bilibili.com/video/BV1cJ4m1j7No/)
```

