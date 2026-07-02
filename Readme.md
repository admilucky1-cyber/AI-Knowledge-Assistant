Here is the **exact, raw Markdown code** you can copy and paste directly into your `README.md` file. 

*(Note: I have put `your_groq_api_key_here` in the example. **Do not** paste your real API key in the README to keep it safe).*

---

```markdown
# AI Knowledge Assistant (RAG Chatbot)

An intelligent AI assistant that allows users to upload PDF and TXT files and ask questions about the content using Natural Language Processing (RAG - Retrieval-Augmented Generation). Built with Python, LangChain, and Groq LLM.

## 🚀 Features
- **Drag & Drop Upload:** Easily upload `.pdf` and `.txt` documents via a clean web interface.
- **AI-Powered Q&A:** Ask natural language questions about your uploaded documents.
- **Source Citations:** The AI tells you exactly which file it pulled the answer from.
- **Document Management:** View, delete, or clear all documents with a single click.

## 🛠️ Tech Stack
- **Backend:** Python, Flask, LangChain, Groq API, FAISS (Vector DB), HuggingFace Embeddings
- **Frontend:** HTML, CSS, JavaScript (Vanilla)
- **Data Science:** PyPDFLoader, RecursiveCharacterTextSplitter

## 📁 Project Structure
```
AI-Knowledge-Assistant/
├── backend/
│   ├── app.py                 # Main Flask application
│   ├── requirements.txt       # Python dependencies
│   ├── .env                   # Environment variables (API Keys)
│   └── uploads/               # Folder where uploaded PDFs/TXT files are stored
│
├── frontend/
│   └── index.html             # The user interface (UI)
│
├── .gitignore                 # Files to ignore on GitHub
└── README.md                  # This file
```

## ⚙️ Installation & Setup

Follow these steps to run the project locally on your computer:

### 1. Clone the Repository
```bash
git clone https://github.com/admilucky1-cyber/AI-Knowledge-Assistant.git
cd AI-Knowledge-Assistant
```

### 2. Set up a Virtual Environment (Recommended)
```bash
python -m venv venv

# Activate it (Windows):
.\venv\Scripts\activate

# Activate it (Mac/Linux):
source venv/bin/activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure Environment Variables (`.env`)
Create a file named `.env` in the `backend/` folder and paste your API key inside:

```env
GROQ_API_KEY=your_groq_api_key_here
```

### 5. Run the Application
Navigate to the backend folder and start the Flask server:

```bash
cd backend
python app.py
```
You will see:
`* Running on http://127.0.0.1:5001`

### 6. Open in Browser
Open your web browser and go to:
```
http://127.0.0.1:5001
```

## 📂 requirements.txt
Make sure your `requirements.txt` file inside the `backend` folder contains the following libraries:

```text
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

## 🤝 How to Use the AI
1. On the homepage, drag and drop a `.pdf` or `.txt` file into the upload zone.
2. Wait a few seconds for the AI to process the document.
3. Type a question into the chatbox and press Send.
4. The AI will answer based strictly on the content of the uploaded files!

## 📧 Contact
Created by **Aftab** ([@luckyman950](https://www.fiverr.com/luckyman950)). 

**Looking to hire?** I am available on Fiverr for custom AI Chatbot and Data Analytics projects!
```