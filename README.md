# Face Recognition Authentication System

A full-stack face recognition application that uses facial biometrics for secure user authentication and authorization. The system verifies a user's identity by recognizing their face and grants access to protected features without relying solely on traditional passwords.

## 📌 Overview

This project demonstrates how face recognition can be integrated into a modern web application for secure authentication. Users register their facial data once, and subsequent logins are performed by verifying their face against the stored facial embeddings.

The application consists of a frontend for user interaction and a backend that handles face detection, recognition, authentication, and authorization.

## ✨ Features

* User registration
* Face enrollment during registration
* Face recognition login
* Secure authentication
* Authorization for protected resources
* User profile management
* RESTful API
* Responsive frontend
* Database integration
* Error handling and validation

## 🛠️ Tech Stack

### Frontend

* Next.js
* React
* TypeScript
* Tailwind CSS

### Backend

* FastAPI
* Python
* SQLAlchemy
* PostgreSQL (or SQLite for development)

### Face Recognition

* OpenCV
* face_recognition
* NumPy

## 📂 Project Structure

```text
Face-Recognition/
│
├── frontend/                 # Next.js frontend
│
├── backend/
│   ├── app/
│   │   ├── routes/
│   │   ├── services/
│   │   ├── models.py
│   │   ├── schemas.py
│   │   ├── database.py
│   │   └── main.py
│   │
│   ├── requirements.txt
│   └── .env
│
├── .gitignore
├── README.md
└── LICENSE
```

## 🚀 Getting Started

### Clone the repository

```bash
git clone https://github.com/Biren26/Face-Recognition.git
cd Face-Recognition
```

### Backend Setup

```bash
cd backend

python -m venv .venv
```

Activate the virtual environment.

**Windows**

```bash
.venv\Scripts\activate
```

Install dependencies.

```bash
pip install -r requirements.txt
```

Run the FastAPI server.

```bash
uvicorn app.main:app --reload
```

The backend will be available at:

```
http://127.0.0.1:8000
```

Swagger documentation:

```
http://127.0.0.1:8000/docs
```

### Frontend Setup

```bash
cd frontend

npm install

npm run dev
```

or

```bash
pnpm install
pnpm dev
```

The frontend will be available at:

```
http://localhost:3000
```

## 📖 Workflow

1. Register a new user.
2. Capture and store the user's facial data.
3. Extract facial embeddings.
4. Store facial embeddings securely in the database.
5. During login, capture a live image.
6. Compare the captured face with stored embeddings.
7. Authenticate the user if a match is found.
8. Grant access to authorized resources.

## 🔐 Security Considerations

* Passwords should be hashed before storage.
* Facial embeddings should be stored securely.
* Authentication tokens should be used for session management.
* HTTPS should be enabled in production.
* Input validation should be performed on all API requests.

## 📌 Future Improvements

* Liveness detection to prevent spoofing
* Multi-factor authentication (MFA)
* JWT-based authentication
* Role-Based Access Control (RBAC)
* Email verification
* Password recovery
* Face recognition confidence threshold tuning
* Audit logging
* Docker deployment
* CI/CD pipeline
* Cloud storage integration

## 🤝 Contributing

Contributions are welcome.

1. Fork the repository.
2. Create a feature branch.
3. Commit your changes.
4. Push the branch.
5. Open a Pull Request.

## 📄 License

This project is intended for educational and learning purposes.
