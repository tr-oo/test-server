## О проекте
Проект представляет собой простое веб-приложение, развернутое в Docker-контейнерах с Nginx в качестве reverse proxy.  
Backend — HTTP-сервер на Python, отвечающий текстом "Hello from Effective Mobile!".

---
## Стек технологий
- **Docker**, **Docker Compose**
- **Nginx**
- **Python 3.12**

---
## Структура проекта

**├── backend/  
│ ├── Dockerfile  
│ └── server.py   
├── nginx/  
│ └── nginx.conf   
├── docker-compose.yml  
└── README.md**

---

# Запуск
```bash
docker-compose up
```

# Проверка 
```bash
curl http://localhost
```

## Ожидаемый ответ: `Hello from Effective Mobile!`

Backend недоступен с хоста (порт 8080 закрыт):

```bash
curl http://localhost:8080
```
