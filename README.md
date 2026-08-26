# 🎓 AI Exam Preparation Assistant

An intelligent study assistant powered by **OpenAI Agents**, **FastAPI**, and **React**. Upload study materials, generate practice questions, create flashcards, and interact with your personal AI study tutor.

---

## ✨ Features

- 🧠 **AI-Powered Study Agent**: Interacts with your documents using OpenAI Agents & ChatKit.
- 📚 **Vector Store Knowledge Retrieval**: Automatically indexes and searches through uploaded study documents.
- 🟢 **Live API Monitoring & Health Check**: Includes a custom `GET /health` endpoint and a live pulsing status badge on the frontend header to ensure real-time backend connection status.
- 🎨 **Modern React UI**: Sleek, accessible interface with document previews and ChatKit integration.

---

## 🏗️ Architecture Overview

- **Backend**: Python 3.11+, FastAPI, OpenAI Agents SDK, Logfire, Uvicorn.
- **Frontend**: React 18, Vite, Tailwind CSS, ChatKit Web Component.

---

## 🚀 Quick Start Guide

### Prerequisites
- **Python**: 3.11+
- **Node.js**: 20+ / 22+

---

### 1. Environment Setup

Copy `.env.template` to `.env`:

```bash
cp .env.template .env
```

Ensure `.env` contains your configuration:
```env
OPENAI_API_KEY=your_openai_api_key
EXAM_PREP_VECTOR_STORE_ID=vs_your_vector_store_id
NOTION_TOKEN=your_notion_token
```

---

### 2. Start the FastAPI Backend

From the repository root:

```bash
cd backend
python -m pip install -e .
python -m uvicorn app.main:app --reload
```

> **Health Check Verification**: Open [http://127.0.0.1:8000/health](http://127.0.0.1:8000/health) in your browser to verify API status (`{"status": "ok"}`).

---

### 3. Start the React Frontend

In a new terminal:

```bash
cd frontend
npm install
npm run dev
```

Open [http://localhost:5172](http://localhost:5172) in your browser. Look for the **`🟢 API Connected`** badge in the header!

---

## 📄 License

This project is open source and licensed under the [GNU General Public License v3.0](LICENSE).
