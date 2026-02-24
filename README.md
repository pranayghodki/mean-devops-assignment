# 🚀 MEAN Stack CRUD Application – DevOps Deployment

This project demonstrates a full-stack CRUD application built using the **MEAN stack** and fully containerized using **Docker & Docker Compose**.

---

## 🛠 Tech Stack

- MongoDB
- Express.js
- Angular 15
- Node.js
- Docker
- Docker Compose
- Nginx

---

## 📦 Application Features

- Create Tutorial
- Retrieve Tutorials
- Update Tutorial
- Delete Tutorial
- Search by Title
- Published Status Toggle

Each tutorial contains:
- id
- title
- description
- published

---

## 🏗 Architecture

```
User (Browser)
      ↓
Nginx (Frontend Container)
      ↓
Node.js + Express (Backend Container)
      ↓
MongoDB (Database Container)
```

---

## 📁 Project Structure

```
crud-dd-task-mean-app/
│
├── backend/
│   ├── Dockerfile
│   └── app/
│
├── frontend/
│   ├── Dockerfile
│   ├── nginx.conf
│
├── docker-compose.yml
└── README.md
```

---

# 🐳 Run Using Docker Compose (Recommended)

## 1️⃣ Build and Start Containers

```bash
docker compose up --build
```

## 2️⃣ Access Application

Frontend:
```
http://localhost
```

Backend API:
```
http://localhost:8080/api/tutorials
```

---

# 🛑 Stop Containers

```bash
docker compose down
```

---

# ⚙ Backend Runs On

- Port: 8080
- Database: MongoDB (Containerized)
- Environment: Docker Network

---

# ⚙ Frontend Runs On

- Served using Nginx
- Port: 80
- Built using Angular Production Build

---

# 📡 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/tutorials | Get all tutorials |
| GET | /api/tutorials/:id | Get tutorial by ID |
| POST | /api/tutorials | Create tutorial |
| PUT | /api/tutorials/:id | Update tutorial |
| DELETE | /api/tutorials/:id | Delete tutorial |

---

# 💡 DevOps Highlights

- Multi-container architecture
- Dockerized backend & frontend
- Custom Docker network
- Production-ready Angular build
- Nginx reverse serving
- MongoDB containerized
- Fully reproducible environment using docker-compose

---

## 📸 Deployment Screenshots

### ✅ 1. GitHub Actions – CI/CD Success
![CI/CD Success](screenshots/ci-cd-success.png)

### 🐳 2. Docker Hub Images
![Docker Hub](screenshots/docker-hub.png)

### ☁️ 3. AWS EC2 Instance Running
![EC2](screenshots/ec2-instance.png)

### 🚀 4. Application Running on EC2
![App Running](screenshots/app-running.png)

### 🖥 5. Docker Containers Running on Server
![Docker PS](screenshots/docker-ps.png)
# 👨‍💻 Author

Pranay Ghodki  
DevOps & Cloud Enthusiast 🚀

---

# 📌 Conclusion

This project demonstrates containerization, networking, service orchestration, and production-ready deployment of a full-stack MEAN application using Docker.
