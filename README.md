# 🚀 next-fastapi-starter

> 一个基于 **Next.js + FastAPI + PostgreSQL + Docker** 的现代全栈开发模板
> A modern full-stack starter powered by **Next.js + FastAPI + PostgreSQL + Docker**

---

## ✨ 项目特点 | Features

* ⚡ 前端：Next.js（App Router）
  Frontend: Next.js (App Router)

* 🐍 后端：FastAPI（高性能 API）
  Backend: FastAPI (high-performance API)

* 🗄️ 数据库：PostgreSQL
  Database: PostgreSQL

* 🐳 Docker Compose 一键启动
  One-command startup with Docker Compose

* 🔄 支持前后端热更新
  Hot reload for both frontend and backend

* 🧱 清晰结构，适合快速开发 MVP
  Clean structure for rapid MVP development

---

## 📁 项目结构 | Project Structure

```bash
.
├── api/                  # FastAPI backend
├── web/                  # Next.js frontend
├── docker-compose.yml
└── README.md
```

---

## 🚀 快速开始 | Quick Start

### 1️⃣ 克隆项目 | Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/next-fastapi-starter.git
cd next-fastapi-starter
```

---

### 2️⃣ 一键启动 | Start everything

```bash
docker compose up --build
```

---

### 3️⃣ 访问服务 | Access services

* 前端 Frontend
  👉 http://localhost:3000

* 后端 Backend
  👉 http://localhost:8000

---

## ⚙️ 环境变量 | Environment Variables

### 后端 Backend (`api/.env`)

```env
DATABASE_URL=postgresql://colvor:colvor123@postgres:5432/colvor
```

---

### 前端 Frontend (`web/.env.local`)

```env
NEXT_PUBLIC_API_URL=http://localhost:8000
```

---

## 🔗 前后端通信 | Frontend ↔ Backend

```ts
fetch(process.env.NEXT_PUBLIC_API_URL + "/")
```

---

## 🐳 Docker 说明 | Docker Services

* `postgres` → 数据库 / Database
* `api` → 后端服务 / Backend service
* `web` → 前端服务 / Frontend service

服务之间通过 **服务名通信**
Services communicate via **service names (not localhost)**

---

## 🧠 本地开发 | Local Development

### 前端 Frontend

```bash
cd web
npm install
npm run dev
```

---

### 后端 Backend

```bash
cd api
pip install -r requirements.txt
uvicorn main:app --reload
```

---

## 📌 TODO

* [ ] 用户系统（登录 / 注册）
* [ ] 数据库模型设计
* [ ] API 权限控制
* [ ] 前端接口封装
* [ ] 部署上线（VPS / Cloud）

---

## 📄 License

MIT

---

## 💡 项目定位 | About

这是一个用于快速构建 AI 工具 / SaaS 产品的基础模板
This is a starter template for building AI tools and SaaS products quickly

---
