# HIT SYMPHONY

![Java](https://img.shields.io/badge/Java-17-blue)![Spring Boot](https://img.shields.io/badge/Spring_Boot-3.x-brightgreen)![ReactJS](https://img.shields.io/badge/ReactJS-18.x-blue?logo=react)![MySQL](https://img.shields.io/badge/MySQL-8+-orange?logo=mysql)![License](https://img.shields.io/badge/license-MIT-green)

Nền tảng quản lý thành viên, lớp học và các hoạt động dành cho Câu lạc bộ HIT. Dự án hướng tới việc cung cấp một không gian chuyên nghiệp để quản lý và giao tiếp, giải quyết các vấn đề thiếu hiệu quả trong việc quản lý thành viên cũng như tương tác sau các buổi học và sự kiện.

## ✨ Chức năng chính

*   **👤 Quản lý Người dùng**: Quản lý thông tin, vai trò và tài khoản của thành viên.
*   **🔐 Xác thực & Phân quyền**: Đăng nhập, quản lý token (`AccessToken` & `RefreshToken`), phân quyền theo vai trò.
*   **🏫 Quản lý Lớp học**: Tạo, cập nhật, xóa và quản lý thành viên trong các lớp học.
*   **📚 Quản lý Buổi học**: Lên lịch và quản lý nội dung cho từng buổi học cụ thể.
*   **📝 Quản lý Bài tập**: Giao bài tập, nộp bài và chấm điểm.
*   **🏆 Quản lý Cuộc thi**: Tổ chức các cuộc thi, quản lý thí sinh và bài dự thi.
*   **🔔 Quản lý Thông báo**: Gửi thông báo tới các lớp học hoặc cuộc thi.

## 🛠️ Công nghệ sử dụng

| Hạng mục      | Công nghệ                                                |
| :------------ | :------------------------------------------------------- |
| **Backend**   | Spring Boot, Spring Security, Spring Data JPA, JWT       |
| **Frontend**  | ReactJS                                                  |
| **Database**  | MySQL                                                    |
| **DevOps**    | Docker                                                   |
| **Dịch vụ**   | Cloudinary (Lưu trữ ảnh)                                 |
| **Công cụ**   | Maven, Postman, IntelliJ IDEA                            |

---

## 🚀 Cài đặt & Chạy dự án

### 1. Yêu cầu Môi trường (Prerequisites)

*   **IDE**: **IntelliJ IDEA** (Khuyến nghị).
*   **Java**: **JDK 17**.
*   **Maven**: **3.9+**.
*   **MySQL**: **8.0+**.
*   **Tài khoản Cloudinary**: Để lưu trữ file.

### 2. Clone dự án

```bash
git clone https://github.com/HIT-SYMPHONY/Backend-Symphony.git
cd Backend-Symphony
```

### 3. Cấu hình

Mọi cấu hình được quản lý trong file `application.properties` tại `src/main/resources`. Hãy sao chép và điền thông tin thực tế của bạn vào các trường dưới đây.

<details>
<summary><b>📄 Nhấn vào đây để xem nội dung file application.properties</b></summary>

```properties
spring.application.name=BackendSymphony

# DATABASE
spring.datasource.url=jdbc:mysql://localhost:3306/backendsymphony_db?createDatabaseIfNotExist=true
spring.datasource.username=root
spring.datasource.password=MAT_KHAU_MYSQL_CUA_BAN
spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver

# JPA / HIBERNATE
spring.jpa.database-platform=org.hibernate.dialect.MySQL8Dialect
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true

# JWT
jwt.secret=CHUOI_BI_MAT_MA_HOA_JWT_CUA_BAN
jwt.access.expiration_time=60
jwt.refresh.expiration_time=1440

# CLOUDINARY
cloudinary.cloud_name=TEN_CLOUD_CUA_BAN
cloudinary.api_key=API_KEY_CUA_BAN
cloudinary.api_secret=API_SECRET_CUA_BAN

# EMAIL (Ví dụ với Gmail)
spring.mail.host=smtp.gmail.com
spring.mail.port=587
spring.mail.username=EMAIL_GMAIL_CUA_BAN@gmail.com
# Lưu ý: Đây là Mật khẩu Ứng dụng (App Password), không phải mật khẩu đăng nhập Gmail
spring.mail.password=MAT_KHAU_UNG_DUNG_GMAIL_CUA_BAN
spring.mail.properties.mail.smtp.auth=true
spring.mail.properties.mail.smtp.starttls.enable=true

# CÁC CẤU HÌNH KHÁC
logging.level.org.springframework.security=DEBUG
spring.servlet.multipart.max-file-size=5MB
spring.servlet.multipart.max-request-size=10MB
spring.datasource.hikari.maximum-pool-size=10
spring.datasource.hikari.minimum-idle=5
spring.datasource.hikari.idle-timeout=30000
spring.datasource.hikari.max-lifetime=60000
spring.datasource.hikari.connection-timeout=20000
spring.datasource.hikari.pool-name=HikariCP-BackendSymphony
```
</details>


### 4. Chạy ứng dụng
Mở dự án bằng IntelliJ IDEA, đợi Maven tải các thư viện, sau đó nhấn nút ▶️ **Run** trên thanh công cụ.
<img width="572" alt="image" src="https://github.com/user-attachments/assets/445e4214-e06e-42d4-9250-52b9ffcc2fab" />

---

## 🤝 Hướng dẫn Đóng góp
Chúng tôi hoan nghênh mọi đóng góp! Vui lòng tuân thủ quy trình dưới đây:

1.  **Tạo branch mới từ `develop`**:
    ```bash
    git checkout -b feature/ten-tinh-nang
    ```

2.  **Commit các thay đổi**: Sử dụng commit message theo quy ước.
    *   Đối với tính năng mới:
        ```bash
        git commit -m "feat: ten feature"
        ```
    *   Đối với sửa lỗi:
        ```bash
        git commit -m "fix: noi-dung-fix"
        ```

3.  **Đẩy branch lên repository**:
    ```bash
    git push origin feature/ten-tinh-nang
    ```

4.  **Tạo Pull Request**

## 📂 Cấu trúc Thư mục
<details>
<summary><b>Nhấn vào đây để xem chi tiết cấu trúc thư mục</b></summary>

```
.
└── src
    └── main
        ├── java
        │   └── my_computer.backendsymphony
        │       ├── base          # Chứa các lớp cơ sở (Base classes)
        │       ├── config        # Các lớp cấu hình cho ứng dụng
        │       ├── constant      # Các hằng số và Enum
        │       ├── controller    # Tầng xử lý request (API Endpoints)
        │       ├── domain        # Chứa các đối tượng dữ liệu
        │       │   ├── dto       # Data Transfer Objects
        │       │   ├── entity    # Các thực thể ánh xạ CSDL (JPA Entities)
        │       │   └── mapper    # Ánh xạ giữa Entity và DTO (MapStruct)
        │       ├── exception     # Xử lý ngoại lệ tùy chỉnh
        │       ├── repository    # Tầng truy cập dữ liệu (Data Access Layer)
        │       ├── security      # Cấu hình bảo mật (Spring Security, JWT)
        │       ├── service       # Tầng logic nghiệp vụ (Business Logic)
        │       │   ├── impl      # Các lớp implement service interface
        │       │   └── ...Service # Các service interface
        │       ├── util          # Các lớp tiện ích (helper methods)
        │       ├── websocket     # Xử lý giao tiếp thời gian thực
        │       └── BackendSymphonyApplication.java # Điểm khởi chạy ứng dụng
        │
        └── resources                 # Chứa các file tài nguyên, cấu hình
            └── application.properties # File cấu hình chính của Spring Boot
```
</details>


## 🔗 Tài liệu & Demo

*   **Thiết kế Giao diện**: [Link Figma](https://www.figma.com/design/vI7ilYugZQZ8GUxwJtpq12/HIT---Symphony---Design?node-id=27-26&t=viIK8WCRXO19vGm2-0)
*   **Bản Demo trực tiếp**: [Link Demo](http://159.223.49.56:5173/)
