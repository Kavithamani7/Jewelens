# JeweLens

JeweLens is a multimodal jewellery retrieval system that allows users to search for jewellery using text, images, or voice. The application combines computer vision, semantic search, and large language models to provide relevant jewellery recommendations through a unified interface.

## Features

- Text-based jewellery search using natural language
- Image-based retrieval using CLIP embeddings
- Voice search with speech recognition
- AI-assisted responses powered by Gemini
- FastAPI backend with React frontend
- Configurable deployment using environment variables

---

## Tech Stack

### Frontend
- React
- Vite
- JavaScript

### Backend
- FastAPI
- Python
- Uvicorn

### AI & Retrieval
- OpenAI CLIP
- FAISS
- Google Gemini API

---

## Project Structure

```
Jewelens/
├── backend/          # FastAPI backend
├── frontend/         # React application
├── Jewelry_RAG/      # Retrieval pipeline and vector indices
├── .gitignore
├── .env.example
└── README.md
```

---

## Getting Started

### Clone the repository

```bash
git clone https://github.com/Kavithamani7/Jewelens.git
cd Jewelens
```

### Backend

```bash
cd backend

python -m venv venv

# Windows
venv\Scripts\activate

# Linux/macOS
source venv/bin/activate

pip install -r requirements.txt
```

Create a `.env` file inside the `backend` directory.

```env
GEMINI_API_KEY=YOUR_API_KEY
ALLOWED_ORIGINS=http://localhost:5173
```

Start the backend:

```bash
uvicorn main:app --reload
```

---

### Frontend

```bash
cd frontend

npm install
```

Create a `.env` file inside the `frontend` directory.

```env
VITE_API_URL=http://localhost:8000
```

Run the development server:

```bash
npm run dev
```

---

## Deployment

The application is configured for deployment using environment variables.

### Backend

```
GEMINI_API_KEY=<your-api-key>
ALLOWED_ORIGINS=<frontend-url>
```

### Frontend

```
VITE_API_URL=<backend-url>
```

The backend can be deployed on Render, while the frontend can be deployed on Vercel without modifying the source code.

---

## Screenshots

Screenshots of the application can be added here.

- Home page
- Text search
- Image search
- Voice search
- Search results

---

## Future Improvements

- User authentication
- Personalized recommendations
- Additional retrieval models
- Performance optimization
- Expanded jewellery dataset

---

## Author

**Kavithamani P.**
