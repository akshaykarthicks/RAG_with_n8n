# 🧠 Supabase RAG Agent  using n8n

This project implements a RAG (Retrieval-Augmented Generation) pipeline using [n8n](https://n8n.io/), integrated with OpenAI, Supabase, and PostgreSQL. It enables contextual AI chat with persistent memory and document search capabilities.

## 📦 Features

- 🧠 **RAG Agent** powered by OpenAI's GPT model
- 💾 **Postgres-backed chat memory** for context retention
- 📚 **Supabase vector store** for embedding search
- 📂 **Google Drive integration** to load documents
- 🧩 **LangChain nodes** for document parsing and splitting
- 🔄 **Automated embedding + indexing pipeline**

## 🛠️ Components

- **OpenAI Chat Model:** Handles user interaction via GPT-4o-mini
- **Postgres Memory:** Stores past messages for contextual understanding
- **Supabase Vector Store:** Enables semantic search with embedded documents
- **Document Loader & Splitter:** Parses binary data, splits text for embedding
- **Google Drive Node:** Automatically pulls documents from Drive

## 🚀 Workflow Overview

![Screenshot 2025-06-05 194059](https://github.com/user-attachments/assets/052071d4-02af-413f-bb66-a2a23510020e)
![image](https://github.com/user-attachments/assets/ef8f2c33-0917-406c-a5fc-d040d9ca986e)



1. Trigger: Chat message or manual trigger
2. RAG Agent uses OpenAI + Postgres Memory + Supabase Vector Search
3. Binary files from Drive are loaded, split, embedded
4. Embeddings stored in Supabase for retrieval
5. Answers are returned with contextual + factual relevance

## 📂 How to Use

1. Download the workflow and auth it .
2. Connect credentials for:
   - Google Drive
   - OpenAI
   - Supabase
   - Postgres
3. Upload documents to the specified Drive folder.
4. Trigger the workflow using chat or manual test.
5. Enjoy your intelligent assistant with memory and vector search!



