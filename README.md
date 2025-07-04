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

- http://3.95.38.228:8080/service1/hello
- http://3.95.38.228:8080/service1/ping
- http://3.95.38.228:8080/service2/hello
- http://3.95.38.228:8080/service2/ping

## 🩺 Health Checks

Both services have `/ping` endpoints used by Docker for health checking.

![image](https://github.com/user-attachments/assets/5e908690-53a3-4309-8dbc-133b72d17b64)

## 📜 Logging


![image](https://github.com/user-attachments/assets/03c6b4f7-82b0-4c3e-9b3a-c5f0b3df9753)
