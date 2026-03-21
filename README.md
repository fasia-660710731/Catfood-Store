# 🚀 How to Run This Project

## 1. Clone Repository

```bash
git clone https://github.com/your-username/catfood-store.git
cd catfood-store
```

---

## 2. Setup Environment Variables

สร้างไฟล์ `.env` ในแต่ละ service

### 🔹 Backend (`catfoodstore_backend/.env`)

```
PORT=8080
DB_HOST=db
DB_PORT=5432
DB_USER=postgres
DB_PASSWORD=yourpassword
DB_NAME=catfood
JWT_SECRET=your_secret
```

### 🔹 Database (`catfoodstore_db/.env`)

```
POSTGRES_USER=postgres
POSTGRES_PASSWORD=yourpassword
POSTGRES_DB=catfood
```

---

## 3. Run ด้วย Docker

```bash
docker-compose up --build
```

---

## 4. เข้าใช้งานระบบ (ผ่าน Nginx)

* 🌐 Web Application: http://localhost (Port 80)
* ⚙️ API (ผ่าน Nginx): http://localhost/api
* 🗄️ pgAdmin: http://localhost:5050

---

## ⚠️ หมายเหตุ

* ระบบใช้ Nginx เป็น Reverse Proxy (port 80)
* Backend และ Frontend ทำงานอยู่ภายใน Docker network
* ต้องติดตั้ง Docker และ Docker Compose ก่อนใช้งาน
