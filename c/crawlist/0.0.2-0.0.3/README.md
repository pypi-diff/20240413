# Comparing `tmp/crawlist-0.0.2.tar.gz` & `tmp/crawlist-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crawlist-0.0.2.tar", last modified: Fri Apr 12 09:23:31 2024, max compression
+gzip compressed data, was "crawlist-0.0.3.tar", last modified: Sat Apr 13 05:41:06 2024, max compression
```

## Comparing `crawlist-0.0.2.tar` & `crawlist-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:23:31.658490 crawlist-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-12 09:23:24.000000 crawlist-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-12 09:23:24.000000 crawlist-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-12 09:23:31.658490 crawlist-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-04-12 09:23:24.000000 crawlist-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:23:31.658490 crawlist-0.0.2/crawlist/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:23:31.658490 crawlist-0.0.2/crawlist/analyzers/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3387 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    10660 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/dynamic_pager.py
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/pager.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2869 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/static_pager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/analyzers/valid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:23:31.658490 crawlist-0.0.2/crawlist/processings/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/processings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-04-12 09:23:24.000000 crawlist-0.0.2/crawlist/processings/action.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 09:23:31.658490 crawlist-0.0.2/crawlist.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6839 2024-04-12 09:23:31.000000 crawlist-0.0.2/crawlist.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-12 09:23:31.000000 crawlist-0.0.2/crawlist.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 09:23:31.000000 crawlist-0.0.2/crawlist.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 09:23:31.000000 crawlist-0.0.2/crawlist.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-12 09:23:31.000000 crawlist-0.0.2/crawlist.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 09:23:31.658490 crawlist-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-12 09:23:24.000000 crawlist-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:41:06.954359 crawlist-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-13 05:41:02.000000 crawlist-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-13 05:41:02.000000 crawlist-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-13 05:41:06.954359 crawlist-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-13 05:41:02.000000 crawlist-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:41:06.954359 crawlist-0.0.3/crawlist/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-13 05:41:02.000000 crawlist-0.0.3/crawlist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-13 05:41:02.000000 crawlist-0.0.3/crawlist/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:41:06.954359 crawlist-0.0.3/crawlist/analyzers/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-13 05:41:02.000000 crawlist-0.0.3/crawlist/analyzers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3839 2024-04-13 05:41:02.000000 crawlist-0.0.3/crawlist/analyzers/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11099 2024-04-13 05:41:02.000000 crawlist-0.0.3/crawlist/analyzers/dynamic_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-13 05:41:02.000000 crawlist-0.0.3/crawlist/analyzers/pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      785 2024-04-13 05:41:02.000000 crawlist-0.0.3/crawlist/analyzers/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-04-13 05:41:02.000000 crawlist-0.0.3/crawlist/analyzers/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2024-04-13 05:41:02.000000 crawlist-0.0.3/crawlist/analyzers/static_pager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-13 05:41:02.000000 crawlist-0.0.3/crawlist/analyzers/valid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:41:06.954359 crawlist-0.0.3/crawlist/processings/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-13 05:41:02.000000 crawlist-0.0.3/crawlist/processings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3944 2024-04-13 05:41:02.000000 crawlist-0.0.3/crawlist/processings/action.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 05:41:06.954359 crawlist-0.0.3/crawlist.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-13 05:41:06.000000 crawlist-0.0.3/crawlist.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-13 05:41:06.000000 crawlist-0.0.3/crawlist.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 05:41:06.000000 crawlist-0.0.3/crawlist.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-13 05:41:06.000000 crawlist-0.0.3/crawlist.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 05:41:06.000000 crawlist-0.0.3/crawlist.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 05:41:06.954359 crawlist-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-13 05:41:02.000000 crawlist-0.0.3/setup.py
```

### Comparing `crawlist-0.0.2/LICENSE` & `crawlist-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.2/crawlist/analyzers/dynamic_pager.py` & `crawlist-0.0.3/crawlist/analyzers/dynamic_pager.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from selenium import webdriver as wd
 from selenium.webdriver.chrome.service import Service
 
 
 class DynamicPager(Pager):
     def __init__(self, webdriver: WebDriver = None, interval: float = 0.1) -> None:
         """
-        :param webdriver: selenium的WebDriver对象
-        :param interval: 抓取list频率，可使用self.sleep()方法控制频率
+        :param webdriver: WebDriver object for selenium
+        :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         if not webdriver:
             option = wd.ChromeOptions()
             option.add_argument("start-maximized")
             option.add_argument("--headless")
             option.add_argument("window-size=1920x3000")
             agent = 'user-agent="Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36"'
@@ -26,16 +26,16 @@
             self.webdriver = wd.Chrome(service=Service(ChromeDriverManager().install()), options=option)
         else:
             self.webdriver = webdriver
         super().__init__(interval=interval)
 
     def click_safety(self, button: WebElement) -> None:
         """
