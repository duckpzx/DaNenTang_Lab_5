# 📝 Flutter Todo App

> Ứng dụng quản lý công việc cá nhân được xây dựng với Flutter, NodeJS và MongoDB Atlas.

---

## 🎬 Video Demo

[![Demo Video](https://img.shields.io/badge/▶%20Xem%20Demo-Video-red?style=for-the-badge&logo=github)](https://private-user-images.githubusercontent.com/126335789/589925769-93a4bdc7-0e46-4195-a098-cd50c4fe9e2e.mp4?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3NzgzMTIzODgsIm5iZiI6MTc3ODMxMjA4OCwicGF0aCI6Ii8xMjYzMzU3ODkvNTg5OTI1NzY5LTkzYTRiZGM3LTBlNDYtNDE5NS1hMDk4LWNkNTBjNGZlOWUyZS5tcDQ_WC1BbXotQWxnb3JpdGhtPUFXUzQtSE1BQy1TSEEyNTYmWC1BbXotQ3JlZGVudGlhbD1BS0lBVkNPRFlMU0E1M1BRSzRaQSUyRjIwMjYwNTA5JTJGdXMtZWFzdC0xJTJGczMlMkZhd3M0X3JlcXVlc3QmWC1BbXotRGF0ZT0yMDI2MDUwOVQwNzM0NDhaJlgtQW16LUV4cGlyZXM9MzAwJlgtQW16LVNpZ25hdHVyZT0wM2ZlYjBhYzVmZDFkMzNlZWY2MzRjNDY2NzU0ZDI5ZmQxMmZhYWVlNjkzOTc1NDI0MTFjMjRhMjVjMTljNmQyJlgtQW16LVNpZ25lZEhlYWRlcnM9aG9zdCZyZXNwb25zZS1jb250ZW50LXR5cGU9dmlkZW8lMkZtcDQ)

---

## 👤 Thông tin sinh viên

| Họ và tên | MSSV |
|-----------|------|
| **PHẠM XUÂN ĐỨC** | `2224802010615` |

---

## �️ Tech Stack

| Thành phần | Công nghệ |
|------------|-----------|
| 📱 Frontend | Flutter (Web / Android) |
| ⚙️ Backend | Node.js + Express |
| 🗄️ Database | MongoDB Atlas (Cloud) |
| 🔐 Auth | JWT + bcrypt |

---

## 📁 Cấu trúc dự án

```
Lab5/
├── 📂 nodejs_backend/        # Backend REST API
│   ├── config/               # Cấu hình database
│   ├── controller/           # Xử lý logic
│   ├── models/               # Schema MongoDB
│   ├── routes/               # Định tuyến API
│   ├── app.js
│   └── index.js
│
└── 📂 flutter_todo_app/      # Flutter Frontend
    ├── lib/
    │   ├── main.dart         # Entry point
    │   ├── loginPage.dart    # Màn hình đăng nhập
    │   ├── registration.dart # Màn hình đăng ký
    │   ├── dashboard.dart    # Màn hình chính
    │   ├── config.dart       # Cấu hình API URL
    │   └── applogo.dart      # Widget logo
    └── pubspec.yaml
```

---

## ⚙️ Hướng dẫn chạy dự án

### 1️⃣ Khởi động Backend

```bash
cd nodejs_backend
npm install
node index.js
```

> Server chạy tại: **http://localhost:3000**

### 2️⃣ Khởi động Flutter App

```bash
cd flutter_todo_app
flutter pub get
flutter run -d chrome
```

> App chạy tại: **http://localhost:8080**

---

## ✨ Tính năng

- 🔐 **Đăng ký** tài khoản — mã hóa mật khẩu bằng `bcrypt`
- 🔑 **Đăng nhập** — xác thực bằng `JWT Token` (hết hạn sau 1 giờ)
- ➕ **Thêm** công việc mới
- 📋 **Xem** danh sách công việc theo tài khoản
- 🗑️ **Xóa** công việc bằng cách vuốt sang trái
- ☁️ **Lưu trữ** trên MongoDB Atlas Cloud

---

## 📡 API Endpoints

| Method | Endpoint | Chức năng |
|--------|----------|-----------|
| `POST` | `/register` | Đăng ký tài khoản mới |
| `POST` | `/login` | Đăng nhập, nhận JWT token |
| `POST` | `/createToDo` | Tạo todo mới |
| `POST` | `/getUserTodoList` | Lấy danh sách todo của user |
| `POST` | `/deleteTodo` | Xóa todo theo ID |

---

## 📦 Các thư viện sử dụng

### Flutter
| Package | Mô tả |
|---------|-------|
| `velocity_x` | UI utility widgets |
| `http` | Gọi REST API |
| `shared_preferences` | Lưu token cục bộ |
| `jwt_decoder` | Giải mã JWT token |
| `flutter_slidable` | Vuốt để xóa item |

### Node.js
| Package | Mô tả |
|---------|-------|
| `express` | Web framework |
| `mongoose` | ODM cho MongoDB |
| `jsonwebtoken` | Tạo & xác thực JWT |
| `bcrypt` | Mã hóa mật khẩu |
| `cors` | Xử lý CORS |

---

<div align="center">
  <sub>© 2024 PHẠM XUÂN ĐỨC — MSSV: 2224802010615</sub>
</div>
