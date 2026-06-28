# 📚 AI Knowledge Assistant (RAG Chatbot)

## 📖 Overview

AI Knowledge Assistant is a Retrieval-Augmented Generation (RAG) chatbot that answers questions from PDF documents using semantic search and Large Language Models (LLMs).

The application extracts text from PDF files, splits it into chunks, generates OpenAI embeddings, stores them in **Qdrant**, and retrieves the most relevant context before generating accurate responses.

---

## ✨ Features

* 📄 PDF document ingestion
* ✂️ Intelligent document chunking
* 🔍 Semantic similarity search
* 🧠 OpenAI embedding generation
* 💬 Context-aware question answering
* ⚡ Fast retrieval using Qdrant
* 🐳 Dockerized vector database

---

## 🛠 Tech Stack

| Category         | Technologies           |
| ---------------- | ---------------------- |
| Language         | Python                 |
| AI Framework     | LangChain              |
| LLM              | OpenAI GPT             |
| Embeddings       | text-embedding-3-large |
| Vector Database  | Qdrant                 |
| PDF Loader       | PyPDF                  |
| Containerization | Docker                 |

---

## 🏗 RAG Pipeline

```text
PDF
 │
 ▼
Load Document
 │
 ▼
Split into Chunks
 │
 ▼
Generate OpenAI Embeddings
 │
 ▼
Store in Qdrant
 │
 ▼
User Question
 │
 ▼
Semantic Search
 │
 ▼
Relevant Chunks
 │
 ▼
OpenAI GPT
 │
 ▼
Answer
```

---

## 📂 Project Structure

```text
genai-rag-chatbot/
│── chat.py
│── index.py
│── nodejs.pdf
│── docker-compose.yml
│── requirements.txt
│── .env.example
│── README.md
```

---

## ⚙️ Installation

### Clone the repository

```bash
git clone https://github.com/Harsh-code-dev/genai-rag-chatbot.git
cd genai-rag-chatbot
```

### Create a virtual environment

```bash
python -m venv venv
```

### Activate the environment (Windows)

```bash
venv\Scripts\activate
```

### Install dependencies

```bash
pip install -r requirements.txt
```

### Configure environment variables

Create a `.env` file.

```env
OPENAI_API_KEY=your_openai_api_key
```

### Start Qdrant

```bash
docker compose up -d
```

### Index the PDF

```bash
python index.py
```

### Start chatting

```bash
python chat.py
```

---

## 🚀 Future Improvements

* Support multiple PDF documents
* Chat history
* Web interface
* Streaming responses
* Citation support
* Conversation memory

---

## 👨‍💻 Author

**Harsh Kumar**

GitHub: https://github.com/Harsh-code-dev