-        尝试多次点击按钮
-        :param button: 按钮元素
+        Attempt to click the button multiple times
+        :param button: Button elements
         """
         # 点击失败后多次尝试点击
         for _ in range(3):
             try:
                 button.click()
                 self.sleep()
                 break
@@ -52,21 +52,21 @@
             pass
 
 
 class DynamicRedirectPager(DynamicPager):
     def __init__(self, uri: str, uri_split: str, webdriver: WebDriver = None, start: int = 1, offset: int = 1,
                  interval: float = 0.1) -> None:
         """
-        基于动态网页分析器(重定向翻页)
-        :param uri: 第一页链接
-        :param uri_split: 链接分页(使用%v代理) example:https://www.boc.cn/sourcedb/whpj/index_%v.html
-        :param webdriver: selenium的WebDriver对象
-        :param start: 起始页
-        :param offset: 分页间隔
-        :param interval: 抓取list频率，可使用self.sleep()方法控制频率
+        Based on dynamic web page analyzer (redirect page flipping)
+        :param uri: First page link
+        :param uri_split: Link pagination (using% v proxy) Example: https://www.boc.cn/sourcedb/whpj/index_%v.html
+        :param webdriver: WebDriver object for selenium
+        :param start: Start page
+        :param offset: pagination interval
+        :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert '%v' in uri_split
         assert Valid.is_valid_url(uri) and Valid.is_valid_url(uri_split.replace('%v', str(start)))
         assert offset >= 1 and start >= 0
         super().__init__(webdriver=webdriver, interval=interval)
         self.pre_load(webdriver)
         self.index = start
@@ -84,18 +84,18 @@
         self.webdriver.get(self.current_uri)
         return self.webdriver.page_source
 
 
 class DynamicListRedirectPager(DynamicPager):
     def __init__(self, uris: list, webdriver: WebDriver = None, interval: float = 0.1) -> None:
         """
-        基于动态网页分析器(重定向翻页)
-        :param uris: 含多个uri的list，按照顺序往下执行
-        :param webdriver: selenium的WebDriver对象
-        :param interval: 抓取list频率，可使用self.sleep()方法控制频率
+        Based on dynamic web page analyzer (redirect page flipping)
+        :param uris: A list containing multiple uris, executed in order downwards
+        :param webdriver: WebDriver object for selenium
+        :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert isinstance(uris, list)
         for uri in uris:
             assert Valid.is_valid_url(uri)
         assert len(uris) > 0
         super().__init__(webdriver=webdriver, interval=interval)
         self.pre_load(webdriver)
@@ -116,18 +116,18 @@
         self.webdriver.get(uri)
         return self.webdriver.page_source
 
 
 class DynamicScrollPager(DynamicPager):
     def __init__(self, uri: str, webdriver: WebDriver = None, interval: float = 1) -> None:
         """
-        基于动态网页分析器(滚动翻页)
-        :param uri: 网页链接，该网页是滚动翻页
-        :param webdriver: selenium的WebDriver对象
-        :param interval: 抓取list频率，可使用self.sleep()方法控制频率
+        Based on dynamic web page analyzer (scrolling and flipping)
+        :param uri: webpage link, which is a scrolling page
+        :param webdriver: WebDriver object for selenium
+        :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert Valid.is_valid_url(uri)
         super().__init__(webdriver=webdriver, interval=interval)
         if not self.pre_load(self.webdriver):
             self.webdriver.get(uri)
         self.uri = uri
 
