# Comparing `tmp/haedream-0.0.8.tar.gz` & `tmp/haedream-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "haedream-0.0.8.tar", last modified: Mon Apr  1 01:53:34 2024, max compression
+gzip compressed data, was "haedream-0.0.9.tar", last modified: Sat Apr 13 06:00:36 2024, max compression
```

## Comparing `haedream-0.0.8.tar` & `haedream-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-01 01:53:34.014150 haedream-0.0.8/
--rw-rw-rw-   0        0        0      446 2024-04-01 01:53:34.014150 haedream-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       45 2024-03-27 00:42:43.000000 haedream-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-01 01:53:34.002210 haedream-0.0.8/haedream/
--rw-rw-rw-   0        0        0       62 2024-03-27 00:41:56.000000 haedream-0.0.8/haedream/__init__.py
--rw-rw-rw-   0        0        0       19 2024-04-01 01:53:15.000000 haedream-0.0.8/haedream/__version__.py
--rw-rw-rw-   0        0        0     1345 2024-04-01 01:52:51.000000 haedream-0.0.8/haedream/saveLog.py
-drwxrwxrwx   0        0        0        0 2024-04-01 01:53:34.013152 haedream-0.0.8/haedream.egg-info/
--rw-rw-rw-   0        0        0      446 2024-04-01 01:53:33.000000 haedream-0.0.8/haedream.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-04-01 01:53:33.000000 haedream-0.0.8/haedream.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-01 01:53:33.000000 haedream-0.0.8/haedream.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-01 01:53:33.000000 haedream-0.0.8/haedream.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-04-01 01:53:34.016145 haedream-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      649 2024-04-01 01:53:24.000000 haedream-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:00:36.891010 haedream-0.0.9/
+-rw-rw-rw-   0        0        0     1152 2024-04-13 06:00:36.891010 haedream-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      734 2024-04-13 05:51:03.000000 haedream-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-13 06:00:36.855106 haedream-0.0.9/haedream/
+-rw-rw-rw-   0        0        0       62 2024-03-27 00:41:56.000000 haedream-0.0.9/haedream/__init__.py
+-rw-rw-rw-   0        0        0       19 2024-04-13 05:38:35.000000 haedream-0.0.9/haedream/__version__.py
+-rw-rw-rw-   0        0        0     2063 2024-04-13 05:51:12.000000 haedream-0.0.9/haedream/saveLog.py
+drwxrwxrwx   0        0        0        0 2024-04-13 06:00:36.890013 haedream-0.0.9/haedream.egg-info/
+-rw-rw-rw-   0        0        0     1152 2024-04-13 06:00:36.000000 haedream-0.0.9/haedream.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-04-13 06:00:36.000000 haedream-0.0.9/haedream.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 06:00:36.000000 haedream-0.0.9/haedream.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-13 06:00:36.000000 haedream-0.0.9/haedream.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-04-13 06:00:36.893021 haedream-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      683 2024-04-13 06:00:32.000000 haedream-0.0.9/setup.py
```

### Comparing `haedream-0.0.8/haedream/saveLog.py` & `haedream-0.0.9/haedream/saveLog.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,38 +2,39 @@
 import json
 
 class ModelRunner:
 
     server_url = "http://localhost:8088/save_data"
 
     def run_model(self, modelName, projectName, inputData, apiKey, outputData):
-        
-        # 결과를 JSON 형식으로 변환
+        warning_message = "주의 : projectName, apiKey를 잘못 입력하면 저장되지 않습니다."
+        print("\033[1m" + warning_message + "\033[0m")  # 강조하여 출력
+
         json_output = self._format_output(modelName, projectName, inputData, outputData, apiKey)
        
-        # 결과를 서버로 전송하여 저장
         self._save_to_server(json_output)
         
-        # 결과 반환
         return json_output
 
     def _format_output(self, modelName, projectName, inputData, outputData, apiKey):
-        # 결과를 JSON 형식으로 포맷팅합니다.
         result = {
             "modelName": modelName,
             "projectName": projectName,
             "inputData": inputData,
             "outputData": outputData,
             "apiKey": apiKey
         }
         return json.dumps(result)
 
     def _save_to_server(self, data):
-        # 서버로 데이터를 전송하여 저장합니다.
         
         data2 = {"js" : data}
         with requests.post(self.server_url, data=data2, stream=True) as response:
             if response.ok:
                 print("Data successfully saved to server.")
             else:
                 print("Failed to save data to server.")
                 print(response.status_code)
+
+
+def help():
+    print("이 패키지는 해드림의 LLM output 평가를 위해 해드림 서버로 데이터를 전송할 수 있는 모듈 패키지입니다. \n사용을 위해서는 해드림 회원가입과 프로젝트 생성이 필요합니다.\n\n1. 먼저 평가할 모델의 질의를 inputData로 정의하고 결과를 outputData로 정의합니다.\n2. 회원가입 후 발급받은 apiKey를 apiKey로 정의하고 생성한 프로젝트 이름을 projectName으로 정의합니다.\n3. 모델의 이름은 modelName으로 정의합니다.\n4. runner 객체를 생성하고 run_model 함수에 각 매개변수를 채워넣고 실행합니다.\n\n  ❗ 이때 잘못된 projectName, apiKey를 입력하면 데이터가 저장되지 않으니 주의 바랍니다.")
```

### Comparing `haedream-0.0.8/setup.py` & `haedream-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 
 import setuptools
 
-with open("README.md", "r") as fh:
+with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="haedream",
-    version="0.0.8",
+    version="0.0.9",
     author="GOSEGU",
-    author_email="",
+    author_email="jhj990203@gmail.com",
     description="This is a package for haedream",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/Gosegu2024/Haedream.git", ##
+    url="https://github.com/Gosegu2024/Haedream.git",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

