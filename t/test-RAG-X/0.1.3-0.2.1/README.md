# Comparing `tmp/test_RAG_X-0.1.3.tar.gz` & `tmp/test_RAG_X-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "test_RAG_X-0.1.3.tar", last modified: Sat Apr  6 04:58:19 2024, max compression
+gzip compressed data, was "test_RAG_X-0.2.1.tar", last modified: Sat Apr 13 10:49:29 2024, max compression
```

## Comparing `test_RAG_X-0.1.3.tar` & `test_RAG_X-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 ankitbaliyan   (501) staff       (20)        0 2024-04-06 04:58:19.569289 test_RAG_X-0.1.3/
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     1073 2024-04-02 17:20:52.000000 test_RAG_X-0.1.3/LICENSE
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     3769 2024-04-06 04:58:19.568934 test_RAG_X-0.1.3/PKG-INFO
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     2936 2024-04-06 04:46:14.000000 test_RAG_X-0.1.3/README.md
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)       38 2024-04-06 04:58:19.569370 test_RAG_X-0.1.3/setup.cfg
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     1644 2024-04-06 04:47:48.000000 test_RAG_X-0.1.3/setup.py
-drwxr-xr-x   0 ankitbaliyan   (501) staff       (20)        0 2024-04-06 04:58:19.567473 test_RAG_X-0.1.3/test_RAG_X/
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)        0 2024-04-03 14:43:42.000000 test_RAG_X-0.1.3/test_RAG_X/__init__.py
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     4885 2024-04-06 04:55:59.000000 test_RAG_X-0.1.3/test_RAG_X/chunk_it.py
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     1868 2024-04-02 15:58:56.000000 test_RAG_X-0.1.3/test_RAG_X/clean_it.py
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)      919 2024-04-02 15:58:21.000000 test_RAG_X-0.1.3/test_RAG_X/extractor.py
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     5596 2024-04-01 11:46:39.000000 test_RAG_X-0.1.3/test_RAG_X/get_evaluation_question.py
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     5617 2024-04-06 04:55:36.000000 test_RAG_X-0.1.3/test_RAG_X/prag.py
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     5440 2024-04-02 16:09:16.000000 test_RAG_X-0.1.3/test_RAG_X/trulens.py
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     3686 2024-04-06 04:56:53.000000 test_RAG_X-0.1.3/test_RAG_X/utils.py
-drwxr-xr-x   0 ankitbaliyan   (501) staff       (20)        0 2024-04-06 04:58:19.568542 test_RAG_X-0.1.3/test_RAG_X.egg-info/
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)     3769 2024-04-06 04:58:19.000000 test_RAG_X-0.1.3/test_RAG_X.egg-info/PKG-INFO
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)      387 2024-04-06 04:58:19.000000 test_RAG_X-0.1.3/test_RAG_X.egg-info/SOURCES.txt
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)        1 2024-04-06 04:58:19.000000 test_RAG_X-0.1.3/test_RAG_X.egg-info/dependency_links.txt
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)      135 2024-04-06 04:58:19.000000 test_RAG_X-0.1.3/test_RAG_X.egg-info/requires.txt
--rw-r--r--   0 ankitbaliyan   (501) staff       (20)       11 2024-04-06 04:58:19.000000 test_RAG_X-0.1.3/test_RAG_X.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-13 10:49:28.988190 test_RAG_X-0.2.1/
+-rw-rw-rw-   0        0        0     1073 2024-04-12 20:49:58.000000 test_RAG_X-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     4267 2024-04-13 10:49:28.977545 test_RAG_X-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3307 2024-04-13 10:21:16.000000 test_RAG_X-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-13 10:49:28.988190 test_RAG_X-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1081 2024-04-13 10:49:23.000000 test_RAG_X-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-13 10:49:28.792629 test_RAG_X-0.2.1/test_RAG_X/
+-rw-rw-rw-   0        0        0      358 2024-04-12 20:49:58.000000 test_RAG_X-0.2.1/test_RAG_X/__init__.py
+-rw-rw-rw-   0        0        0     1126 2024-04-13 10:11:35.000000 test_RAG_X-0.2.1/test_RAG_X/document_extractor.py
+-rw-rw-rw-   0        0        0     3111 2024-04-13 10:48:57.000000 test_RAG_X-0.2.1/test_RAG_X/evaluation_question_generator.py
+-rw-rw-rw-   0        0        0     7801 2024-04-13 10:09:50.000000 test_RAG_X-0.2.1/test_RAG_X/hub.py
+-rw-rw-rw-   0        0        0     4956 2024-04-13 09:39:56.000000 test_RAG_X-0.2.1/test_RAG_X/library_exceptions.py
+-rw-rw-rw-   0        0        0     7144 2024-04-12 20:49:58.000000 test_RAG_X-0.2.1/test_RAG_X/text_chunker.py
+-rw-rw-rw-   0        0        0     2330 2024-04-13 10:48:57.000000 test_RAG_X-0.2.1/test_RAG_X/text_cleaner.py
+-rw-rw-rw-   0        0        0     3666 2024-04-12 20:49:58.000000 test_RAG_X-0.2.1/test_RAG_X/text_utils.py
+-rw-rw-rw-   0        0        0     5144 2024-04-12 20:49:58.000000 test_RAG_X-0.2.1/test_RAG_X/tru_lens_evaluator.py
+drwxrwxrwx   0        0        0        0 2024-04-13 10:49:28.965423 test_RAG_X-0.2.1/test_RAG_X.egg-info/
+-rw-rw-rw-   0        0        0     4267 2024-04-13 10:49:27.000000 test_RAG_X-0.2.1/test_RAG_X.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      458 2024-04-13 10:49:28.000000 test_RAG_X-0.2.1/test_RAG_X.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-13 10:49:27.000000 test_RAG_X-0.2.1/test_RAG_X.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2024-04-13 10:49:27.000000 test_RAG_X-0.2.1/test_RAG_X.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-13 10:49:27.000000 test_RAG_X-0.2.1/test_RAG_X.egg-info/top_level.txt
```

### Comparing `test_RAG_X-0.1.3/LICENSE` & `test_RAG_X-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `test_RAG_X-0.1.3/PKG-INFO` & `test_RAG_X-0.2.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,20 @@
-Metadata-Version: 2.1
-Name: test_RAG_X
-Version: 0.1.3
-Summary: This library is to search the best parameters across different steps of the RAG process.
-Home-page: https://github.com/hidevscommunity/gen-ai-library/tree/main/Ankit
-Author: Ankit
-Author-email: a.baliyan008@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: langchain==0.1.13
-Requires-Dist: langchain-openai>=0.1.1
-Requires-Dist: trulens-eval==0.27.0
-Requires-Dist: chromadb==0.4.24
-Requires-Dist: sentence-transformers==2.6.1
-Requires-Dist: unstructured[pdf]==0.13.0
-
 
 ---
 
 # RAG-X Library
 
 ## Overview
 
 RAG-X is a comprehensive library designed to optimize Retrieval-Augmented Generation (RAG) processes. It provides a suite of tools to automatically determine the best parameters for processing specific documents. This includes selecting appropriate chunking techniques, embedding models, vector databases, and Language Model (LLM) configurations.
 
+## Flow Chart
+
+![Flow Chart](pictures/structure.png)
+
 ### Key Features:
 - **Adaptive Chunking:** Incorporates four advanced text chunking methodologies to enhance the handling of diverse document structures.
   - Specific Text Splitting
   - Recursive Text Splitting
   - Sentence Window Splitting
   - Semantic Window Splitting
 - **Expandability:** Future versions will introduce additional chunking strategies and enhancements based on user feedback and ongoing research.
@@ -58,57 +40,66 @@
 
 Before diving into the functionality of test-RAG-X, ensure that your environment variables are properly configured with your OpenAI API key and your Hugging Face token:
 
 ```python
 import os
 
 os.environ['OPENAI_API_KEY'] = "YOUR_OPENAI_API_KEY"
