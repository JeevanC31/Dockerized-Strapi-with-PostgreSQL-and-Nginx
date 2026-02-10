# Dockerized Strapi with PostgreSQL and Nginx

##  Overview
This project demonstrates a Dockerized setup of a **Strapi application** using:
- **Node.js** (custom Strapi build)
- **PostgreSQL** as the database
- **Nginx** as a reverse proxy

All services run on a **user-defined Docker network** and are orchestrated using **Docker Compose**.

---

##  Architecture
```text
Browser (localhost:80)
        |
      Nginx
        |
     Strapi (1337)
        |
    PostgreSQL
```
## 📁 Project Structure
```text
day2/
├── my-strapi-app/ # Strapi application (Node-based)
│ ├── Dockerfile
│ ├── .env
│ ├── package.json
│ ├── config/
│ ├── src/
│ └── public/
│
├── nginx/
│ └── nginx.conf # Reverse proxy configuration
│
├── docker-compose.yml
└── README.md
```

## ⚙️ Prerequisites
- Docker
- Docker Compose

---

## 🚀 How to Run the Project

### 1️. Clone the Repository
```bash
git clone (https://github.com/JeevanC31/Dockerized-Strapi-with-PostgreSQL-and-Nginx)

2️. Build and Start Containers
docker compose build
docker compose up -d

3️. Verify Running Containers
docker ps

4️. Access Strapi Admin Dashboard

Open your browser and go to:

http://localhost/admin

```
