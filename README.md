# Study Buddy — Starter

## Prereqs
- Docker & Docker Compose OR
- Python 3.11+, Node 18+

## Quick dev (local, without Docker)
1. Backend:
   - cd backend
   - copy `.env.example` -> `.env` and set `OPENAI_API_KEY`
   - python -m venv venv
   - source venv/bin/activate
   - pip install -r requirements.txt
   - uvicorn app.main:app --reload --port 8000

2. Frontend:
   - cd frontend
   - copy `.env.example` -> `.env`
   - npm install
   - npm run dev

Open `http://localhost:5173`.

## Quick with Docker
- Copy backend/.env.example and set OPENAI_API_KEY (or pass env in another secure way)
- docker-compose up --build
- Visit http://localhost:5173