-os.environ['HF_TOKEN'] = "YOUR_HUGGINGFACE_TOKEN"
-```
 
+```
+** Note :- API Key from Free tier OpenAI account is not supported. **  
 ## Usage
 
 The following steps guide you through the process of utilizing the test-RAG-X library to optimize your RAG parameters:
 
 ```python
-from test_RAG_X.prag import parent_class
+import hagrid as hg
 
 # Specify the path to your PDF document
 file_path = "PATH_TO_YOUR_PDF_FILE"
 
 # Initialize the RAG-X instance
-my_instance = parent_class(file_path)
+model = hg.ChunkEvaluator(file_path)
 
 # Generate the optimal RAG parameters for your document
-score_card = my_instance.get_best_param()
+score_card = model.evaluate_parameters()
 
 # Output the results
 print(score_card)
 ```
 
 
-## Set parameters
+## Set parameters for evaluation
 
 If you wish to analyse the performance of your parameters, you can pass the parameters as below:
 ```python
 kwarg = {
-        'number_of_questions': 5, # Number of questions: type(int)
+        'number_of_questions': 5, # Number of questions used to evaluate the process: type(int)
         'chunk_size': 250, # Chunk size: type(int)
         'chunk_overlap': 0, # Chunk overlap size: type(int)
         'separator': '',  # Separator to be used for chunking if any, type(str)
         'strip_whitespace': False, # Strip white space, type(bool)
         'sentence_buffer_window': 3, # Sentence Buffer window, type(int) 
         'sentence_cutoff_percentile': 80, # Sentence chunk split percentile for spliting context, type(int), range(1,100)
         }
 
 # Specify the path to your PDF document
 file_path = "PATH_TO_YOUR_PDF_FILE"
 
 # Initialize the RAG-X instance
-my_instance = parent_class(file_path, **kwargs)
+model = hg.ChunkEvaluator(file_path, **kwargs)
 
 # Generate the optimal RAG parameters for your document
-score_card = my_instance.get_best_param()
+score_card = model.evaluate_parameters()
 
-# Output the results
+# Output the results, output will be a pandas dataframe
 print(score_card)
 ```
