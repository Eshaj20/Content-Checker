# 📚 Content Checker - Full Stack Application

![FastAPI](https://img.shields.io/badge/FastAPI-005571?logo=fastapi)
![React](https://img.shields.io/badge/React-20232A?logo=react)
![Python](https://img.shields.io/badge/Python-3.9+-blue)
![Node.js](https://img.shields.io/badge/Node.js-14.x-green)

A complete text analysis platform with AI-powered grammar checking, plagiarism detection, and content moderation.

## 🌟 Features

### Backend Services
✅ Grammar error detection  
✅ Plagiarism similarity scoring  
✅ Fact verification engine  
✅ Content moderation system  
✅ RESTful API endpoints  

### Frontend Features
📝 Interactive text editor  
📊 Real-time analysis dashboard  
📑 Multi-format report generation  
🎨 Responsive Material-UI design  

## 🛠 Tech Stack

| Layer          | Technologies                          |
|----------------|---------------------------------------|
| **Frontend**   | React, Material-UI, Chart.js          |
| **Backend**    | FastAPI, Python, spaCy, Scikit-learn  |
| **Build Tools**| Vite, npm                             |
| **Deployment** | Docker, Nginx (optional)              |

## 🚀 Quick Start

### 1. Frontend Setup
                             cd frontend
                             npm install
                             npm run dev


### 2. Backend Setup

                            cd backend
                            python -m venv venv
                            source venv/bin/activate  # Linux/Mac
                            venv\Scripts\activate     # Windows

                            pip install -r requirements.txt
                            python -m spacy download en_core_web_sm
                            # Backend (http://localhost:8000)
                            uvicorn main:app --reload
                            # Frontend (http://localhost:3000)
                            npm run dev
                          
Production :                docker-compose up --build -d

📂 Project Structure

```bash
content-checker/
├── backend/
│   ├── models/          # NLP models
│   ├── routes/          # API endpoints
│   ├── main.py          # FastAPI app
│   └── requirements.txt
├── frontend/
│   ├── public/          # Static assets
│   ├── src/
│   │   ├── components/  # React components
│   │   ├── pages/       # Application views
│   │   ├── services/    # API clients
│   │   └── App.js       # Root component
│   └── package.json
└── README.md

