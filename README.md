# AI Knowledge Assistant

> Upload PDFs & TXT files and ask natural-language questions. Powered by LangChain + Groq + FAISS.

[![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)](https://python.org)
[![LangChain](https://img.shields.io/badge/LangChain-0.1%2B-green)](https://langchain.com)
[![Groq](https://img.shields.io/badge/LLM-Groq-f55036)](https://groq.com)
[![License](https://img.shields.io/badge/License-Apache%202.0-orange)](LICENSE)

---

## Features

- **Drag & drop upload** — PDF and TXT
- **RAG Q&A** — Answers grounded strictly in your documents
- **Source citations** — Know which file the answer came from
- **Document management** — View, delete, or clear all
- **Clean UI** — Vanilla HTML/CSS/JS frontend

---

## Tech Stack

| Layer | Stack |
|-------|-------|
| Backend | Python · Flask · LangChain · Groq · FAISS · HuggingFace embeddings |
| Frontend | HTML · CSS · JavaScript |
| Loaders | PyPDFLoader · RecursiveCharacterTextSplitter |

---

## Project Structure

```
AI-Knowledge-Assistant/
├── backend/
│   ├── app.py              # Flask application
│   ├── requirements.txt
│   ├── test.py
│   └── uploads/            # Uploaded documents (gitignored)
├── frontend/
│   └── index.html          # User interface
├── .env.example            # Template for secrets
├── .gitignore
├── LICENSE
└── README.md
```

---

## Quick Start

```bash
git clone https://github.com/admilucky1-cyber/AI-Knowledge-Assistant.git
cd AI-Knowledge-Assistant

python -m venv venv
# Windows: .\venv\Scripts\activate
# macOS/Linux: source venv/bin/activate

pip install -r backend/requirements.txt

cp .env.example backend/.env
# Edit backend/.env and add your GROQ_API_KEY

cd backend
python app.py
```

Open **http://127.0.0.1:5001**

---

## Environment

Create `backend/.env`:

```env
GROQ_API_KEY=your_groq_api_key_here
```

Get a free key at [console.groq.com](https://console.groq.com).

---

## How to Use

1. Drag & drop a `.pdf` or `.txt` file
2. Wait for indexing
3. Ask a question in the chat
4. Receive an answer grounded in the uploaded content

---

## Requirements

```
flask
flask-cors
python-dotenv
werkzeug
langchain-community
langchain-groq
faiss-cpu
pypdf
sentence-transformers
```

---

## License

Apache License 2.0 — see [LICENSE](LICENSE)

---

**Built for learning and production RAG demos.**