+
+## Output
+![output_image](pictures/result.png)
+
+## Contribution
+We are open for contributions and any feedback from the users. Feel free to contact us.
+
+## Contact Us:
+If you wish to integarte GenAI into your company, please contact at ...
```

### Comparing `test_RAG_X-0.1.3/test_RAG_X/clean_it.py` & `test_RAG_X-0.2.1/test_RAG_X/text_cleaner.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,56 +6,67 @@
     clean_extra_whitespace,
     clean_non_ascii_chars,
     clean_ordered_bullets,
     clean_postfix,
     clean_prefix,
     clean_trailing_punctuation,
     group_broken_paragraphs,
-    remove_punctuation,
-    replace_unicode_quotes,
 )
 from unstructured.partition.html import partition_html
 from unstructured.documents.elements import Text
+from test_RAG_X.library_exceptions import *
 
 
+class TextCleaner:
+    """
+    A class for cleaning unstructured text.
+    """
+    def __init__(self, uncleaned_text: str, parent_instance=None):
+        """
+        Initialize the TextCleaner with uncleaned text.
 
-
-class TextCleaner():
-
-    def __init__(self, uncleaned_text:str):
+        Args:
+            uncleaned_text (str): The unstructured text to be cleaned.
+            parent_instance: Parent instance (if any).
+        """
         self.uncleaned_text = uncleaned_text
 
-    def unstructured_text(self):
+    def clean_text(self) -> str:
         """
         Clean the unstructured text by applying all the cleaning operations.
 
         Args:
             uncleaned_text (str): The unstructured text to be cleaned.
 
         Returns:
             str: The cleaned text.
         """
-        # Creating an element from the text
-        text = self.uncleaned_text
-        element = Text(text)
-
-        # Applying all available operations
-        element.apply(replace_unicode_quotes)
-        # element.apply(bytes_string_to_string)
-        element.apply(clean)
-        element.apply(clean_bullets)
-        element.apply(clean_dashes)
-        element.apply(clean_extra_whitespace)
-        element.apply(clean_non_ascii_chars)
-        element.apply(clean_ordered_bullets)
-        element.apply(lambda text: clean_postfix(text, r"(END|STOP)", ignore_case=True))
-        element.apply(lambda text: clean_prefix(text, r"(SUMMARY|DESCRIPTION):", ignore_case=True))
-        element.apply(clean_trailing_punctuation)
-        element.text = group_broken_paragraphs(element.text)
-        # element.text = remove_punctuation(element.text)
-        elements = partition_html(text=element.text)
-        if elements:
-            element = elements[0]  # Considering only the first element
-
-        return element.text
-
-    
+        try:
+            # Creating an element from the text
+            text = self.uncleaned_text
+            element = Text(text)
+
+            # Applying all available operations
+            element.apply(replace_unicode_quotes)
+            element.apply(clean)
+            element.apply(clean_bullets)
+            element.apply(clean_dashes)
+            element.apply(clean_extra_whitespace)
+            element.apply(clean_non_ascii_chars)
+            element.apply(clean_ordered_bullets)
+            element.apply(
+                lambda text: clean_postfix(text, r"(END|STOP)", ignore_case=True)
+            )
+            element.apply(
+                lambda text: clean_prefix(
+                    text, r"(SUMMARY|DESCRIPTION):", ignore_case=True
+                )
+            )
+            element.apply(clean_trailing_punctuation)
+            element.text = group_broken_paragraphs(element.text)
+            elements = partition_html(text=element.text)
+            if elements:
+                element = elements[0]  # Considering only the first element
+
+            return element.text
+        except Exception as e:
+            raise f"An error occurred during text cleaning: {e}"
```

### Comparing `test_RAG_X-0.1.3/test_RAG_X/extractor.py` & `test_RAG_X-0.2.1/test_RAG_X/document_extractor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from unstructured.partition.pdf import partition_pdf
+from .library_exceptions import DocumentExtractorError,InvalidFilePath,InvalidFileType
+import os
+
 
 class DocumentExtractor:
     """
     A class for extracting data from a parsed PDF document.
     """
 
-    def __init__(self, file_path:str):
+    def __init__(self, file_path: str, parent_instance=None):
         self.file_path = file_path
 
-    def extract_data(self):
+    def extract_data(self) -> str:
         """
-        Extracts data from the loaded document content (list of images).
-
-        Args:
-            document_content (list): A list of PIL Image objects representing the converted pages.
+        Extracts data from the loaded document content.
 
         Returns:
             str: A string containing the extracted data.
 
         Raises:
-            Exception: If an error occurs during extraction.
+            DocumentExtractionError: If an error occurs during extraction.
         """
-
-        try:
-
-            elements = partition_pdf(filename=self.file_path) 
-            extracted_text = ''.join([str(element) for element in elements])
-            return extracted_text
-
-        except Exception as e:
-            raise Exception(f"Error during data extraction: {e}")
-        
+        if self.file_path.endswith(".pdf"):
+            if os.path.exists(self.file_path):
+                try:
+                    elements = partition_pdf(filename=self.file_path)
+                    extracted_text = "".join([str(element) for element in elements])
+                    return extracted_text
+                except:
+                    raise DocumentExtractorError()
+            else:
+                raise InvalidFilePath()
+        else:
+            raise InvalidFileType()
```

### Comparing `test_RAG_X-0.1.3/test_RAG_X/prag.py` & `test_RAG_X-0.2.1/test_RAG_X/hub.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,155 +1,217 @@
-
-from .chunk_it import Chunker
-from .extractor import DocumentExtractor
-from .clean_it import TextCleaner
-from .get_evaluation_question import GenerateEvaluationQuestions
 import pandas as pd
