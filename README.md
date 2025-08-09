## Tên dự án:
HIT SYMPHONY

## Mục tiêu dự án:
- Tạo web quản lý thành viên CLB
- Giải quyết vấn đề thiếu không gian chuyên nghiệp trong việc quản lý thành viên cũng như giao tiếp sau buổi học
- Hướng tới các thành viên trong câu lạc bộ

## Chức năng chính:
- Quản lý Xác thực và Tài khoản (Authentication)
- Quản lý Người dùng (User Management)
- Quản lý Lớp học (Classroom Management)
- Quản lý Buổi học (Lesson Management)
- Quản lý Bài tập & Tương tác (Post & Comment-Post)
- Quản lý Cuộc thi (Competition Management)
- Quản lý Bài dự thi (Competition Submission)
- Quản lý Thông báo (Notification)

## Công nghệ sử dụng:
- ReactJS
- SpringBoot
- Spring Security
- Spring Data JPA
- JWT
- Postman
- Cloudinary 
- MySQL
- Docker

## Yêu cầu hệ thống :
- IDE: Intellij Community
- Java: 17
- Maven: 3.9+
- MySQL: 8+
- Cloudiary

## Cấu trúc thư mục
```
.
└── src
    └── main
        ├── java
        │   └── my_computer.backendsymphony
        │           ├── base          # Chứa các lớp cơ sở (Base classes)
        │           ├── config        # Các lớp cấu hình cho ứng dụng
        │           ├── constant      # Các hằng số và Enum
        │           ├── controller    # Tầng xử lý request (API Endpoints)
        │           ├── domain        # Chứa các đối tượng dữ liệu
        │           │   ├── dto       # Data Transfer Objects
        │           │   ├── entity    # Các thực thể ánh xạ CSDL (JPA Entities)
        │           │   └── mapper    # Ánh xạ giữa Entity và DTO (MapStruct)
        │           ├── exception     # Xử lý ngoại lệ tùy chỉnh
        │           ├── repository    # Tầng truy cập dữ liệu (Data Access Layer)
        │           ├── security      # Cấu hình bảo mật (Spring Security, JWT)
        │           ├── service       # Tầng logic nghiệp vụ (Business Logic)
        │           │   ├── impl      # Các lớp implement service interface
        │           │   └── ...Service # Các service interface
        │           ├── util          # Các lớp tiện ích (helper methods)
        │           ├── websocket     # Xử lý giao tiếp thời gian thực
        │           └── BackendSymphonyApplication.java # Điểm khởi chạy ứng dụng
        │
        └── resources                 # Chứa các file tài nguyên, cấu hình
            └── application.properties # File cấu hình chính của Spring Boot
```
## Cách cài đặt
1. Clone dự án
   ```
   git clone https://github.com/HIT-SYMPHONY/Backend-Symphony.git
   ```
2. Cấu hình database
   - Cấu hình trong file application.properties
   ```
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
    
    # EMAIL
    spring.mail.host=smtp.gmail.com
    spring.mail.port=587
    spring.mail.username=EMAIL_GMAIL_CUA_BAN@gmail.com
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
3. Chạy chương trình
   - Ấn nút run trên thanh công cụ
   <img width="572" height="57" alt="image" src="https://github.com/user-attachments/assets/445e4214-e06e-42d4-9250-52b9ffcc2fab" />

## Cách đóng góp:
- Đứng từ develop, tạo branch mới: git checkout -b feature/ten-tinh-nang
- Commit thay đổi: git commit -m "feat: ten feature"
- Push lên branch: git push origin feature/ten-tinh-nang
- Tạo Pull Request
- Sửa lỗi : git commit -m "fix/noi-dung-fix"

## Tài liệu thêm:
- [Figma](https://www.figma.com/design/vI7ilYugZQZ8GUxwJtpq12/HIT---Symphony---Design?node-id=27-26&t=viIK8WCRXO19vGm2-0)
- [Demo](http://159.223.49.56:5173/?fbclid=IwY2xjawMEOHNleHRuA2FlbQIxMQABHtzK8v0fkP2a6I5YLLXZsOrcbyj1gl2lhs7TCaZiAwm-VzOH7qKIT_hvIMTk_aem_fHSOiPdGqMYKNadEMss5LA)