@@ -148,19 +148,19 @@
         return self.webdriver.page_source
 
 
 class DynamicLineButtonPager(DynamicPager):
     def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: WebDriver = None,
                  interval: float = 1) -> None:
         """
-        基于动态网页分析器(行按钮翻页)
-        :param uri: 网页链接，该网页是行按钮翻页
-        :param button_selector: 行按钮选择器
-        :param webdriver: selenium的WebDriver对象
-        :param interval: 抓取list频率，可使用self.sleep()方法控制频率
+        Based on dynamic web page analyzer (row button page flipping)
+        :param uri: webpage link, which is a row button for flipping pages
+        :param button.selector: row button selector
+        :param webdriver: WebDriver object for selenium
+        :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert Valid.is_valid_url(uri)
         super().__init__(webdriver=webdriver, interval=interval)
         if not self.pre_load(self.webdriver):
             self.webdriver.get(uri)
         assert len(button_selector(self.webdriver, interval=interval)) > 0
         self.uri = uri
@@ -176,21 +176,21 @@
         return self.webdriver.page_source
 
 
 class DynamicNumButtonPager(DynamicPager):
     def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: WebDriver = None, start: int = 1,
                  offset: int = 1, interval: float = 1) -> None:
         """
-        基于动态网页分析器(数字按钮翻页)
-        :param uri: 网页链接，该网页是数字按钮翻页
-        :param button_selector: 数字按钮选择器
-        :param webdriver: selenium的WebDriver对象
-        :param start: 起始页
-        :param offset: 分页间隔
-        :param interval: 抓取list频率，可使用self.sleep()方法控制频率
+        Based on dynamic web page analyzer (digital button flipping)
+        :param uri: webpage link, which is a numeric button for flipping pages
+        :param button.selector: numeric button selector
+        :param webdriver: WebDriver object for selenium
+        :param start: Start page
+        :param offset: pagination interval
+        :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert Valid.is_valid_url(uri)
         super().__init__(webdriver=webdriver, interval=interval)
         if not self.pre_load(self.webdriver):
             self.webdriver.get(uri)
         assert len(button_selector(self.webdriver, interval=interval)) > 0
         self.uri = uri
@@ -251,21 +251,21 @@
         return None
 
 
 class DynamicNextButtonPager(DynamicPager):
     def __init__(self, uri: str, button_selector: WebElementSelector, webdriver: WebDriver = None, start: int = 1,
                  offset: int = 1, interval: float = 1) -> None:
         """
-        基于动态网页分析器(点击下一页按钮翻页)
-        :param uri: 网页链接，该网页是点击下一页按钮翻页
-        :param button_selector: 点击下一页按钮选择器
-        :param webdriver: selenium的WebDriver对象
-        :param start: 起始页
-        :param offset: 分页间隔
-        :param interval: 抓取list频率，可使用self.sleep()方法控制频率
+        Based on dynamic web page analyzer (click the next page button to page)
+        :param uri: Web page link, which is a page that can be flipped by clicking the next page button
+        :param button.selector: Click on the next page button selector
+        :param webdriver: WebDriver object for selenium
+        :param start: Start page
+        :param offset: pagination interval
+        :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert Valid.is_valid_url(uri)
         super().__init__(webdriver=webdriver, interval=interval)
         if not self.pre_load(self.webdriver):
             self.webdriver.get(uri)
         assert len(button_selector(self.webdriver, interval=interval)) > 0
         self.uri = uri
```

### Comparing `crawlist-0.0.2/crawlist/analyzers/selector.py` & `crawlist-0.0.3/crawlist/analyzers/selector.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,35 +11,35 @@
 class BaseSelector(object):
     pass
 
 
 class Selector(BaseSelector):
     def __init__(self, pattern: str) -> None:
         """
-        选择器
-        :param pattern: 抓取规则
+        Selector
+        :param pattern: Grab rules
         """
         assert self.valid(pattern)
         self.pattern = pattern
 
     def select(self, html: str) -> list[str]:
         raise NotImplementedError
 
     def valid(self, pattern) -> bool:
-        raise NotImplementedError
+        return True
 
     def __call__(self, html: str) -> list[str]:
         return self.select(html)
 
 
 class WebElementSelector(BaseSelector):
     def __init__(self, pattern: str) -> None:
         """
-        webElement选择器(selenium)
-        :param pattern: 抓取规则
+        WebElement selector (selenium)
+        :param pattern: Grab rules
         """
         assert self.valid(pattern)
         self.pattern = pattern
 
     def select(self, webdriver: WebDriver, interval: float = 0.1) -> list[WebElement]:
         raise NotImplementedError
 
@@ -48,39 +48,39 @@
 
     def __call__(self, webdriver: WebDriver, interval: float = 0.1) -> list[WebElement]:
         return self.select(webdriver, interval)
 
 
 class CssSelector(Selector):
     """