-
 from langchain_community.embeddings.sentence_transformer import (
     SentenceTransformerEmbeddings,
 )
-from .trulens import *
-
+from .tru_lens_evaluator import Chroma, TruLensEvaluator
+from .text_chunker import TextChunker
+from .document_extractor import DocumentExtractor
+from .text_cleaner import TextCleaner
+from .evaluation_question_generator import EvaluationQuestionGenerator
 from dotenv import load_dotenv
+from .library_exceptions import ApiKeyError
+import os
+
 
 load_dotenv()
 
+
 class ChunkEvaluator:
+    """
+    A class containing methods for evaluating chunking methods and determining the best parameters.
+    """
+
     def __init__(self, file_path, **kwargs):
-        expected_types = {
-                'number_of_questions': int,
-                'chunk_size': int, 
-                'chunk_overlap': int, 
-                'separator': str, 
-                'strip_whitespace': bool,
-                'sentence_buffer_window': int,
-                'sentence_cutoff_percentile': int,
-            }
+        """
+        Initialize the ChunkEvaluator with the file path and optional parameters.
 
+        Args:
+            file_path (str): The path to the input file.
+            **kwargs: Additional keyword arguments for configuring evaluation parameters.
+
+        Raises:
+            TypeError: If any parameter does not match the expected data type.
+        """
+        expected_types = {
+            "number_of_questions": int,
+            "chunk_size": int,
+            "chunk_overlap": int,
+            "separator": str,
+            "strip_whitespace": bool,
+            "sentence_buffer_window": int,
+            "sentence_cutoff_percentile": int,
+        }
         default_attributes = {
-            'number_of_questions': 5,
-            'chunk_size': 250, 
-            'chunk_overlap': 0, 
-            'separator': '', 
-            'strip_whitespace': False,
-            'sentence_buffer_window': 3,
-            'sentence_cutoff_percentile': 80,
+            "number_of_questions": 5,
+            "chunk_size": 250,
+            "chunk_overlap": 0,
+            "separator": "",
+            "strip_whitespace": False,
+            "sentence_buffer_window": 3,
+            "sentence_cutoff_percentile": 80,
         }
-            
         default_attributes.update(kwargs)
-    
+
         for key, value in default_attributes.items():
             expected_type = expected_types.get(key)
             if expected_type and not isinstance(value, expected_type):
                 raise TypeError(f"{key} must be of type {expected_type.__name__}")
             setattr(self, key, value)
 
         self.file_path = file_path
 
-        def __str__(self):
-            return self.text    
-
-
-
+    def __str__(self):
+        return self.text
 
     def reset_params(self):
         """
-        Resets all parameters to their default values.
+        Reset the evaluation parameters to default values.
+
+        Returns:
+            dict: A dictionary containing the default evaluation parameters.
         """
         return {
-                'chunk_size': '-', 
-                'chunk_overlap': '-', 
-                'separator': '-', 
-                'strip_whitespace': '-',
-                'sentence_buffer_window': '-',
-                'sentence_cutoff_percentile': '-',
-            }
-    
+            "chunk_size": "-",
+            "chunk_overlap": "-",
+            "separator": "-",
+            "strip_whitespace": "-",
+            "sentence_buffer_window": "-",
+            "sentence_cutoff_percentile": "-",
+        }
 
-    def evaluate_chunk(self, chunks, method_name, eval_questions):
+    def eval_function(self, chunks, method_name, eval_questions):
         """
         Evaluate the performance of a chunking method using the TruLens framework.
 
-        Parameters
-        ----------
-        chunks : list of str
-            The list of chunks to evaluate.
-        method_name : str
-            The name of the chunking method.
-        eval_questions : list of str
-            The list of evaluation questions.
-
-        Returns
-        -------
-        float
-            The performance score (Padas DataFrame) of the chunking method.
-
-        """
-        # persist_directory="01_coding/crucible/db"
-        embedding_function = SentenceTransformerEmbeddings(model_name="sentence-transformers/all-MiniLM-l6-v2")
-
-        # db = Chroma.from_documents(chunks, embedding_function, persist_directory=persist_directory)
-        db = Chroma.from_documents(chunks, embedding_function)
-        score = trulens_evaluation(evalation_questions = eval_questions, 
-                            vectorstore=db, chunking_type=method_name)
-        return score
+        Args:
+            chunks (list): A list of Document objects representing chunks of text.
+            method_name (str): The name of the chunking method being evaluated.
+            eval_questions (list): A list of evaluation questions.
 
