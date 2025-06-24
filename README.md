# 🔁 Nginx Reverse Proxy + Docker Compose

This project sets up two microservices (Golang & Python) behind an Nginx reverse proxy using Docker Compose.

## 🧱 Project Structure

```
.
├── docker-compose.yml
├── nginx/
│   ├── nginx.conf
│   └── Dockerfile
├── service_1/ (Golang)
├── service_2/ (Python Flask)
```

## 🚀 How to Run

```bash
docker-compose up --build
```

## 🌐 Access

- http://localhost:8080/service1/hello
- http://localhost:8080/service2/hello

## 🩺 Health Checks

Both services have `/ping` endpoints used by Docker for health checking.

## 📜 Logging

Nginx logs all requests with timestamp and path.
