# Comparing `tmp/AgentBruno-0.0.3-py3-none-any.whl.zip` & `tmp/AgentBruno-0.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 14519 bytes, number of entries: 9
+Zip file size: 14631 bytes, number of entries: 9
 -rw-r--r--  2.0 unx      285 b- defN 24-Apr-09 05:03 AgentBruno/__init__.py
--rw-r--r--  2.0 unx    31667 b- defN 24-Apr-09 07:09 AgentBruno/research.py
--rw-r--r--  2.0 unx     2405 b- defN 24-Apr-09 06:19 AgentBruno/storm.py
--rw-r--r--  2.0 unx      351 b- defN 24-Apr-11 07:21 AgentBruno-0.0.3.dist-info/LICENSE
--rw-r--r--  2.0 unx    10024 b- defN 24-Apr-11 07:21 AgentBruno-0.0.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 07:21 AgentBruno-0.0.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 24-Apr-11 07:21 AgentBruno-0.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-11 07:21 AgentBruno-0.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      733 b- defN 24-Apr-11 07:21 AgentBruno-0.0.3.dist-info/RECORD
-9 files, 45640 bytes uncompressed, 13253 bytes compressed:  71.0%
+-rw-r--r--  2.0 unx    32166 b- defN 24-Apr-12 06:57 AgentBruno/research.py
+-rw-r--r--  2.0 unx     2429 b- defN 24-Apr-12 04:42 AgentBruno/storm.py
+-rw-r--r--  2.0 unx      351 b- defN 24-Apr-12 06:57 AgentBruno-0.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     9987 b- defN 24-Apr-12 06:57 AgentBruno-0.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 06:57 AgentBruno-0.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 24-Apr-12 06:57 AgentBruno-0.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-12 06:57 AgentBruno-0.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      732 b- defN 24-Apr-12 06:57 AgentBruno-0.0.4.dist-info/RECORD
+9 files, 46125 bytes uncompressed, 13365 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: AgentBruno/research.py
 Comment: 
 
 Filename: AgentBruno/storm.py
 Comment: 
 
-Filename: AgentBruno-0.0.3.dist-info/LICENSE
+Filename: AgentBruno-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: AgentBruno-0.0.3.dist-info/METADATA
+Filename: AgentBruno-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: AgentBruno-0.0.3.dist-info/WHEEL
+Filename: AgentBruno-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: AgentBruno-0.0.3.dist-info/entry_points.txt
+Filename: AgentBruno-0.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: AgentBruno-0.0.3.dist-info/top_level.txt
+Filename: AgentBruno-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: AgentBruno-0.0.3.dist-info/RECORD
+Filename: AgentBruno-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## AgentBruno/research.py

