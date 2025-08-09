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
src/
├── main/
│ ├── java/com/example/hit_networking_base
│ │ ├── base           # Các base dùng chung cho controller
│ │ ├── config         # Cấu hình Cloudinary, JWT properties, OpenApi, Dotenv,...
│ │ ├── constant       # Cấu hình các enum, url Constant
│ │ ├── controller     # REST API Controller
│ │ ├── domain
│ │ │  ├── dto         # Data Transfer Object
│ │ │  │  ├── request  # Dữ liệu nhận vào
│ │ │  │  ├── response # Dữ liệu trả lại
│ │ │  ├── entity      # Các entiry của ứng dựng
│ │ │  ├── mapstruct   # Map dto với entity
│ │ ├── exception      # Xử lý lỗi
│ │ └── repository     # JPA Repository
│ │ └── security       # Cấu hình security
│ │ └── service        # Các hàm xử lý logic
│ │ │  ├── impl        # Các thực hiện của các hàm xử lý logic
│ │ └── util           # Cấu hình các hàm hỗ trợ
│ └── resources/
│    ├── application.properties
.env

## Liên hệ hỗ trợ:
...

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


