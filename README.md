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
    # CORE SERVER CONFIGURATION
    server.port=8080
    
    # DATABASE CONFIGURATION (MySQL)
    spring.datasource.url=jdbc:mysql://localhost:3306/backendsymphony_db?createDatabaseIfNotExist=true
    spring.datasource.username=root
    spring.datasource.password=MAT_KHAU_MYSQL_CUA_BAN
    spring.datasource.driver-class-name=com.mysql.cj.jdbc.Driver
    
    # JPA / HIBERNATE CONFIGURATION
    spring.jpa.hibernate.ddl-auto=update
    spring.jpa.show-sql=true
    spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQLDialect
    
    # ADMIN DEFAULT ACCOUNT
    admin.username=admin
    admin.password=admin123@
    
    # JWT CONFIGURATION
    jwt.secret=dayLaChuoiBiMatSieuDaiSieuBaoMatDungDeMaHoaTokenJWT123456789
    jwt.accessExpirationTime=86400000
    jwt.refreshExpirationTime=604800000
    
    # EMAIL (SMTP) CONFIGURATION
    spring.mail.host=smtp.gmail.com
    spring.mail.port=587
    spring.mail.username=EMAIL_CUA_BAN@gmail.com
    spring.mail.password=MAT_KHAU_UNG_DUNG_GMAIL_CUA_BAN # (Lưu ý: Mật khẩu ứng dụng của Gmail)
    
    # CLOUDINARY CONFIGURATION
    cloudinary.cloud_name=TEN_CLOUD_CUA_BAN
    cloudinary.api_key=API_KEY_CUA_BAN
    cloudinary.api_secret=API_SECRET_CUA_BAN
   ```
4. Chạy chương trình
   
## Giấy phép:
MIT/GPL/...

## Cách đóng góp:
- Đứng từ develop, tạo branch mới: git checkout -b feature/ten-tinh-nang
- Commit thay đổi: git commit -m "feat: ten feature"
- Push lên branch: git push origin feature/ten-tinh-nang
- Tạo Pull Request
- Sửa lỗi : git commit -m "fix/noi-dung-fix"

## Tài liệu thêm:
- [Figma](https://www.figma.com/design/vI7ilYugZQZ8GUxwJtpq12/HIT---Symphony---Design?node-id=27-26&t=viIK8WCRXO19vGm2-0)
- [Demo](http://159.223.49.56:5173/?fbclid=IwY2xjawMEOHNleHRuA2FlbQIxMQABHtzK8v0fkP2a6I5YLLXZsOrcbyj1gl2lhs7TCaZiAwm-VzOH7qKIT_hvIMTk_aem_fHSOiPdGqMYKNadEMss5LA)