```diff
@@ -8,18 +8,18 @@
 from langchain_core.pydantic_v1 import BaseModel, Field, constr
 from langchain_core.prompts import ChatPromptTemplate
 from langchain_community.retrievers import WikipediaRetriever
 from langchain_core.runnables import RunnableLambda, chain as as_runnable, RunnableConfig
 from langchain_core.messages import AIMessage, HumanMessage, ToolMessage, AnyMessage
 from langgraph.graph import StateGraph, END
 from langchain_core.prompts import MessagesPlaceholder
-from langchain.vectorstores import Pinecone
+#from langchain.vectorstores import Pinecone
 from langchain_community.utilities.duckduckgo_search import DuckDuckGoSearchAPIWrapper
 from langchain_core.tools import tool
-from langchain_community.vectorstores import SKLearnVectorStore
+from langchain_community.vectorstores import SKLearnVectorStore, Pinecone
 from langchain_core.documents import Document
 from langchain_core.output_parsers import StrOutputParser
 from langchain_openai import ChatOpenAI, OpenAIEmbeddings
 
 # Pydantic models for handling subsections, sections, and outlines
 
 class Subsection(BaseModel):
@@ -84,15 +84,15 @@
     """
     section_title: str = Field(..., title="Title of the section")
     content: str = Field(..., title="Full content of the section")
     subsections: Optional[List[Subsection]] = Field(
         default=None,
         title="Titles and descriptions for each subsection of the Wikipedia page.",
     )
-    citations: List[str] = Field(default_factory=list)
+    citations: Optional[List[str]]  = Field(default_factory=list)
 
     @property
     def as_str(self) -> str:
         """
         Generates a string representation of the section, including its subsections and citations.
         """
         subsections = "\n\n".join(
@@ -431,15 +431,15 @@
     gen_queries_chain = gen_queries_prompt | fast_llm.with_structured_output(Queries, include_raw=True)
     
     
     class AnswerWithCitations(BaseModel):
         answer: str = Field(
             description="Comprehensive answer to the user's question with citations.",
         )
-        cited_urls: List[str] = Field(
+        cited_urls: Optional[List[str]]  = Field(
             description="List of urls cited in the answer.",
         )
     
         @property
         def as_str(self) -> str:
             return f"{self.answer}\n\nCitations:\n\n" + "\n".join(
                 f"[{i+1}]: {url}" for i, url in enumerate(self.cited_urls)
@@ -500,28 +500,40 @@
         name: str = "Subject_Matter_Expert",
         max_str_len: int = 15000
     ):
         name = sanitize_name(name)
         swapped_state = swap_roles(state, name)  # Convert all other AI messages
         queries = await gen_queries_chain.ainvoke(swapped_state)
         
+        
+        successful_results = []
+        
+        try:
             
-        query_results = await search_engine.abatch(
-            queries["parsed"].queries, config, return_exceptions=True
-        )
+            ## Logic to fetch data from Agent Bruno vectorstore
+            if pinecone_index != '':
+                #print("********** Pinecone index is provided.********")
+                vector_results = await search_knowledge_catalogue.abatch(queries["parsed"].queries)
+                #print("Vector store results: ", vector_results)
+                successful_results += vector_results
+                
+            query_results = await search_engine.abatch(
+                queries["parsed"].queries, config, return_exceptions=True
+            )
+        except Exception as e:
+            # Handle the exception here
+            print(f"An error occurred while fetching data from Agent Bruno vectorstore: {e}")
+            
+        
+        #successful_results.extend(res for res in query_results if not isinstance(res, Exception))
 
-        successful_results = [
+        successful_results += [
             res for res in query_results if not isinstance(res, Exception)
         ]
         
-        ## Logic to fetch data from Agent Bruno vectorstore
-        if pinecone_index != '':
-            #print("********** Pinecone index is provided.********")
-            vector_results = await search_knowledge_catalogue.abatch(queries["parsed"].queries)
-            successful_results.extend(vector_results)
         
         all_query_results = {
             res["url"]: res["content"] for results in successful_results for res in results
         }
 
         # We could be more precise about handling max token length if we wanted to here
         dumped = json.dumps(all_query_results)[:max_str_len]
@@ -693,15 +705,15 @@
         # Add reference documents to the list of all documents
         all_docs.extend(reference_docs)
     
     # Check if there are any reference documents
     if len(all_docs) > 0:
         # If reference documents exist, add them to the vector store
         
-        print("*****index_references****** : ", len(all_docs))
+        #print("*****index_references****** : ", len(all_docs))
         
         await vectorstore.aadd_documents(all_docs)
 
 
         
     else:
         # If there are no reference documents, handle it as an error
@@ -755,17 +767,17 @@
         # Format the retrieved documents
         formatted = "\n".join(
             [
                 f'<Document href="{doc.metadata["source"]}"/>\n{doc.page_content}\n</Document>'
                 for doc in docs
             ]
         )
-        print("****write_section*****")
-        print(formatted)
-        print("*********")
+        # print("****write_section*****")
+        # print(formatted)
+        # print("*********")
         return {"docs": formatted, **inputs}
 
     # Define the section writer pipeline
     section_writer = (
         retrieve
         | section_writer_prompt
         | long_context_llm.with_structured_output(WikiSection)
```

## AgentBruno/storm.py

