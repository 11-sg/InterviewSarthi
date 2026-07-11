# InterviewSarthi

> **From Resume to Offer Letter.**

InterviewSarthi is a full-stack AI-powered web application that helps job seekers analyze their resumes against a target job description, receive an AI-generated profile match score, identify skill gaps, and prepare for interviews with personalized technical and behavioral questions. It also generates a structured preparation roadmap to help candidates improve before their interviews.

---

## 🌐 Live Demo

**Frontend:**  
https://interviewsarthi-1.onrender.com

**Backend:**  
https://interviewsarthi.onrender.com

---

# Features

- 🔐 Secure User Authentication (Register/Login)
- 🍪 JWT Authentication using HTTP-Only Cookies
- 📄 Resume Upload (PDF)
- 💼 Job Description Analysis
- 📝 Optional Self Description
- 🤖 AI-powered Resume Evaluation using Google Gemini
- 📊 Resume Match Score (0–100)
- 💡 Skill Gap Identification
- 🎯 Personalized Technical Interview Questions
- 💬 Personalized Behavioral Interview Questions
- 📅 AI-generated Day-wise Preparation Roadmap
- 📂 Save and View Previous Interview Reports
- 📥 Download AI-Generated Resume PDF
- 📱 Responsive Modern UI

---

# 🛠️ Tech Stack

## Frontend
- React.js
- Vite
- Axios
- React Router DOM

## Backend
- Node.js
- Express.js
- MongoDB Atlas
- Mongoose
- JWT Authentication
- Cookie Parser
- Multer
- PDF Parser

## AI
- Google Gemini API

## Deployment
- Render
- MongoDB Atlas

---

# 📂 Project Structure

```
InterviewSarthi
│
├── interview-ai
│   ├── Frontend
│   │   ├── src
│   │   ├── public
│   │   └── package.json
│   │
│   └── Backend
│       ├── src
│       ├── server.js
│       └── package.json
│
└── README.md
```

---

# ⚙️ Installation

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/11-sg/InterviewSarthi.git
```

---

## 2️⃣ Backend Setup

```bash
cd interview-ai/Backend
npm install
```

Create a `.env` file inside the Backend folder:

Run the backend:

```bash
npm start
```

---

## 3️⃣ Frontend Setup

```bash
cd interview-ai/Frontend
npm install
```

Create a `.env` file inside the Frontend folder:

```env
VITE_API_URL=http://localhost:3000
```

Run the frontend:

```bash
npm run dev
```

---

# 🔄 Application Workflow

```
User Login/Register
        │
        ▼
Upload Resume (PDF)
        │
        ▼
Enter Job Description
        │
        ▼
(Optional) Self Description
        │
        ▼
Resume Parsing
        │
        ▼
Google Gemini AI Analysis
        │
        ▼
──────────────────────────────
✔ Match Score
✔ Technical Questions
✔ Behavioral Questions
✔ Skill Gap Analysis
✔ Preparation Roadmap
──────────────────────────────
        │
        ▼
Save Report to MongoDB
        │
        ▼
View Previous Reports
        │
        ▼
Download AI Resume PDF
```


# 🔐 Authentication

- JWT Authentication
- HTTP-Only Secure Cookies
- Protected Routes
- Cookie-based Session Management
- Token Blacklisting on Logout

---

# 📌 API Endpoints

## Authentication

| Method | Endpoint |
|----------|----------------------------|
| POST | `/api/auth/register` |
| POST | `/api/auth/login` |
| GET | `/api/auth/logout` |
| GET | `/api/auth/get-me` |

---

## Interview

| Method | Endpoint |
|----------|------------------------------------------|
| POST | `/api/interview` |
| GET | `/api/interview` |
| GET | `/api/interview/report/:interviewId` |
| POST | `/api/interview/resume/pdf/:interviewId` |

---

---
