# 🚀 next-fastapi-starter

<p align="right">
  <a href="#english">English</a> | 
  <a href="#中文">中文</a>
</p>

---

## 中文

### ✨ 项目特点

* ⚡ 前端：Next.js（App Router）
* 🐍 后端：FastAPI
* 🗄️ 数据库：PostgreSQL
* 🐳 Docker Compose 一键启动
* 🔄 支持热更新
* 🧱 适合快速开发 MVP

---

### 📁 项目结构

```
.
├── api/          # FastAPI 后端
├── web/          # Next.js 前端
├── docker-compose.yml
└── README.md
```

---

### 🚀 快速开始

```bash
git clone https://github.com/YOUR_USERNAME/next-fastapi-starter.git
cd next-fastapi-starter
docker compose up --build
```

---

### 🌐 访问

* 前端：http://localhost:3000
* 后端：http://localhost:8000

---

### ⚙️ 环境变量

**api/.env**

```env
DATABASE_URL=postgresql://colvor:colvor123@postgres:5432/colvor
```

**web/.env.local**

```env
NEXT_PUBLIC_API_URL=http://localhost:8000
```

---

### 🔗 前后端通信

```ts
fetch(process.env.NEXT_PUBLIC_API_URL + "/")
```

---

### 🐳 服务说明

* `postgres`：数据库
* `api`：后端
* `web`：前端

服务之间通过服务名通信（不要用 localhost）

---

### 🧠 本地开发

```bash
# frontend
cd web
npm install
npm run dev
```

```bash
# backend
cd api
pip install -r requirements.txt
uvicorn main:app --reload
```

---

## English

### ✨ Features

* ⚡ Next.js frontend (App Router)
* 🐍 FastAPI backend
* 🗄️ PostgreSQL database
* 🐳 One-command startup with Docker Compose
* 🔄 Hot reload support
* 🧱 Clean structure for MVP development

---

### 📁 Project Structure

```
.
├── api/          # FastAPI backend
├── web/          # Next.js frontend
├── docker-compose.yml
└── README.md
```

---

### 🚀 Quick Start

```bash
git clone https://github.com/YOUR_USERNAME/next-fastapi-starter.git
cd next-fastapi-starter
docker compose up --build
```

---

### 🌐 Access

* Frontend: http://localhost:3000
* Backend: http://localhost:8000

---

### ⚙️ Environment Variables

**api/.env**

```env
DATABASE_URL=postgresql://colvor:colvor123@postgres:5432/colvor
```

**web/.env.local**

```env
NEXT_PUBLIC_API_URL=http://localhost:8000
```

---

### 🔗 Frontend ↔ Backend

```ts
fetch(process.env.NEXT_PUBLIC_API_URL + "/")
```

---

### 🐳 Services

* `postgres`: database
* `api`: backend
* `web`: frontend

Services communicate via service names (not localhost)

---

### 🧠 Local Development

```bash
# frontend
cd web
npm install
npm run dev
```

```bash
# backend
cd api
pip install -r requirements.txt
uvicorn main:app --reload
```

---

## 📄 License

MIT

---
