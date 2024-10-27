1. Phân tích kiến trúc
Đề xuất kiến trúc
Hệ thống "Payroll System" sẽ được xây dựng theo kiến trúc đa tầng (Multi-Tier). Kiến trúc này chia hệ thống thành các lớp (layer) riêng biệt để dễ dàng quản lý và mở rộng:
- Presentation Layer (Tầng giao diện): Là tầng giao tiếp với người dùng, nơi hiển thị thông tin và nhận yêu cầu của họ.
- Business Logic Layer (Tầng xử lý nghiệp vụ): Tầng này xử lý các quy tắc nghiệp vụ của hệ thống, bao gồm việc tính lương, quản lý thông tin nhân viên, thẻ công và các quy trình thanh toán.
- Data Access Layer (Tầng truy xuất dữ liệu): Là tầng quản lý cơ sở dữ liệu, xử lý các thao tác lưu trữ, truy vấn dữ liệu, và đảm bảo an toàn dữ liệu.
