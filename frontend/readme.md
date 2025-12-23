# Mini AI-Powered Notes Manager

This is a full-stack web application that allows users to create notes and search them using semantic similarity powered by AI embeddings.

## Tech Stack
- Backend: FastAPI (Python)
- Database: SQLite
- AI Model: sentence-transformers (all-MiniLM-L6-v2)
- Frontend: Vanilla JavaScript + HTML

## Features
- Create and store notes
- Generate embeddings for note content
- Semantic search using cosine similarity
- Simple frontend UI

## Setup Instructions

### Backend
```bash
cd backend/backend
python -m venv venv
venv\Scripts\activate
python -m pip install -r requirements.txt
python -m uvicorn main:app --reload
