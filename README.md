# Exam Preparation Agent Workshop

## What's Inside
- FastAPI service that is backed by OpenAI Agents.
- ChatKit Web Component wrapped in React with a document panel.
- Vector-store tooling for ingesting documents and exposing REST endpoints for previews, uploads.
- **Health Check API**: `GET /health` endpoint for monitoring backend uptime.
- **Live Status Indicator**: Pulse status badge on the frontend header reflecting real-time API connectivity.

## Prerequisites
- Python 3.11+
- Node.js 22+
- OpenAI API key as `OPENAI_API_KEY` in `.env`

## Steps to Run:

### 1. Setup Environment
Copy template into `.env`:
```cmd
copy .env.template .env
```

### 2. Start the FastAPI Backend
```cmd
cd backend
python -m pip install -e .
python -m uvicorn app.main:app --reload
```

### 3. Start the React Frontend
In a new terminal window:
```cmd
cd frontend
npm install
npm run dev
```
