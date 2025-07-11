# RTI Tracker & Response Summarizer

An AI-powered platform to help citizens track the status of their RTI (Right to Information) applications and summarize bulky RTI replies into key points.

---

## 🚀 Features

- **RTI Status Tracker:**
  - Enter RTI reference numbers to fetch status updates (mock API/data).
- **RTI Response Summarizer:**
  - Upload PDF or paste text RTI responses and get concise summaries using GPT (via LangChain).
- **Similar RTI Suggestions:**
  - Get suggestions for similar successful RTIs based on keywords or departments (semantic search with FAISS).
- **Open Data/Precedents:**
  - (Optional) Links to open government datasets or legal precedents based on department/keywords.

---

## 🛠️ Tech Stack

- **Backend:** Python, FastAPI, LangChain, OpenAI/GPT, FAISS, PyMuPDF
- **Frontend:** React (Create React App)
- **Other:** Mock data, PDF parsing, REST API

---

## ⚡ Quickstart

### 1. Backend

```bash
cd backend
python3 -m venv venv
source venv/bin/activate
pip install -r requirements.txt
uvicorn main:app --reload
```

### 2. Frontend

```bash
cd frontend
npm install
npm start
```

---

## 📂 Project Structure

```
Right-to-Information-RTI-Tracker-Response-Summarizer/
├── backend/
│   ├── main.py
│   ├── rti_status.py
│   ├── summarizer.py
│   ├── similarity.py
│   ├── pdf_utils.py
│   ├── data/
│   │   └── rti_samples.json
│   └── requirements.txt
└── frontend/
    ├── public/
    ├── src/
    └── package.json
```

---

## 📝 Usage

- **Track RTI:** Enter your RTI reference number to get the latest status.
- **Summarize Response:** Upload a PDF or paste the RTI reply text to get a summary.
- **Find Similar RTIs:** Get suggestions for similar successful RTIs.

---

## 🤖 AI & Data

- Summarization powered by OpenAI/GPT via LangChain.
- Semantic similarity search using FAISS.
- PDF parsing with PyMuPDF.
- Mock RTI data for demo/testing.

---

## 📄 License

MIT
