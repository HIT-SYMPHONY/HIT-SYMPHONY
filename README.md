## Tên dự án:
HIT SYMPHONY

## Mục tiêu dự án:
- Tạo web quản lý thành viên CLB
- Giải quyết vấn đề thiếu không gian chuyên nghiệp trong việc quản lý thành viên cũng như giao tiếp sau buổi học
- Hướng tới các thành viên trong câu lạc bộ

## Chức năng chính:
- Tài khoản và xác thực
- Quản lý lớp học và thành viên
- Quản lý bài tập và kết quả học tập
- Quản lý cuộc thi

## Công nghệ sử dụng:
- Frontend: ReactJS
- Backend: SpringBoot
- Cơ sở dữ liệu: MySQL

## Cách sử dụng:
...

## 🛠️ Lỗi thường gặp & cách khắc phục

| **Lỗi** | **Nguyên nhân** | **Cách khắc phục** |
|--------|----------------|-------------------|
| 🔑 **Không đăng nhập được** | Sai thông tin đăng nhập, tài khoản bị khóa hoặc chưa được cấp | Kiểm tra tài khoản trong hệ thống; nếu cần, admin cấp lại hoặc mở khóa |
| ⚠️ **Không tạo được lớp học mới** | Trùng tên lớp hoặc thiếu thông tin bắt buộc | Kiểm tra xem tên lớp đã tồn tại chưa và nhập đầy đủ các trường |
| 🚫 **Không thể nộp bài tập** | Quá hạn nộp hoặc thiếu tệp đính kèm | Kiểm tra thời hạn nộp bài và đảm bảo đã chọn tệp hợp lệ |
| 🔄 **Không sửa được thông tin cá nhân** | Session hết hạn hoặc backend không phản hồi | Đăng nhập lại và kiểm tra kết nối backend |
| 📅 **Thông báo lịch học không hiển thị** | Chưa có lịch học nào được tạo hoặc lỗi frontend | Kiểm tra dữ liệu backend và debug phần hiển thị lịch |
| ❗ **Không tạo được tài khoản mới** | Trùng email hoặc thiếu thông tin đầu vào | Kiểm tra tính hợp lệ của email và điền đủ thông tin |
| ❌ **Không xóa được lớp học** | Lớp học vẫn còn thành viên hoặc bài tập liên kết | Cần xoá hoặc chuyển thành viên, bài tập trước khi xoá lớp |
| 🧑‍🤝‍🧑 **Không phân nhóm được** | Số lượng thành viên không hợp lệ hoặc nhóm đã đầy | Kiểm tra lại số lượng thành viên và giới hạn nhóm |
| 🔒 **Lỗi phân quyền (403 Forbidden)** | Người dùng không có quyền truy cập chức năng đó | Kiểm tra lại role (vai trò) của tài khoản, cấu hình phân quyền backend |
| 🔌 **Frontend không gọi được API** | Sai địa chỉ API hoặc backend chưa chạy | Kiểm tra biến môi trường (env) hoặc trạng thái server backend |
| 🐞 **Lỗi dữ liệu không đồng bộ giữa frontend và backend** | Không reload dữ liệu sau thao tác tạo/xoá | Gọi lại API fetch dữ liệu sau mỗi thao tác hoặc dùng state management (Redux, Context) hợp lý |
| 🧭 **Lỗi định tuyến (404 Not Found)** | Sai đường dẫn hoặc chưa khai báo route | Kiểm tra các route trong React Router hoặc Spring Controller |



## Liên hệ hỗ trợ:
...

## Giấy phép:
MIT/GPL/...

## Các đóng góp:
...

## Tài liệu thêm:
- [Figma](...)
- [Demo](...)


