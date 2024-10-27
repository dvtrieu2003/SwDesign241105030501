1. Phân tích kiến trúc
Đề xuất kiến trúc
Hệ thống "Payroll System" sẽ được xây dựng theo kiến trúc đa tầng (Multi-Tier). Kiến trúc này chia hệ thống thành các lớp (layer) riêng biệt để dễ dàng quản lý và mở rộng:
- Presentation Layer (Tầng giao diện): Là tầng giao tiếp với người dùng, nơi hiển thị thông tin và nhận yêu cầu của họ.
- Business Logic Layer (Tầng xử lý nghiệp vụ): Tầng này xử lý các quy tắc nghiệp vụ của hệ thống, bao gồm việc tính lương, quản lý thông tin nhân viên, thẻ công và các quy trình thanh toán.
- Data Access Layer (Tầng truy xuất dữ liệu): Là tầng quản lý cơ sở dữ liệu, xử lý các thao tác lưu trữ, truy vấn dữ liệu, và đảm bảo an toàn dữ liệu.
![Biểu đồ Pakage](https://www.planttext.com/api/plantuml/png/R91B2i8m48RtEKKkq2j85Lq85RhGLUbYJ8SIpADCqaKGJ-R28ta5CmYbrMx_npS_ytw-oX21ucYD643Te4TP4mPq4QBsheA49Ez2okPoRCL3JAdT6BJ342hVQpMBrP1iRjVaLNOzjIoUjKK5r9t0vUvNEzZ1-8GuQJFu7Y9i5GEMPFB6i7U5W0i8YqputruKcvMjOcK-9tyEYn9Tnx_v0000__y30000)
Giải thích các thành phần
- UI (PresentationLayer): Giao diện tương tác với người dùng, cho phép nhân viên và quản lý nhập và truy vấn dữ liệu.
- PaymentProcessor (BusinessLogicLayer): Xử lý các quy tắc và logic tính toán thanh toán cho từng nhân viên.
- TimecardManager (BusinessLogicLayer): Quản lý thông tin thẻ công của nhân viên.
- EmployeeManager (BusinessLogicLayer): Quản lý thông tin nhân viên, bao gồm cập nhật và tra cứu dữ liệu.
- PayrollDatabase (DataAccessLayer): Quản lý lưu trữ và truy xuất dữ liệu thanh toán.
- EmployeeData (DataAccessLayer): Lưu trữ thông tin về các nhân viên và truy vấn thông tin nhân viên khi cần.
2. Cơ chế phân tích
- Cơ chế quản lý người dùng: Đảm bảo quyền truy cập hợp lệ cho từng vai trò (nhân viên, quản lý).
- Cơ chế tính toán lương: Tự động tính toán lương dựa trên thông tin thẻ công và các quy tắc tính lương.
- Cơ chế quản lý và lưu trữ dữ liệu: Đảm bảo dữ liệu được lưu trữ chính xác và truy xuất hiệu quả.
- Cơ chế bảo mật: Đảm bảo an toàn cho dữ liệu nhạy cảm, đặc biệt là thông tin cá nhân và lương của nhân viên.
- Cơ chế xử lý thời gian thực: Cập nhật tức thời thông tin về thời gian làm việc và thanh toán, giúp hệ thống luôn duy trì dữ liệu chính xác.
3. Phân tích ca sử dụng "Select Payment"
  Xác định các lớp phân tích
- PaymentProcessor: Lớp xử lý các quy tắc và tính toán thanh toán.
- Employee: Đại diện cho thông tin nhân viên.
- PayrollDatabase: Quản lý lưu trữ dữ liệu thanh toán.
![Biểu đồ Sequence cho Select Payment](https://www.planttext.com/api/plantuml/png/Z94z3i8m38Ltdy8Nu08TK14mi5LK7C2aHggKn5NY8lLi31o9Az1A9OAc0wlztllyyteyowWKj7SMoAW4l4GEq8sbrhGTUSMA1iTUgo26OvIi6SJQ0obTAV9Fx-WwAmCpm9I9csqMLM3DbarYm58mcxuH1PvPGyjtJW0y-Pl0GeURLM3coNWVHO5xigQtf9pcI-xryBc2EoVzlzlKuz4JODpDI6YWPDzCBta3003__mC0)
![Biểu đồ lớp cho Select Payment](https://www.planttext.com/api/plantuml/png/R9112i8m44NtEKMMBTWBT25TwC9TqHDCsq4Baumaaq8HJ-R28ta5OqqfMBCQykU__vdNurbv0IV1a6e9lDSrZ0Qjr8vRz9wTlYaTNmlK1WB1f6TehiGZOgdtQSfBtN5e2DKziMObCVgkrBsLQRPWelKahhVdwUF2mT5uZ0ahJ8nqJBG3WGRyJ7COpJZW798bVBuqclQyi5krFdntDneC1ojpPFGEt7SnMQtkK1JR1VnN_UcfAhJTvx1l0000__y30000)
  Giải thích các lớp phân tích
- PaymentProcessor: Có nhiệm vụ chính là tính toán thanh toán. Các phương thức bao gồm calculatePayment(), nhận thông tin Employee và trả về số tiền phải trả.
- Employee: Lưu trữ thông tin nhân viên, bao gồm id, name, và hourlyRate.
- PayrollDatabase: Quản lý việc truy xuất và lưu trữ thông tin thanh toán.
4. Phân tích ca sử dụng "Maintain Timecard"
  Xác định các lớp phân tích
- TimecardManager: Quản lý và cập nhật thẻ công cho nhân viên.
- Timecard: Đại diện cho thông tin thẻ công của nhân viên.
- PayrollDatabase: Quản lý lưu trữ dữ liệu về thẻ công
![Biểu đồ Sequence cho Maintain Timecard](https://www.planttext.com/api/plantuml/png/UhzxlqDnIM9HIMbk3bTYSab-aK9eSMeHLm5GA3Cvio0nhqGX93CtDJcnACKtCIyn7Kqk8B6oA3ydnoMn934fiJWLgpukBf2H2hfsw2PPAJWNfIQMf29KeYb0rcEbu9cNMPAPc9DPXLy3cfEi588Jov1qEAJcfO0y2m000F__0m00)
![Biểu đồ lớp cho Maintain Timecard](https://www.planttext.com/api/plantuml/png/R90z3i8m38NtdC8ZIEq5Cg0EB0m81Yfcjx6W8cqg9wbK8Kx6m96u0cbLMYbg1kVdsU-pytr_CkkGdQ-rA3LQ2vUgfX9P7R716p4y1OHLCg6Z4-Uj2li_PqDrgqrFT50IgiObCAWIzY4cS3UUxTNmWuAgZ2yqRILqfbBY5S4cob8zNbSCnlU8EhkTiMUZTQZ70YrDfXQxfM4t7UICNbeIyUXfkflJLiK8A39grF2JFm000F__0m00)
  Giải thích các lớp phân tích
- TimecardManager: Xử lý việc tạo và cập nhật thẻ công cho nhân viên. Các phương thức bao gồm createOrUpdateTimecard(), nhận employeeId, date, và hoursWorked.
- Timecard: Chứa thông tin thẻ công của nhân viên như date, hoursWorked, và employeeId.
- PayrollDatabase: Quản lý lưu trữ và truy vấn các thẻ công trong cơ sở dữ liệu.
5. Hợp nhất kết quả phân tích
 Các ca sử dụng Select Payment và Maintain Timecard đã được phân tích để xác định các lớp cần thiết và mối quan hệ giữa chúng. Sau khi kết hợp, ta có các lớp cốt lõi của hệ thống "Payroll System" bao gồm:
- Employee: Thông tin nhân viên.
- Timecard: Thông tin chấm công cho từng ngày.
- PayrollDatabase: Lớp quản lý dữ liệu.
- PaymentProcessor: Xử lý tính toán thanh toán.
- TimecardManager: Quản lý thẻ công.
Hệ thống sẽ có kiến trúc đa tầng, hỗ trợ bảo trì và mở rộng dễ dàng. Các cơ chế đã được phân tích sẽ đảm bảo hiệu quả xử lý và bảo mật trong toàn bộ hệ thống.

