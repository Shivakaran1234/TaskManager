📌 AI-Driven Task Manager

An AI-powered task management application that helps users create, organize, and prioritize tasks intelligently using LLM-based assistance.
The project is designed with a scalable architecture and is being extended with DevOps best practices for production readiness.

🚀 Features

📝 Create, update, and delete tasks

🤖 AI-powered task suggestions and summaries

📊 Task prioritization using AI insights

⚡ Fast and responsive frontend

🔗 RESTful API backend

🧠 Integration with LLM (Groq API)

🛠 Tech Stack
Frontend

React (Vite + TypeScript)

Tailwind CSS

Backend

FastAPI (Python)

REST APIs

Uvicorn server

Database

SQLite (development)

AI Integration

Groq LLM API

🧱 Project Architecture (Current)
Frontend (React)
     |
     |  HTTP Requests
     v
Backend (FastAPI)
     |
     |  ORM / Queries
     v
Database (SQLite)
     |
     |  AI Requests
     v
Groq LLM API

📂 Project Structure
ai-taskmanager/
│
├── frontend/          # React frontend
│
├── backend/           # FastAPI backend
│   ├── main.py
│   ├── requirements.txt
│
├── README.md

⚙️ How to Run Locally
1️⃣ Clone the Repository
git clone https://github.com/<your-username>/ai-taskmanager.git
cd ai-taskmanager

2️⃣ Backend Setup
cd backend
python -m venv venv
source venv/bin/activate   # Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload


Backend runs at:

http://localhost:8000

3️⃣ Frontend Setup
cd frontend
npm install
npm run dev


Frontend runs at:

http://localhost:5173

🔐 Environment Variables

Create a .env file in the backend directory:

GROQ_API_KEY=your_api_key_here


⚠️ Never commit .env files to GitHub.

🧪 API Documentation

FastAPI Swagger UI available at:

http://localhost:8000/docs