-    
-    def find_best_params(self):
+        Returns:
+            float: The evaluation score.
+        """
+        try:
+            embedding_function = SentenceTransformerEmbeddings(
+                model_name="sentence-transformers/all-MiniLM-l6-v2"
+            )
+
+            db = Chroma.from_documents(chunks, embedding_function)
+            score = TruLensEvaluator.trulens_evaluation(
+                evaluation_questions=eval_questions,
+                vectorstore=db,
+                chunking_type=method_name,
+            )
+            return score
+
+        except Exception as e:
+            raise e 
+
+    def rearrangeGrid(self,method_eval_score):
+        selected_df_filtered = []
+        param_list = [
+            "chunk_size",
+            "chunk_overlap",
+            "separator",
+            "strip_whitespace",
+            "sentence_buffer_window",
+            "sentence_cutoff_percentile",
+        ]
+        selected_columns = [
+            "app_id",
+            "input",
+            "output",
+            "Answer Relevance",
+            "Context Relevance",
+            "Groundedness",
+        ]
+        selected_columns.extend(param_list)
+        for df in method_eval_score:
+            selected_df = df[[col for col in selected_columns if col in df.columns]]
+            selected_df_filtered.append(selected_df)
+        merged_df = pd.concat(selected_df_filtered, ignore_index=True)
+        groupby_columns = ["app_id"] + param_list
+        grouped_df = (
+            merged_df.groupby(groupby_columns)[
+                ["Answer Relevance", "Context Relevance", "Groundedness"]
+            ]
+            .mean()
+            .reset_index()
+        )
+        return grouped_df
+
+    #*************************Main Function************************
+    #*****************************************************************
+    def evaluate_parameters(self):
         """
-        This function returns the best parameters for the chunking method based on the evaluation of the performance of the chunking method.
+        Determine the best parameters for the chunking method based on performance evaluation.
 
         Returns:
-            pandas.DataFrame: The parameters summary for the chunking method based on the evaluation of the performance of the chunking method.
+            pandas.DataFrame: A DataFrame containing the best parameters and their corresponding evaluation scores.
         """
-        extractor_instance = DocumentExtractor(file_path=self.file_path)
+        if 'OPENAI_API_KEY' not in os.environ:
+            raise ApiKeyError()
+        # Create an instance of DocumentExtractor to extract data from the file
+        extractor_instance = DocumentExtractor(
+            file_path=self.file_path, parent_instance=self
+        )
+        # Extract uncleaned text data using the extractor_instance
         uncleaned_text = extractor_instance.extract_data()
 
-        cleaner_instance = TextCleaner(uncleaned_text=uncleaned_text)
-        cleaned_text = cleaner_instance.unstructured_text()
+        # Create an instance of TextCleaner to clean the unstructured text
+        cleaner_instance = TextCleaner(
+            uncleaned_text=uncleaned_text, parent_instance=self
+        )
+        # Clean the unstructured text using the cleaner_instance
+        cleaned_text = cleaner_instance.clean_text()
+
+        # Generate evaluation questions using EvaluationQuestionGenerator
+        # based on the cleaned text and the specified number of questions
+ 
+        eval_questions = EvaluationQuestionGenerator(
+            document=cleaned_text, number_of_questions=self.number_of_questions
+        ).get_evaluation_questions()
+        
 
-        eval_questions_instance = GenerateEvaluationQuestions(document=cleaned_text, number_of_questions=self.number_of_questions)
-        eval_questions = eval_questions_instance.get_evaluation_questions()
+        # Get a list of methods from the TextChunker class that are callable and not private
+        methods_list = [
+            method
+            for method in dir(TextChunker)
+            if callable(getattr(TextChunker, method)) and not method.startswith("__")
+        ]
 
-        methods_list = [method for method in dir(Chunker)
-                if callable(getattr(Chunker, method)) and not method.startswith('__')]
-        
-        chunk_instance = Chunker(clean_text=cleaned_text, parent_instance=self)
+        # Create an instance of TextChunker with the cleaned text and parent instance
+        chunk_text = TextChunker(clean_text=cleaned_text, parent_instance=self)
 
+        # Initialize an empty list to store evaluation scores for each method
         method_eval_score = []
+
+        # Iterate through the methods in the methods_list
         for method_name in methods_list:
-            print(method_name)
-            method = getattr(chunk_instance, method_name, None)  
+
+            # Get the method from the chunk_instance by its name
+            method = getattr(chunk_text, method_name, None)
+
+            # Check if the method exists
             if method:
+                # Call the method to get chunks and parameters
                 chunks, params = method()
-                
-                model_results = self.evaluate_chunk(chunks=chunks, method_name=method_name, eval_questions=eval_questions)
+
+                # Evaluate the performance of the method using TruLens framework
+                model_results = self.eval_function(
+                    chunks=chunks,
+                    method_name=method_name,
+                    eval_questions=eval_questions,
+                )
+                # Create a DataFrame containing the parameters
                 params_df = pd.DataFrame([params])
-                repeated_params_df = pd.concat([params_df] * len(model_results), ignore_index=True)
+                # Repeat the parameters DataFrame for each model result
+                repeated_params_df = pd.concat(
+                    [params_df] * len(model_results), ignore_index=True
+                )
 
                 out = pd.concat([model_results, repeated_params_df], axis=1)
                 method_eval_score.append(out)
-        
-
-        selected_df_filtered=[]
-        param_list = [
-            'chunk_size', 
-            'chunk_overlap', 
-            'separator', 
-            'strip_whitespace',
-            'sentence_buffer_window',
-            'sentence_cutoff_percentile',
-        ]
-        # Selected columns
-        selected_columns = ["app_id","input", "output", "Answer Relevance", "Context Relevance", "Groundedness"]
-        selected_columns.extend(param_list)
-        for df in method_eval_score:
-            selected_df = df[[col for col in selected_columns if col in df.columns]]
-            selected_df_filtered.append(selected_df)
-        merged_df = pd.concat(selected_df_filtered, ignore_index=True)
-        groupby_columns = ['app_id'] + param_list
-        grouped_df = merged_df.groupby(groupby_columns)[["Answer Relevance", "Context Relevance", "Groundedness"]].mean().reset_index()
-        return grouped_df
-
-
 
+        return self.rearrangeGrid(method_eval_score)    
+            
+
```

### Comparing `test_RAG_X-0.1.3/test_RAG_X/utils.py` & `test_RAG_X-0.2.1/test_RAG_X/text_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,96 @@
-import numpy as np
 import os
+import numpy as np
 from sklearn.metrics.pairwise import cosine_similarity
 from langchain.docstore.document import Document
+from langchain_community.embeddings import HuggingFaceInferenceAPIEmbeddings
 
 
 def combine_sentences(sentences, buffer_size=1):
-    # Go through each sentence dict
-    for i in range(len(sentences)):
-
-        # Create a string that will hold the sentences which are joined
-        combined_sentence = ''
+    """
+    Combines adjacent sentences within a buffer to create new combined sentences.
 