-    css选择器
+    css selector
     """
 
     def select(self, html: str) -> list[str]:
         return parsel.Selector(text=html).css(self.pattern).getall()
 
     def valid(self, pattern) -> bool:
         return Valid.is_valid_css(pattern)
 
 
 class XpathSelector(Selector):
     """
-    xpath选择器
+    xpath selector
     """
 
     def select(self, html: str) -> list[str]:
         return parsel.Selector(text=html).xpath(self.pattern).getall()
 
     def valid(self, pattern) -> bool:
         return Valid.is_valid_xpath(pattern)
 
 
 class RegexSelector(Selector):
     """
-    正则表达式选择器
+    regex selector
     """
 
     def select(self, html: str) -> list[str]:
         return parsel.Selector(text=html).re(self.pattern)
 
     def valid(self, pattern) -> bool:
         return Valid.is_valid_regex(pattern)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `crawlist-0.0.2/crawlist/analyzers/static_pager.py` & `crawlist-0.0.3/crawlist/analyzers/static_pager.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,38 +2,35 @@
 from .valid import Valid
 from .pager import Pager
 
 
 class StaticPager(Pager):
     def __init__(self, request: Request = None, interval: float = 0.1):
         """
-        :param request: 请求对象
-        :param interval: 抓取list频率，可使用self.sleep()方法控制频率
+        :param request: Request object
+        :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         if not request:
-            self.request = Request(headers={
-                "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_14_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/70.0.3538.77 Safari/537.36",
-                'Cache-Control': 'max-age=0',
-            })
+            self.request = Request()
         else:
             self.request = request
         super().__init__(interval=interval)
 
 
 class StaticRedirectPager(StaticPager):
     def __init__(self, uri: str, uri_split: str, request: Request = None, start: int = 1, offset: int = 1,
                  interval: float = 0.1) -> None:
         """
-        基于静态网页分析器(重定向翻页)
-        :param uri: 第一页链接
-        :param uri_split: 链接分页(使用%v代替) example:https://www.boc.cn/sourcedb/whpj/index_%v.html
-        :param request: 请求对象
-        :param start: 起始页
-        :param offset: 分页间隔
-        :param interval: 抓取list频率，可使用self.sleep()方法控制频率
+        Based on static web page analyzer (redirect page flipping)
+        :param uri: First page link
+        :param uri_split: Link pagination (using %v instead) Example: https://www.boc.cn/sourcedb/whpj/index_%v.html
+        :param request: Request object
+        :param start: Start page
+        :param offset: pagination interval
+        :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert '%v' in uri_split
         assert Valid.is_valid_url(uri) and Valid.is_valid_url(uri_split.replace('%v', str(start)))
         assert offset >= 1 and start >= 0
         super().__init__(request=request, interval=interval)
         self.index = start
         self.offset = offset
@@ -49,18 +46,18 @@
     def html(self) -> str:
         return self.request(self.current_uri)
 
 
 class StaticListRedirectPager(StaticPager):
     def __init__(self, uris: list, request: Request = None, interval: float = 0.1) -> None:
         """
-        基于静态网页分析器(重定向翻页)
-        :param uris: 含多个uri的list，按照顺序往下执行
-        :param request: 请求对象
-        :param interval: 抓取list频率，可使用self.sleep()方法控制频率
+        Based on static web page analyzer (redirect page flipping)
+        :param uris: A list containing multiple uris, executed in order downwards
+        :param request: Request object
+        :param interval: Grab the list frequency and adjust it according to the actual situation of the webpage
         """
         assert isinstance(uris, list)
         for uri in uris:
             assert Valid.is_valid_url(uri)
         assert len(uris) > 0
         super().__init__(request=request, interval=interval)
         self.index = 0
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `crawlist-0.0.2/crawlist/analyzers/valid.py` & `crawlist-0.0.3/crawlist/analyzers/valid.py`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.2/crawlist/processings/action.py` & `crawlist-0.0.3/crawlist/processings/action.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,18 +9,18 @@
 
 
 class Action:
 
     @staticmethod
     def click(driver: WebDriver, xpath: str) -> bool:
         """
-        处理点击事件
+        Handling click events
         :param driver: selenium webdriver
