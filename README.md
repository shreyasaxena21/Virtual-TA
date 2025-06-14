# 🤖 Virtual Teaching Assistant

A smart assistant designed to help students and educators navigate course-related discussions and content. This project processes discussion forum threads, converts them into a structured format, embeds the knowledge, and serves an intelligent API for answering questions.

---

## 📁 Project Structure

```
Virtual TA/
│
├── pycache/ # Python cache files
├── downloaded_threads/ # Raw downloaded threads from discourse/forum
├── markdown_files/ # Cleaned and formatted markdown files
├── venv/ # Python virtual environment
│
├── .env # Environment variables (API keys, etc.)
├── .gitignore # Git ignored files
├── app.py # Main FastAPI app serving Q&A API
├── knowledge_base.db # SQLite database for stored embeddings or content
├── LICENSE # Project license
├── preprocess.py # Script for processing and cleaning thread content
├── README.md # Project documentation (this file)
├── requirements.txt # Python dependencies
└── vercel.json # Vercel deployment configuration
```


---

## ⚙️ Features

- ✅ Scrapes and parses discussion threads
- ✅ Cleans and stores content in markdown and DB
- ✅ Embeds content using LLM-based vector representation
- ✅ Serves a **POST API** to ask contextual questions
- ✅ Deployable to **Vercel** using `vercel.json`

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/shreyasaxena21/Virtual-TA
cd Virtual-TA
```
### 2. Install dependencies
```bash
pip install -r requirements.txt

```

### 3. Set up environment variables
Create a .env file in the root directory:

```bash
OPENAI_API_KEY=your_openai_key
```
### 4. Run the app
```bash
uvicorn app:app --reload
```