-        # Add sentences before the current one, based on the buffer size.
-        for j in range(i - buffer_size, i):
-            # Check if the index j is not negative (to avoid index out of range like on the first one)
-            if j >= 0:
-                # Add the sentence at index j to the combined_sentence string
-                combined_sentence += sentences[j]['sentence'] + ' '
-
-        # Add the current sentence
-        combined_sentence += sentences[i]['sentence']
-
-        # Add sentences after the current one, based on the buffer size
-        for j in range(i + 1, i + 1 + buffer_size):
-            # Check if the index j is within the range of the sentences list
-            if j < len(sentences):
-                # Add the sentence at index j to the combined_sentence string
-                combined_sentence += ' ' + sentences[j]['sentence']
-
-        # Then add the whole thing to your dict
-        # Store the combined sentence in the current sentence dict
-        sentences[i]['combined_sentence'] = combined_sentence
-
-    return sentences
+    Args:
+        sentences (list): List of dictionaries containing sentence information.
+        buffer_size (int, optional): Size of the buffer for combining sentences. Defaults to 1.
+
+    Returns:
+        list: List of dictionaries with combined_sentence added.
+    """
+    try:
+        for i in range(len(sentences)):
+            combined_sentence = ''
+            for j in range(i - buffer_size, i):
+                if j >= 0:
+                    combined_sentence += sentences[j]['sentence'] + ' '
+            combined_sentence += sentences[i]['sentence']
+            for j in range(i + 1, i + 1 + buffer_size):
+                if j < len(sentences):
+                    combined_sentence += ' ' + sentences[j]['sentence']
+            sentences[i]['combined_sentence'] = combined_sentence
+        return sentences
+    except Exception as e:
+        print(f"Error in combine_sentences: {e}")
+        return []
 
 
 def calculate_cosine_distances(sentences):
-    distances = []
-    
-    for i in range(len(sentences) - 1):
-        embedding_current = sentences[i]['combined_sentence_embedding']
-        embedding_next = sentences[i + 1]['combined_sentence_embedding']
-
-        # Calculate cosine similarity
-        similarity = cosine_similarity([embedding_current], [embedding_next])[0][0]
-
-        # Convert to cosine distance
-        distance = 1 - similarity
-
-        # Append cosine distance to the list
-        distances.append(distance)
-
-        # Store distance in the dictionary
-        sentences[i]['distance_to_next'] = distance
-
-    # Optionally handle the last sentence
-    # sentences[-1]['distance_to_next'] = None  # or a default value
+    """
+    Calculates the cosine distances between combined sentences.
 
-    return distances, sentences
+    Args:
+        sentences (list): List of dictionaries containing combined sentences and embeddings.
 
+    Returns:
+        tuple: Pair of lists containing distances and updated sentences.
+    """
+    try:
+        distances = []
+        for i in range(len(sentences) - 1):
+            embedding_current = sentences[i]['combined_sentence_embedding']
+            embedding_next = sentences[i + 1]['combined_sentence_embedding']
+            similarity = cosine_similarity([embedding_current], [embedding_next])[0][0]
+            distance = 1 - similarity
+            distances.append(distance)
+            sentences[i]['distance_to_next'] = distance
+        return distances, sentences
+    except Exception as e:
+        print(f"Error in calculate_cosine_distances: {e}")
+        return [], []
 
 
 def create_chunk(distances, sentences, cutoff_percentile=90):
+    """
+    Creates chunks of text based on cosine distance thresholds.
 
