# Comparing `tmp/notdiamond-0.1.0b0.tar.gz` & `tmp/notdiamond-0.1.1b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notdiamond-0.1.0b0.tar", max compression
+gzip compressed data, was "notdiamond-0.1.1b0.tar", max compression
```

## Comparing `notdiamond-0.1.0b0.tar` & `notdiamond-0.1.1b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4667 2024-04-09 10:12:26.438700 notdiamond-0.1.0b0/README.md
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.001993 notdiamond-0.1.0b0/notdiamond/__init__.py
--rw-r--r--   0        0        0      440 2024-04-02 07:43:11.002696 notdiamond-0.1.0b0/notdiamond/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.002740 notdiamond-0.1.0b0/notdiamond/llms/__init__.py
--rw-r--r--   0        0        0    20028 2024-04-08 18:48:14.498628 notdiamond-0.1.0b0/notdiamond/llms/llm.py
--rw-r--r--   0        0        0     4432 2024-04-08 18:48:14.499003 notdiamond-0.1.0b0/notdiamond/llms/provider.py
--rw-r--r--   0        0        0     4155 2024-04-08 18:48:14.499307 notdiamond-0.1.0b0/notdiamond/llms/providers.py
--rw-r--r--   0        0        0     6024 2024-04-08 18:48:14.499704 notdiamond-0.1.0b0/notdiamond/llms/request.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004168 notdiamond-0.1.0b0/notdiamond/metrics/__init__.py
--rw-r--r--   0        0        0     1155 2024-04-02 11:25:39.891484 notdiamond-0.1.0b0/notdiamond/metrics/metric.py
--rw-r--r--   0        0        0     1100 2024-04-06 09:04:10.351693 notdiamond-0.1.0b0/notdiamond/metrics/request.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004898 notdiamond-0.1.0b0/notdiamond/prompts/__init__.py
--rw-r--r--   0        0        0      147 2024-04-02 07:43:11.005796 notdiamond-0.1.0b0/notdiamond/prompts/hash.py
--rw-r--r--   0        0        0     7782 2024-04-06 09:04:10.351913 notdiamond-0.1.0b0/notdiamond/prompts/prompt.py
--rw-r--r--   0        0        0     1881 2024-04-06 09:04:10.352179 notdiamond-0.1.0b0/notdiamond/settings.py
--rw-r--r--   0        0        0      972 2024-04-02 07:43:11.007948 notdiamond-0.1.0b0/notdiamond/types.py
--rw-r--r--   0        0        0     1422 2024-04-09 10:13:37.348468 notdiamond-0.1.0b0/pyproject.toml
--rw-r--r--   0        0        0     5769 1970-01-01 00:00:00.000000 notdiamond-0.1.0b0/PKG-INFO
+-rw-r--r--   0        0        0     4667 2024-04-09 10:12:26.438700 notdiamond-0.1.1b0/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.001993 notdiamond-0.1.1b0/notdiamond/__init__.py
+-rw-r--r--   0        0        0      440 2024-04-02 07:43:11.002696 notdiamond-0.1.1b0/notdiamond/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.002740 notdiamond-0.1.1b0/notdiamond/llms/__init__.py
+-rw-r--r--   0        0        0    31483 2024-04-12 16:11:39.811490 notdiamond-0.1.1b0/notdiamond/llms/llm.py
+-rw-r--r--   0        0        0     4432 2024-04-08 18:48:14.499003 notdiamond-0.1.1b0/notdiamond/llms/provider.py
+-rw-r--r--   0        0        0     4155 2024-04-08 18:48:14.499307 notdiamond-0.1.1b0/notdiamond/llms/providers.py
+-rw-r--r--   0        0        0    11277 2024-04-12 16:11:39.811793 notdiamond-0.1.1b0/notdiamond/llms/request.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004168 notdiamond-0.1.1b0/notdiamond/metrics/__init__.py
+-rw-r--r--   0        0        0     1155 2024-04-02 11:25:39.891484 notdiamond-0.1.1b0/notdiamond/metrics/metric.py
+-rw-r--r--   0        0        0     1100 2024-04-06 09:04:10.351693 notdiamond-0.1.1b0/notdiamond/metrics/request.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004898 notdiamond-0.1.1b0/notdiamond/prompts/__init__.py
+-rw-r--r--   0        0        0      147 2024-04-02 07:43:11.005796 notdiamond-0.1.1b0/notdiamond/prompts/hash.py
+-rw-r--r--   0        0        0     7782 2024-04-06 09:04:10.351913 notdiamond-0.1.1b0/notdiamond/prompts/prompt.py
+-rw-r--r--   0        0        0     1881 2024-04-06 09:04:10.352179 notdiamond-0.1.1b0/notdiamond/settings.py
+-rw-r--r--   0        0        0      972 2024-04-02 07:43:11.007948 notdiamond-0.1.1b0/notdiamond/types.py
+-rw-r--r--   0        0        0     1479 2024-04-12 16:11:51.729779 notdiamond-0.1.1b0/pyproject.toml
+-rw-r--r--   0        0        0     5822 1970-01-01 00:00:00.000000 notdiamond-0.1.1b0/PKG-INFO
```

### Comparing `notdiamond-0.1.0b0/README.md` & `notdiamond-0.1.1b0/README.md`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0b0/notdiamond/llms/llm.py` & `notdiamond-0.1.1b0/notdiamond/llms/llm.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 """NDLLM Class"""
 
 import time
-from typing import Any, Dict, Iterator, List, Optional, Union
+from typing import Any, AsyncIterator, Dict, Iterator, List, Optional, Union
 
 from langchain.prompts import PromptTemplate
 from langchain_anthropic import ChatAnthropic
-from langchain_community.chat_models.cohere import ChatCohere
+from langchain_cohere.chat_models import ChatCohere
 from langchain_core.callbacks.manager import CallbackManagerForLLMRun
 from langchain_core.language_models.llms import LLM
 from langchain_core.messages import AIMessage, BaseMessage, BaseMessageChunk
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_google_genai import ChatGoogleGenerativeAI
 from langchain_google_genai.chat_models import ChatGoogleGenerativeAIError
 from langchain_mistralai.chat_models import ChatMistralAI
 from langchain_openai import ChatOpenAI
 from langchain_together import Together
 from litellm import token_counter
 
 from notdiamond import settings
 from notdiamond.exceptions import ApiError, MissingLLMProviders
 from notdiamond.llms.provider import NDLLMProvider
-from notdiamond.llms.request import model_select, report_latency
+from notdiamond.llms.request import amodel_select, model_select, report_latency
 from notdiamond.metrics.metric import NDMetric
 from notdiamond.prompts.prompt import NDChatPromptTemplate, NDPromptTemplate
 from notdiamond.types import NDApiKeyValidator
 
 
 class NDLLM(LLM):
     """
@@ -188,40 +188,42 @@
         run_manager: Optional[CallbackManagerForLLMRun] = None,
         **kwargs: Any,
     ) -> str:
         if stop is not None:
             raise ValueError("stop kwargs are not permitted.")
         return "This function is deprecated for the latest LangChain version, use invoke instead"
 
-    def invoke(
+    async def invoke_base(
         self,
         prompt_template: Union[
             NDPromptTemplate,
             PromptTemplate,
             NDChatPromptTemplate,
             ChatPromptTemplate,
             str,
         ],
         input: Optional[Dict[str, Any]] = None,
         metric: NDMetric = NDMetric("accuracy"),
+        async_mode: bool = False,
         **kwargs,
     ) -> AIMessage:
         """
         Function to invoke the LLM. Behind the scenes what happens:
         1. API call to NotDiamond backend to get the most suitable LLM for the given prompt
-        2. Invoke the returned LLM client side
+        2. Invoke the returned LLM client side (async or sync)
         3. Return the response
 
         Parameters:
             prompt_template (Union[ NDPromptTemplate, PromptTemplate, NDChatPromptTemplate, ChatPromptTemplate, str, ]):
                 the prompt template defined by the user. It also supports Langchain prompt template types.
             input (Optional[Dict[str, Any]], optional): If the prompt_template contains variables, use input to specify
                                                         the values for those variables. Defaults to None, assuming no variables.
             metric (NDMetric, optional): Metric used by NotDiamond router to choose the best LLM.
                                             Defaults to NDMetric("accuracy").
+            async_mode (bool, optional): If set to True, the function will be async. Defaults to False.
             **kwargs: Any other arguments that are supported by Langchain's invoke method, will be passed through.
 
         Raises:
             ApiError: when the NotDiamond API fails
 
         Returns:
             AIMessage: type defined by Langchain, contains the response from the LLM.
@@ -232,23 +234,34 @@
             input = {}
 
         prompt_template.partial_variables = {
             **prompt_template.partial_variables,
             **input,
         }
 
-        best_llm, session_id = model_select(
-            prompt_template=prompt_template,
-            llm_providers=self.llm_providers,
-            metric=metric,
-            notdiamond_api_key=self.api_key,
-            max_model_depth=self.max_model_depth,
-            preference_weights=self.preference_weights,
-            preference_id=self.preference_id,
-        )
+        if async_mode:
+            best_llm, session_id = await amodel_select(
+                prompt_template=prompt_template,
+                llm_providers=self.llm_providers,
+                metric=metric,
+                notdiamond_api_key=self.api_key,
+                max_model_depth=self.max_model_depth,
+                preference_weights=self.preference_weights,
+                preference_id=self.preference_id,
+            )
+        else:
+            best_llm, session_id = model_select(
+                prompt_template=prompt_template,
+                llm_providers=self.llm_providers,
+                metric=metric,
+                notdiamond_api_key=self.api_key,
+                max_model_depth=self.max_model_depth,
+                preference_weights=self.preference_weights,
+                preference_id=self.preference_id,
+            )
 
         is_default = False
         if not best_llm:
             best_llm = self.default_llm_provider
             is_default = True
 
             if best_llm is None:
@@ -264,18 +277,22 @@
             if self.latency_tracking:
                 result = self._invoke_with_latency_tracking(
                     session_id=session_id,
                     chain=chain,
                     llm_provider=best_llm,
                     is_default=is_default,
                     input=input,
+                    async_mode=async_mode,
                     **kwargs,
                 )
             else:
-                result = chain.invoke(input, **kwargs)
+                if async_mode:
+                    result = await chain.ainvoke(input, **kwargs)
+                else:
+                    result = chain.invoke(input, **kwargs)
         except (ChatGoogleGenerativeAIError, ValueError) as e:
             if (
                 isinstance(prompt_template, NDChatPromptTemplate)
                 and best_llm.provider == "google"
             ):
                 print(
                     f"WARNING: Google model's chat messages are violating requirements with error {e}."
@@ -302,29 +319,133 @@
                     if self.latency_tracking:
                         result = self._invoke_with_latency_tracking(
                             session_id=session_id,
                             chain=chain,
                             llm_provider=best_llm,
                             is_default=is_default,
                             input=input,
+                            async_mode=async_mode,
                             **kwargs,
                         )
                     else:
-                        result = chain.invoke(input, **kwargs)
+                        if async_mode:
+                            result = await chain.ainvoke(input, **kwargs)
+                        else:
+                            result = chain.invoke(input, **kwargs)
                 else:
                     raise e
             else:
                 raise e
 
         if isinstance(result, str):
             result = AIMessage(content=result)
 
         return result, session_id, best_llm
 
+    def invoke(
+        self,
+        prompt_template: Union[
+            NDPromptTemplate,
+            PromptTemplate,
+            NDChatPromptTemplate,
+            ChatPromptTemplate,
+            str,
+        ],
+        input: Optional[Dict[str, Any]] = None,
+        metric: NDMetric = NDMetric("accuracy"),
+        **kwargs,
+    ) -> AIMessage:
+        """
+        Function to invoke the LLM. Behind the scenes what happens:
+        1. API call to NotDiamond backend to get the most suitable LLM for the given prompt
+        2. Invoke the returned LLM client side
+        3. Return the response
+
+        Parameters:
+            prompt_template (Union[ NDPromptTemplate, PromptTemplate, NDChatPromptTemplate, ChatPromptTemplate, str, ]):
+                the prompt template defined by the user. It also supports Langchain prompt template types.
+            input (Optional[Dict[str, Any]], optional): If the prompt_template contains variables, use input to specify
+                                                        the values for those variables. Defaults to None, assuming no variables.
+            metric (NDMetric, optional): Metric used by NotDiamond router to choose the best LLM.
+                                            Defaults to NDMetric("accuracy").
+            **kwargs: Any other arguments that are supported by Langchain's invoke method, will be passed through.
+
+        Raises:
+            ApiError: when the NotDiamond API fails
+
+        Returns:
+            AIMessage: type defined by Langchain, contains the response from the LLM.
+        """
+        return self.invoke_base(
+            prompt_template=prompt_template,
+            input=input,
+            metric=metric,
+            async_mode=False,
+            **kwargs,
+        )
+
+    async def ainvoke(
+        self,
+        prompt_template: Union[
+            NDPromptTemplate,
+            PromptTemplate,
+            NDChatPromptTemplate,
+            ChatPromptTemplate,
+            str,
+        ],
+        input: Optional[Dict[str, Any]] = None,
+        metric: NDMetric = NDMetric("accuracy"),
+        **kwargs,
+    ) -> AIMessage:
+        """
+        Function to invoke the LLM. Behind the scenes what happens:
+        1. API call to NotDiamond backend to get the most suitable LLM for the given prompt
+        2. Invoke the returned LLM client side
+        3. Return the response
+
+        Parameters:
+            prompt_template (Union[ NDPromptTemplate, PromptTemplate, NDChatPromptTemplate, ChatPromptTemplate, str, ]):
+                the prompt template defined by the user. It also supports Langchain prompt template types.
+            input (Optional[Dict[str, Any]], optional): If the prompt_template contains variables, use input to specify
+                                                        the values for those variables. Defaults to None, assuming no variables.
+            metric (NDMetric, optional): Metric used by NotDiamond router to choose the best LLM.
+                                            Defaults to NDMetric("accuracy").
+            **kwargs: Any other arguments that are supported by Langchain's invoke method, will be passed through.
+
+        Raises:
+            ApiError: when the NotDiamond API fails
+
+        Returns:
+            AIMessage: type defined by Langchain, contains the response from the LLM.
+        """
+        return await self.invoke_base(
+            prompt_template=prompt_template,
+            input=input,
+            metric=metric,
+            async_mode=True,
+            **kwargs,
+        )
+
     def stream(self, input=None, **kwargs) -> Iterator[BaseMessageChunk]:
+        """
+        This function calls the NotDiamond backend to fetch the most suitable model for the given prompt,
+        and calls the LLM client side to stream the response.
+
+        Parameters:
+            input (Optional[Dict[str, Any]], optional): If the prompt_template contains variables, use input to specify
+                                                        the values for those variables. Defaults to None, assuming no variables.
+            **kwargs: Any other arguments that are supported by Langchain's invoke method, will be passed through.
+
+        Raises:
+            ApiError: when the NotDiamond API fails
+
+        Yields:
+            Iterator[BaseMessageChunk]: returns the response in chunks
+        """
+
         prompt_template = self._prepare_prompt_template(prompt_template=input)
         best_llm, session_id = model_select(
             prompt_template=prompt_template,
             llm_providers=self.llm_providers,
             metric=NDMetric("accuracy"),
             notdiamond_api_key=self.api_key,
             max_model_depth=self.max_model_depth,
@@ -340,14 +461,96 @@
                     + " To avoid disruptions, we recommend setting a default fallback model or make max depth larger."
                 )
 
         llm = self._llm_from_provider(best_llm)
         for chunk in llm.stream(input, **kwargs):
             yield chunk
 
+    async def astream(
+        self, input=None, **kwargs
+    ) -> AsyncIterator[BaseMessageChunk]:
+        """
+        This function calls the NotDiamond backend to fetch the most suitable model for the given prompt,
+        and calls the LLM client side to stream the response. The function is async, so it's suitable for async codebases.
+
+        Parameters:
+            input (Optional[Dict[str, Any]], optional): If the prompt_template contains variables, use input to specify
+                                                        the values for those variables. Defaults to None, assuming no variables.
+            **kwargs: Any other arguments that are supported by Langchain's invoke method, will be passed through.
+
+        Raises:
+            ApiError: when the NotDiamond API fails
+
+        Yields:
+            AsyncIterator[BaseMessageChunk]: returns the response in chunks
+        """
+
+        prompt_template = self._prepare_prompt_template(prompt_template=input)
+        best_llm, session_id = await amodel_select(
+            prompt_template=prompt_template,
+            llm_providers=self.llm_providers,
+            metric=NDMetric("accuracy"),
+            notdiamond_api_key=self.api_key,
+            max_model_depth=self.max_model_depth,
+            preference_weights=self.preference_weights,
+            preference_id=self.preference_id,
+        )
+        if not best_llm:
+            best_llm = self.default_llm_provider
+
+            if best_llm is None:
+                raise ApiError(
+                    "ND couldn't find a suitable model to call."
+                    + " To avoid disruptions, we recommend setting a default fallback model or make max depth larger."
+                )
+
+        llm = self._llm_from_provider(best_llm)
+        async for chunk in llm.astream(input, **kwargs):
+            yield chunk
+
+    async def amodel_select(
+        self,
+        prompt_template: Optional[
+            Union[
+                NDPromptTemplate,
+                PromptTemplate,
+                NDChatPromptTemplate,
+                ChatPromptTemplate,
+                str,
+            ]
+        ],
+        input: Optional[Dict[str, Any]] = None,
+        metric: NDMetric = NDMetric("accuracy"),
+        **kwargs,
+    ) -> tuple[str, Optional[NDLLMProvider]]:
+        """
+        This function calls the NotDiamond backend to fetch the most suitable model for the given prompt,
+        and leaves the execution of the LLM call to the developer.
+        The function is async, so it's suitable for async codebases.
+
+        Parameters:
+            prompt_template (Union[ NDPromptTemplate, PromptTemplate, NDChatPromptTemplate, ChatPromptTemplate, str, ]):
+                the prompt template defined by the user. It also supports Langchain prompt template types.
+            input (Optional[Dict[str, Any]], optional): If the prompt_template contains variables, use input to specify
+                                                        the values for those variables. Defaults to None, assuming no variables.
+            metric (NDMetric, optional): Metric used by NotDiamond router to choose the best LLM.
+                                            Defaults to NDMetric("accuracy").
+            **kwargs: Any other arguments that are supported by Langchain's invoke method, will be passed through.
+
+        Returns:
+            tuple[str, Optional[NDLLMProvider]]: returns the session_id and the chosen LLM provider
+        """
+        return await self.model_select_core(
+            prompt_template=prompt_template,
+            input=input,
+            metric=metric,
+            async_mode=True,
+            **kwargs,
+        )
+
     def model_select(
         self,
         prompt_template: Optional[
             Union[
                 NDPromptTemplate,
                 PromptTemplate,
                 NDChatPromptTemplate,
@@ -371,56 +574,113 @@
             metric (NDMetric, optional): Metric used by NotDiamond router to choose the best LLM.
                                             Defaults to NDMetric("accuracy").
             **kwargs: Any other arguments that are supported by Langchain's invoke method, will be passed through.
 
         Returns:
             tuple[str, Optional[NDLLMProvider]]: returns the session_id and the chosen LLM provider
         """
+        return self.model_select_core(
+            prompt_template=prompt_template,
+            input=input,
+            metric=metric,
+            async_mode=False,
+            **kwargs,
+        )
+
+    async def model_select_core(
+        self,
+        prompt_template: Optional[
+            Union[
+                NDPromptTemplate,
+                PromptTemplate,
+                NDChatPromptTemplate,
+                ChatPromptTemplate,
+                str,
+            ]
+        ],
+        input: Optional[Dict[str, Any]] = None,
+        metric: NDMetric = NDMetric("accuracy"),
+        async_mode: bool = False,
+        **kwargs,
+    ):
+        """
+        This function calls the NotDiamond backend to fetch the most suitable model for the given prompt,
+        and leaves the execution of the LLM call to the developer.
+
+        Parameters:
+            prompt_template (Union[ NDPromptTemplate, PromptTemplate, NDChatPromptTemplate, ChatPromptTemplate, str, ]):
+                the prompt template defined by the user. It also supports Langchain prompt template types.
+            input (Optional[Dict[str, Any]], optional): If the prompt_template contains variables, use input to specify
+                                                        the values for those variables. Defaults to None, assuming no variables.
+            metric (NDMetric, optional): Metric used by NotDiamond router to choose the best LLM.
+                                            Defaults to NDMetric("accuracy").
+            async_mode (bool, optional): If set to True, the function will be async. Defaults to False.
+            **kwargs: Any other arguments that are supported by Langchain's invoke method, will be passed through.
+
+        Returns:
+            tuple[str, Optional[NDLLMProvider]]: returns the session_id and the chosen LLM provider
+        """
+
         prompt_template = self._prepare_prompt_template(prompt_template)
 
         if input is None:
             input = {}
 
         prompt_template.partial_variables = {
             **prompt_template.partial_variables,
             **input,
         }
 
-        best_llm, session_id = model_select(
-            prompt_template=prompt_template,
-            llm_providers=self.llm_providers,
-            metric=metric,
-            notdiamond_api_key=self.api_key,
-            max_model_depth=self.max_model_depth,
-            preference_weights=self.preference_weights,
-            preference_id=self.preference_id,
-        )
+        if async_mode:
+            best_llm, session_id = await amodel_select(
+                prompt_template=prompt_template,
+                llm_providers=self.llm_providers,
+                metric=metric,
+                notdiamond_api_key=self.api_key,
+                max_model_depth=self.max_model_depth,
+                preference_weights=self.preference_weights,
+                preference_id=self.preference_id,
+            )
+        else:
+            best_llm, session_id = model_select(
+                prompt_template=prompt_template,
+                llm_providers=self.llm_providers,
+                metric=metric,
+                notdiamond_api_key=self.api_key,
+                max_model_depth=self.max_model_depth,
+                preference_weights=self.preference_weights,
+                preference_id=self.preference_id,
+            )
 
         if not best_llm and self.default is not None:
             print("ND API error. Falling back to default provider.")
             best_llm = self.default_llm_provider
 
         return session_id, best_llm
 
-    def _invoke_with_latency_tracking(
+    async def _invoke_with_latency_tracking(
         self,
         session_id: str,
         chain: Any,
         llm_provider: NDLLMProvider,
         input: Optional[Dict[str, Any]] = {},
         is_default: bool = True,
+        async_mode: bool = False,
         **kwargs,
     ):
         if session_id in ("NO-SESSION-ID", "") and not is_default:
             raise ApiError(
                 "ND session_id is not valid for latency tracking. Please check the API response."
             )
 
         start_time = time.time()
-        result = chain.invoke(input, **kwargs)
+        if async_mode:
+            result = await chain.ainvoke(input, **kwargs)
+        else:
+            result = chain.invoke(input, **kwargs)
         end_time = time.time()
 
         if isinstance(result, str):
             result = AIMessage(content=result)
 
         tokens_completed = token_counter(
             model=llm_provider.model,
```