```diff
@@ -18,14 +18,15 @@
         self.pinecone_envo = pinecone_envo
         self.pinecone_index = pinecone_index
 
     
     async def write_storm_article(self):
         
         try:
+            print("In")
             builder_of_storm = StateGraph(ResearchState)
             
             
             nodes = [
                 ("init_research", initialize_research),
                 ("conduct_interviews", conduct_interviews),
                 ("refine_outline", refine_outline),
```

## Comparing `AgentBruno-0.0.3.dist-info/METADATA` & `AgentBruno-0.0.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: AgentBruno
-Version: 0.0.3
+Version: 0.0.4
 Summary: Description of your package
 Home-page: https://github.com/NinJagtap/AgentBruno.git
 Author: Ninad Jagtap
 Author-email: digitalforutility@gmail.com
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: langchain ==0.1.14
 Requires-Dist: langchain-community ==0.0.30
 Requires-Dist: langchain-openai ==0.1.1
 Requires-Dist: langgraph ==0.0.30
 Requires-Dist: pinecone-client ==2.2.4
-Requires-Dist: tavily-python ==0.3.3
 Requires-Dist: duckduckgo-search ==5.2.2
 Requires-Dist: wikipedia ==1.4.0
 Requires-Dist: scikit-learn ==1.4.1.post1
 Requires-Dist: streamlit ==1.32.0
 
 # Agent Bruno
```

## Comparing `AgentBruno-0.0.3.dist-info/RECORD` & `AgentBruno-0.0.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 AgentBruno/__init__.py,sha256=em44of2ylJKIbA-m9KYt95WtgqYO9TC00268MG3BqYA,285
-AgentBruno/research.py,sha256=ae4HuwfUxGQRZpryEC4CCKaEQuZhsp2Nf76DvrUDT_k,31667
-AgentBruno/storm.py,sha256=JdEYa3bbJfw7qXkV1VyO6Ouvk73GKaZijVbic-ugz_g,2405
-AgentBruno-0.0.3.dist-info/LICENSE,sha256=h8ov1i6ZptbvI_uWY3kQ6_GU84mnzfuSXc241x5IKDk,351
-AgentBruno-0.0.3.dist-info/METADATA,sha256=-aSTWScOR9pRCpVPwr-lyH_AZdU4D5T0itvs7vtBJ8M,10024
-AgentBruno-0.0.3.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-AgentBruno-0.0.3.dist-info/entry_points.txt,sha256=3FcKJzFRgu0kyLYB7ExjcHtPVlAVTZ4upTq_jbnknRo,72
-AgentBruno-0.0.3.dist-info/top_level.txt,sha256=pJKzwPOeRIEh-EE-rBvdQmY2YWk7rYuP0AGj1gAhRTo,11
-AgentBruno-0.0.3.dist-info/RECORD,,
+AgentBruno/research.py,sha256=c_XKdKLf_5WVeHTD0dEhJ9tC5b3FL9RKVsqfScV0t1U,32166
+AgentBruno/storm.py,sha256=GCs99vHeoo_6IaQU1yG_6BvbTZD_dMW0wH8L36rZSis,2429
+AgentBruno-0.0.4.dist-info/LICENSE,sha256=h8ov1i6ZptbvI_uWY3kQ6_GU84mnzfuSXc241x5IKDk,351
+AgentBruno-0.0.4.dist-info/METADATA,sha256=KB5SdnMzY-DEkdV4EjMUiMM0ZyyNkLq3IX0JOsKKfN8,9987
+AgentBruno-0.0.4.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+AgentBruno-0.0.4.dist-info/entry_points.txt,sha256=3FcKJzFRgu0kyLYB7ExjcHtPVlAVTZ4upTq_jbnknRo,72
+AgentBruno-0.0.4.dist-info/top_level.txt,sha256=pJKzwPOeRIEh-EE-rBvdQmY2YWk7rYuP0AGj1gAhRTo,11
+AgentBruno-0.0.4.dist-info/RECORD,,
```