-    breakpoint_distance_threshold = np.percentile(distances, cutoff_percentile) # If you want more chunks, lower the percentile cutoff
-
-    # Then we'll get the index of the distances that are above the threshold. This will tell us where we should split our text
-    indices_above_thresh = [i for i, x in enumerate(distances) if x > breakpoint_distance_threshold] # The indices of those breakpoints on your list
-
-    # Initialize the start index
-    start_index = 0
-
-    # Create a list to hold the grouped sentences
-    chunks = []
-
-    # Iterate through the breakpoints to slice the sentences
-    for index in indices_above_thresh:
-        # The end index is the current breakpoint
-        end_index = index
-
-        # Slice the sentence_dicts from the current start index to the end index
-        group = sentences[start_index:end_index + 1]
-        combined_text = ' '.join([d['sentence'] for d in group])
-        chunks.append(combined_text)
-
-        # Update the start index for the next group
-        start_index = index + 1
-
-    # The last group, if any sentences remain
-    if start_index < len(sentences):
-        combined_text = ' '.join([d['sentence'] for d in sentences[start_index:]])
-        chunks.append(combined_text)
-
-    chunks_doc = []
-    for i, chunk in enumerate(chunks):
-      doc = Document(page_content=chunk, metadata={"source": f"chunk:{i}"})
-      chunks_doc.append(doc)
-
-    return chunks_doc
+    Args:
+        distances (list): List of cosine distances between combined sentences.
+        sentences (list): List of dictionaries containing combined sentences.
+        cutoff_percentile (int, optional): Percentile threshold for cosine distances. Defaults to 90.
+
+    Returns:
+        list: List of Document objects representing chunks of text.
+    """
+    try:
+        breakpoint_distance_threshold = np.percentile(distances, cutoff_percentile)
+        indices_above_thresh = [i for i, x in enumerate(distances) if x > breakpoint_distance_threshold]
+        start_index = 0
+        chunks = []
+        for index in indices_above_thresh:
+            end_index = index
+            group = sentences[start_index:end_index + 1]
+            combined_text = ' '.join([d['sentence'] for d in group])
+            chunks.append(combined_text)
+            start_index = index + 1
+        if start_index < len(sentences):
+            combined_text = ' '.join([d['sentence'] for d in sentences[start_index:]])
+            chunks.append(combined_text)
+        chunks_doc = []
+        for i, chunk in enumerate(chunks):
+            doc = Document(page_content=chunk, metadata={"source": f"chunk:{i}"})
+            chunks_doc.append(doc)
+        return chunks_doc
+    except Exception as e:
+        print(f"Error in create_chunk: {e}")
+        return []
 
+
```

### Comparing `test_RAG_X-0.1.3/test_RAG_X.egg-info/PKG-INFO` & `test_RAG_X-0.2.1/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,127 @@
-Metadata-Version: 2.1
-Name: test-RAG-X
-Version: 0.1.3
-Summary: This library is to search the best parameters across different steps of the RAG process.
-Home-page: https://github.com/hidevscommunity/gen-ai-library/tree/main/Ankit
-Author: Ankit
-Author-email: a.baliyan008@gmail.com
-License: MIT
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: langchain==0.1.13
-Requires-Dist: langchain-openai>=0.1.1
-Requires-Dist: trulens-eval==0.27.0
-Requires-Dist: chromadb==0.4.24
-Requires-Dist: sentence-transformers==2.6.1
-Requires-Dist: unstructured[pdf]==0.13.0
-
-
----
-
-# RAG-X Library
-
-## Overview
-
-RAG-X is a comprehensive library designed to optimize Retrieval-Augmented Generation (RAG) processes. It provides a suite of tools to automatically determine the best parameters for processing specific documents. This includes selecting appropriate chunking techniques, embedding models, vector databases, and Language Model (LLM) configurations.
-
-### Key Features:
-- **Adaptive Chunking:** Incorporates four advanced text chunking methodologies to enhance the handling of diverse document structures.
-  - Specific Text Splitting
-  - Recursive Text Splitting
-  - Sentence Window Splitting
-  - Semantic Window Splitting
-- **Expandability:** Future versions will introduce additional chunking strategies and enhancements based on user feedback and ongoing research.
-- **Compatibility:** Designed to seamlessly integrate with a wide range of embedding models and vector databases.
-
-## Getting Started
-
-### Installation
-
-To get started, install the test_RAG_X library using the following command:
-
-```bash
-pip install test-RAG-X
-```
-
-To verify the installation and view library details, execute:
-
-```bash
-pip show test_RAG_X
-```
-
-### Setting Up Your Environment
-
-Before diving into the functionality of test-RAG-X, ensure that your environment variables are properly configured with your OpenAI API key and your Hugging Face token:
-
-```python
-import os
-
-os.environ['OPENAI_API_KEY'] = "YOUR_OPENAI_API_KEY"
-os.environ['HF_TOKEN'] = "YOUR_HUGGINGFACE_TOKEN"
-```
-
-## Usage
-
-The following steps guide you through the process of utilizing the test-RAG-X library to optimize your RAG parameters:
-
-```python
-from test_RAG_X.prag import parent_class
-
-# Specify the path to your PDF document
-file_path = "PATH_TO_YOUR_PDF_FILE"
-
-# Initialize the RAG-X instance
-my_instance = parent_class(file_path)
-
-# Generate the optimal RAG parameters for your document
-score_card = my_instance.get_best_param()
-
-# Output the results
-print(score_card)
-```
-
-
-## Set parameters
-
-If you wish to analyse the performance of your parameters, you can pass the parameters as below:
-```python
-kwarg = {
-        'number_of_questions': 5, # Number of questions: type(int)
-        'chunk_size': 250, # Chunk size: type(int)
-        'chunk_overlap': 0, # Chunk overlap size: type(int)
-        'separator': '',  # Separator to be used for chunking if any, type(str)
-        'strip_whitespace': False, # Strip white space, type(bool)
-        'sentence_buffer_window': 3, # Sentence Buffer window, type(int) 
-        'sentence_cutoff_percentile': 80, # Sentence chunk split percentile for spliting context, type(int), range(1,100)
-        }
-
-# Specify the path to your PDF document
-file_path = "PATH_TO_YOUR_PDF_FILE"
-
-# Initialize the RAG-X instance
-my_instance = parent_class(file_path, **kwargs)
-
-# Generate the optimal RAG parameters for your document
-score_card = my_instance.get_best_param()
-
-# Output the results
-print(score_card)
-```
+Metadata-Version: 2.1
+Name: test_RAG_X
+Version: 0.2.1
+Summary: This library is to search the best parameters across different steps of the RAG process.
+Home-page: https://github.com/hidevscommunity/gen-ai-library/tree/main/Ankit
+Author: Ankit
+Author-email: a.baliyan008@gmail.com
+License: MIT
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: langchain>=0.1.13
+Requires-Dist: langchain-openai>=0.1.1
+Requires-Dist: trulens-eval>=0.27.0
+Requires-Dist: chromadb>=0.4.24
+Requires-Dist: sentence-transformers>=2.6.1
+Requires-Dist: unstructured[pdf]==0.13.0
+
+
+---
+
+# RAG-X Library
+
+## Overview
+
+RAG-X is a comprehensive library designed to optimize Retrieval-Augmented Generation (RAG) processes. It provides a suite of tools to automatically determine the best parameters for processing specific documents. This includes selecting appropriate chunking techniques, embedding models, vector databases, and Language Model (LLM) configurations.
+
+## Flow Chart
+
+![Flow Chart](pictures/structure.png)
+
+### Key Features:
+- **Adaptive Chunking:** Incorporates four advanced text chunking methodologies to enhance the handling of diverse document structures.
+  - Specific Text Splitting
+  - Recursive Text Splitting
+  - Sentence Window Splitting
+  - Semantic Window Splitting
+- **Expandability:** Future versions will introduce additional chunking strategies and enhancements based on user feedback and ongoing research.
+- **Compatibility:** Designed to seamlessly integrate with a wide range of embedding models and vector databases.
+
+## Getting Started
+
+### Installation
+
+To get started, install the test_RAG_X library using the following command:
+
+```bash
+pip install test-RAG-X
+```
+
+To verify the installation and view library details, execute:
+
+```bash
+pip show test_RAG_X
+```
+
+### Setting Up Your Environment
+
+Before diving into the functionality of test-RAG-X, ensure that your environment variables are properly configured with your OpenAI API key and your Hugging Face token:
+
+```python
+import os
+
+os.environ['OPENAI_API_KEY'] = "YOUR_OPENAI_API_KEY"
+
+```
+** Note :- API Key from Free tier OpenAI account is not supported. **  
+## Usage
+
+The following steps guide you through the process of utilizing the test-RAG-X library to optimize your RAG parameters:
+
+```python
+import hagrid as hg
+
+# Specify the path to your PDF document
+file_path = "PATH_TO_YOUR_PDF_FILE"
+
+# Initialize the RAG-X instance
+model = hg.ChunkEvaluator(file_path)
+
+# Generate the optimal RAG parameters for your document
+score_card = model.evaluate_parameters()
+
+# Output the results
+print(score_card)
+```
+
+
+## Set parameters for evaluation
+
+If you wish to analyse the performance of your parameters, you can pass the parameters as below:
+```python
+kwarg = {
+        'number_of_questions': 5, # Number of questions used to evaluate the process: type(int)
+        'chunk_size': 250, # Chunk size: type(int)
+        'chunk_overlap': 0, # Chunk overlap size: type(int)
+        'separator': '',  # Separator to be used for chunking if any, type(str)
+        'strip_whitespace': False, # Strip white space, type(bool)
+        'sentence_buffer_window': 3, # Sentence Buffer window, type(int) 
+        'sentence_cutoff_percentile': 80, # Sentence chunk split percentile for spliting context, type(int), range(1,100)
+        }
+
+# Specify the path to your PDF document
+file_path = "PATH_TO_YOUR_PDF_FILE"
+
+# Initialize the RAG-X instance
+model = hg.ChunkEvaluator(file_path, **kwargs)
+
+# Generate the optimal RAG parameters for your document
+score_card = model.evaluate_parameters()
+
+# Output the results, output will be a pandas dataframe
+print(score_card)
+```
+
+## Output
+![output_image](pictures/result.png)
+
+## Contribution
+We are open for contributions and any feedback from the users. Feel free to contact us.
+
+## Contact Us:
+If you wish to integarte GenAI into your company, please contact at ...
```