-        :param xpath: 点击按钮的xpath路径
-        :return: 是否成功
+        :param xpath: Click on the xpath path of the button
+        :return: Whether successful
         """
         WebDriverWait(driver, 2).until(EC.presence_of_element_located((By.XPATH, xpath)))
         element = driver.find_element(By.XPATH, xpath)
         # 尝试点击两次
         try:
             element.click()
             time.sleep(random.uniform(0.1, 0.2))
@@ -30,97 +30,97 @@
             except Exception:
                 return False
         return True
 
     @staticmethod
     def inputKeyword(driver: WebDriver, xpath: str, keyword: str) -> bool:
         """
-        处理键盘输入事件
+        Handling keyboard input events
         :param driver: selenium webdriver
-        :param xpath: 输入框的xpath路径
-        :param keyword:  需要传入keyword关键词
-        :return: 是否成功
+        :param xpath: The xpath path of the input box
+        :param keyword: keyword needs to be passed in
+        :return: Whether successful
         """
         WebDriverWait(driver, 2).until(EC.presence_of_element_located((By.XPATH, xpath)))
         element = driver.find_element(By.XPATH, xpath)
         try:
             element.send_keys(keyword)
         except Exception:
             return False
         return True
 
     @staticmethod
     def sendEnter(driver: WebDriver, xpath: str) -> bool:
         """
-        按一下回车键
+        Press the enter key once
         :param driver: selenium webdriver
-        :param xpath: 输入框的xpath路径
-        :return: 是否成功
+        :param xpath: The xpath path of the input box
+        :return: Whether successful
         """
         WebDriverWait(driver, 2).until(EC.presence_of_element_located((By.XPATH, xpath)))
         element = driver.find_element(By.XPATH, xpath)
         try:
             element.send_keys(Keys.RETURN)
         except Exception:
             return False
         return True
 
     @staticmethod
     def switchLastTab(driver: WebDriver) -> bool:
         """
-        切换到最后一个句柄
+        Switch to the last handle
         :param driver: selenium webdriver
-        :return: 是否成功
+        :return: Whether successful
         """
         try:
             window_handles = driver.window_handles
             if len(window_handles) < 2:
                 return False
             driver.switch_to.window(window_handles[-1])
         except Exception as e:
             return False
         return True
 
     @staticmethod
     def switchTab(driver: WebDriver, index: int) -> bool:
         """
-        切换到第index个句柄
+        Switch to the index handle
         :param driver: selenium webdriver
-        :param index: 第index个句柄
-        :return: 是否成功
+        :param index: The index handle
+        :return: Whether successful
         """
         try:
             window_handles = driver.window_handles
             driver.switch_to.window(window_handles[index])
         except Exception as e:
             return False
         return True
 
     @staticmethod
     def searchRedirect(driver: WebDriver, url: str, keyword: str) -> bool:
         """
-        将路径中的%s替换成keyword,并重定向
+        Replace % s in the path with keyword and redirect it
         :param driver:  selenium webdriver
-        :param url: 含%s的链接
-        :param keyword: 需要传入keyword关键词
-        :return: 是否成功
+        :param url: Link containing %s
+        :param keyword: keyword needs to be passed in
+        :return: Whether successful
         """
         try:
             url = url.replace(r"%s", keyword)
             driver.get(url)
         except Exception:
             return False
         return True
 
     @staticmethod
     def redirect(driver: WebDriver, url: str) -> bool:
         """
-        将路径中的%s替换成keyword,并重定向
+        Direct redirection
         :param driver:  selenium webdriver
-        :param url: 需要重定向的链接
-        :return: 是否成功
+        :param url: Links that require redirection
+        :return: Whether successful
         """
         try:
             driver.get(url)
         except Exception:
             return False
         return True
```

### Comparing `crawlist-0.0.2/crawlist.egg-info/SOURCES.txt` & `crawlist-0.0.3/crawlist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crawlist-0.0.2/setup.py` & `crawlist-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'crawlist'
 DESCRIPTION = 'A universal solution for web crawling lists'
 URL = 'https://github.com/WwwwwyDev/crawlist'
 EMAIL = 'wwy20001014@foxmail.com'
 AUTHOR = 'WwyDev'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'parsel', 'selenium>=4.0.0', 'cssselect', 'lxml', 'requests', 'webdriver-manager'
 ]
 
 # What packages are optional?
```

