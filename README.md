# AI MEDICAL CHATBOT USING IMAGE ANALYSIS

An AI-powered medical image analysis web application that allows users to upload medical images and ask questions in natural language. The application uses **FastAPI** as the backend and integrates with **Groq's Llama 3.2 Vision Model** to provide intelligent image analysis and conversational responses.

> ⚠️ **Disclaimer:** This project is for educational and research purposes only. It should not be used as a substitute for professional medical advice or diagnosis.

---

## 📌 Features

- Upload medical images (X-rays, skin images, reports, etc.)
- AI-powered image analysis using Llama 3.2 Vision
- Interactive chatbot interface
- Fast and lightweight FastAPI backend
- REST API integration with Groq Cloud
- Image validation before processing
- Error handling and user-friendly responses
- Responsive web interface

---

## 🛠️ Tech Stack

### Frontend
- HTML5
- CSS3
- JavaScript

### Backend
- FastAPI
- Uvicorn
- Python

### AI Model
- Groq API
- Llama 3.2 Vision

### Libraries
- Requests
- Pillow (PIL)
- Python Dotenv
- JSON
- Base64

---

## 📂 Project Structure

```
AI_DOCTOR/
│
├── app.py                 # FastAPI Backend
├── requirements.txt
├── .env
├── templates/
│     └── index.html
├── static/
│     ├── css/
│     ├── js/
│     └── images/
├── README.md
└── screenshots/
```

---

## 🚀 How It Works

1. User uploads a medical image.
2. The image is validated using Pillow.
3. The image is converted into Base64 format.
4. FastAPI sends the image and user prompt to the Groq API.
5. Llama 3.2 Vision analyzes the image.
6. The AI-generated response is returned to the frontend.
7. The result is displayed in a chatbot interface.

---

## 🏗️ System Architecture

```
                User
                  │
                  ▼
          Upload Medical Image
                  │
                  ▼
           HTML / JavaScript
                  │
                  ▼
              FastAPI
                  │
                  ▼
          Image Validation
                  │
                  ▼
          Convert to Base64
                  │
                  ▼
             Groq API
                  │
                  ▼
      Llama 3.2 Vision Model
                  │
                  ▼
          AI Generated Response
                  │
                  ▼
             Web Interface
```

---

## ⚙️ Installation

### Clone Repository

```bash
git clone https://github.com/adarshramt/AI_DOCTOR.git
cd AI_DOCTOR
```

### Create Virtual Environment

```bash
python -m venv venv
```

Activate Environment

Windows

```bash
venv\Scripts\activate
```

Linux / Mac

```bash
source venv/bin/activate
```

### Install Dependencies

```bash
pip install -r requirements.txt
```

---

## 🔑 Environment Variables

Create a `.env` file.

```env
GROQ_API_KEY=your_groq_api_key
```

---

## ▶️ Run Application

```bash
uvicorn app:app --reload
```

Open your browser

```
http://127.0.0.1:8000
```

---

## 📌 API Workflow

```
User Request
      │
      ▼
FastAPI Endpoint
      │
      ▼
Validate Image
      │
      ▼
Encode Image (Base64)
      │
      ▼
Groq Vision API
      │
      ▼
AI Response
      │
      ▼
Frontend
```

---

## 💡 Challenges Faced

- Handling image uploads securely
- Validating different image formats
- Integrating external AI APIs
- Parsing AI responses
- Managing API errors gracefully

---

## 🚀 Future Improvements

- User authentication
- Chat history storage
- PDF medical report generation
- Docker deployment
- Cloud deployment (Render/AWS)
- Multi-language support
- Voice input support
- Medical report summarization
- Multiple AI model support

---

## 📚 Skills Demonstrated

- Python
- FastAPI
- REST APIs
- API Integration
- Computer Vision
- Generative AI
- Prompt Engineering
- Backend Development
- Image Processing
- JSON
- Base64 Encoding
- Uvicorn
- Git & GitHub

---


---

## 📈 Future Scope

- Integrate Electronic Health Records (EHR)
- Deploy using Docker & Kubernetes
- Add authentication & authorization
- Improve response accuracy using Retrieval-Augmented Generation (RAG)
- Fine-tune open-source medical vision models

---

## 👨‍💻 Author

**Adarsh Tripathi**

B.Tech (Artificial Intelligence & Machine Learning)

GitHub: https://github.com/adarshtramt

LinkedIn: https://linkedin.com/in/adarsh
---

## ⭐ If you found this project useful, please consider giving it a Star!
