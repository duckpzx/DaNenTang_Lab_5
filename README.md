# 📝 Flutter Todo App

> Ứng dụng quản lý công việc cá nhân được xây dựng với Flutter, NodeJS và MongoDB Atlas.

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

### Video
https://github.com/duckpzx/Cotyphu/issues/2#issue-4411687143
