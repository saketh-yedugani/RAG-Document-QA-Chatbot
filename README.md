# 📄 RAG Document Q&A with Groq & LLaMA 3.1

This project is a **Retrieval-Augmented Generation (RAG)** application that enables users to ask questions from research papers and receive accurate, context aware answers.

The app uses **FAISS vector search**, **OpenAI embeddings**, and **LLaMA 3.1 (via Groq)** for ultra fast inference, all wrapped in an interactive **Streamlit UI**.

---

## 🚀 Features

- 📂 Load and process multiple research papers (PDFs)
- ✂️ Chunk documents using RecursiveCharacterTextSplitter
- 🔍 Store embeddings in FAISS vector database
- 🤖 Query documents using LLaMA 3.1 via Groq
- ⚡ Low latency responses with Groq inference
- 📑 View document similarity results alongside answers

---

## 🧠 Architecture (RAG Pipeline)

1. PDF documents are loaded from a directory  
2. Documents are split into chunks  
3. OpenAI embeddings are generated  
4. FAISS stores vectors for similarity search  
5. Relevant chunks are retrieved  
6. LLaMA 3.1 generates answers **only from retrieved context**


