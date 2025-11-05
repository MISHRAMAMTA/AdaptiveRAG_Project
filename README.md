# AdaptiveRAG_Project
# Intelligent RAG Workflow using LangGraph, LangChain, and OpenAI

This project implements a **Retrieval-Augmented Generation (RAG)** system that dynamically routes queries, retrieves context from vector databases, detects hallucinations, and reformulates questions when necessary — all orchestrated through **LangGraph**.  

It integrates **LangChain**, **FAISS**, **OpenAI embeddings**, and **structured decision nodes** to build a complete autonomous reasoning loop.

---

## 🚀 Features

- **Dynamic Query Routing:**  
  Determines whether to use local vectorstore or perform a web search using a routing LLM.  

- **Document Relevance Grading:**  
  Filters out irrelevant documents retrieved from the FAISS vectorstore.  

- **Query Transformation:**  
  Automatically rewrites unclear queries to improve retrieval accuracy.  

- **Answer Generation:**  
  Uses a structured OpenAI LLM to synthesize context-grounded responses.  

- **Hallucination & Relevance Detection:**  
  Validates whether the generated answer is factually supported and relevant to the user query.  

- **Web Search Integration:**  
  Uses Tavily Search (or LangChain Tavily wrapper) when the local knowledge base doesn’t have relevant information.  