### Comparing `notdiamond-0.1.0b0/notdiamond/llms/provider.py` & `notdiamond-0.1.1b0/notdiamond/llms/provider.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0b0/notdiamond/llms/providers.py` & `notdiamond-0.1.1b0/notdiamond/llms/providers.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0b0/notdiamond/metrics/metric.py` & `notdiamond-0.1.1b0/notdiamond/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0b0/notdiamond/metrics/request.py` & `notdiamond-0.1.1b0/notdiamond/metrics/request.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0b0/notdiamond/prompts/prompt.py` & `notdiamond-0.1.1b0/notdiamond/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0b0/notdiamond/settings.py` & `notdiamond-0.1.1b0/notdiamond/settings.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0b0/notdiamond/types.py` & `notdiamond-0.1.1b0/notdiamond/types.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.0b0/pyproject.toml` & `notdiamond-0.1.1b0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "notdiamond"
-version = "0.1.0-beta"
+version = "0.1.1-beta"
 description = "Not Diamond Python Library"
 authors = ["Not Diamond <t5@notdiamond.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 langchain = ">=0.1.10"
@@ -13,21 +13,23 @@
 litellm = "^1.32.4"
 langchain-openai = "^0.0.5"
 python-dotenv = "^1.0.1"
 openai = ">=1.0.0"
 ppdeep = "^20200505"
 langchain-anthropic = "^0.1.4"
 langchain-community = "^0.0.28"
-cohere = "^4.56"
 langchain-mistralai = "^0.0.5"
 together = "^0.2.11"
 langchain-together = "^0.0.2.post1"
+aiohttp = "^3.9.3"
+langchain-cohere = "^0.1.1"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
+pytest-asyncio = "^0.23.6"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.1"
 pydantic = "^2.5.3"
 pre-commit = "^3.7.0"
 black = "^24.3.0"
 flake8 = "^7.0.0"
```

### Comparing `notdiamond-0.1.0b0/PKG-INFO` & `notdiamond-0.1.1b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: notdiamond
-Version: 0.1.0b0
+Version: 0.1.1b0
 Summary: Not Diamond Python Library
 Author: Not Diamond
 Author-email: t5@notdiamond.ai
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
 Requires-Dist: anthropic (>=0.20.0,<0.21.0)
-Requires-Dist: cohere (>=4.56,<5.0)
 Requires-Dist: langchain (>=0.1.10)
 Requires-Dist: langchain-anthropic (>=0.1.4,<0.2.0)
+Requires-Dist: langchain-cohere (>=0.1.1,<0.2.0)
 Requires-Dist: langchain-community (>=0.0.28,<0.0.29)
 Requires-Dist: langchain-google-genai (>=0.0.2)
 Requires-Dist: langchain-mistralai (>=0.0.5,<0.0.6)
 Requires-Dist: langchain-openai (>=0.0.5,<0.0.6)
 Requires-Dist: langchain-together (>=0.0.2.post1,<0.0.3)
 Requires-Dist: litellm (>=1.32.4,<2.0.0)
 Requires-Dist: openai (>=1.0.0)
```

