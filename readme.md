# 🚀 Ares — Dockerized Full-Stack Application

![Docker](https://img.shields.io/badge/Docker-Containerized-blue?logo=docker)
![Node.js](https://img.shields.io/badge/Frontend-Node.js-green?logo=node.js)
![Flask](https://img.shields.io/badge/Backend-Flask-lightgrey?logo=flask)
![Status](https://img.shields.io/badge/Status-Working-success)

Ares is a **full-stack application** built with **Flask (backend)** and **Node.js (frontend)**, fully containerized using **Docker** and orchestrated via **Docker Compose**.

It demonstrates **multi-container architecture**, **service-to-service communication**, and **clean development workflow using containers**.

---

## 📌 Features

* 🧩 Multi-container setup (Frontend + Backend)
* 🔗 Seamless API communication using Docker networking
* ⚡ Fast development with volume mounting
* 🐳 Fully Dockerized (no local dependency conflicts)
* 🛠 Easy to scale and extend

---

## 🛠 Tech Stack

| Layer    | Technology             |
| -------- | ---------------------- |
| Frontend | Node.js                |
| Backend  | Flask (Python)         |
| DevOps   | Docker, Docker Compose |

---

## 📂 Project Structure

```bash
ares/
│
├── backend/
│   ├── app.py
│   ├── business.py
│   ├── requirements.txt
│   └── Dockerfile
│
├── frontend/
│   ├── app.js
│   ├── package.json
│   └── Dockerfile
│
├── docker-compose.yaml
├── .gitignore
├── .dockerignore
└── README.md
```

---

## ⚙️ How It Works

* Backend runs on **port 5000**
* Frontend runs on **port 3000**
* Frontend communicates with backend using:

  ```
  http://backend:5000/api
  ```
* Docker Compose creates a **shared network**, allowing services to communicate

---

## 🐳 Getting Started

### 🔹 Prerequisites

* Docker installed
* Docker Compose installed

---

### 🔹 Run the Application

```bash
docker-compose up 
```

---

### 🔹 Access the App   

| Service  | URL                       |
| -------- | ------------------------- |
| Frontend | http://localhost:3000     |
| Backend  | http://localhost:5000/api |

---

## 🔁 API Example

### Request:

```bash
GET /api
```

### Response:

```json
{
  "data": ["Zeus", "Kratos", "Thor", "Loki", "Odin", "Hela", "Artemis", "Aries"]
}
```

---

## 🧠 Key Learnings

* Writing Dockerfiles for different services
* Managing multi-container apps with Docker Compose
* Internal container networking (service-based DNS)
* Debugging real-world Docker issues
* Using `.dockerignore` and `.gitignore` effectively

---

## ⚠️ Important Notes

* Flask is running in **development mode** (not suitable for production)

---

## 🚀 Future Improvements

* 🔁 Add NGINX reverse proxy
* ⚙️ Use Gunicorn for production backend
* 🗄 Integrate database (MongoDB / MySQL)
* 🔐 Add authentication & authorization
* 🌱 Use `.env` for environment configs

---

## 👨‍💻 Author

**Anuj Singh Bhadouriya**


