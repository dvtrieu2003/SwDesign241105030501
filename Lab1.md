1.Phân tích kiến trúc:

Đề xuất kiến trúc : Kiến trúc tầng.

Kiến trúc này chia hệ thống thành ba tầng:

+) Tầng giao diện người dùng(Presentation Layer)

+) Tầng ứng dụng(Application Layer)

+) Tầng truy cập dữ liệu(Data Access Layer).

Lý do lựa chọn kiến trúc này: Mỗi tầng thực hiện chức năng độc lập, cho phép thay đổi một tầng mà không ảnh hưởng đến các tầng khác, đặc biệt hữu ích khi cần bảo trì hoặc nâng cấp hệ thống.Các tầng có thể dễ dàng mở rộng hoặc điều chỉnh để đáp ứng các yêu cầu mới mà không làm thay đổi toàn bộ hệ thống, được tách biệt hỗ trợ kiểm thử đơn vị và kiểm thử tích hợp tốt hơn, đảm bảo logic nghiệp vụ và xử lý dữ liệu chính xác.Các tầng tách biệt theo chức năng giúp hệ thống dễ bảo trì và kiểm tra lỗi, cải thiện năng suất quản lý và bảo trì hệ thống.

Ý nghĩa từng phần trong kiến trúc:

+) Tầng giao diện người dùng(Presentation): Đây là tầng chịu trách nhiệm hiển thị thông tin và cung cấp giao diện để người dùng tương tác với hệ thống.

+)Tầng ứng dụng (Application Layer): Tầng trung gian, xử lý các yêu cầu từ tầng giao diện và điều phối nghiệp vụ. Tầng này thực hiện các quy trình logic nghiệp vụ và đảm bảo tính nhất quán của dữ liệu khi có thay đổi.

+) Tầng dữ liệu(Data Access Layer): Tầng chịu trách nhiệm truy xuất, lưu trữ, và quản lý dữ liệu của hệ thống, đảm bảo tính toàn vẹn và nhất quán của dữ liệu.
 ![Biểu đồ Package cho Kiến trúc Hệ thống](https://www.planttext.com/api/plantuml/png/T91D2W8n34RtFKKlu1La2kD2SB0BFK1eWnRxHreNWtWo5nx9AzY2oenbkdnDlfVazNXsAGFbgxCiWhh02RaaJEWpP1Fy3aOaVcEyF6KX9RvnqOOHyRYTm05ywQJ2xkoN8sAqHYt4I1WfM2ifA4mfqFpB5V-0-HpqX1-CGmMaFxAfgeSCGjMavO5xiM_zS_WrL5hIsqEirirMh5cp5FtDmphqkfxu3G00__y30000)
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
![Biểu đồ Lớp Hợp Nhất cho cả hai ca sử dụng "Select Payment" và "Maintain Timecard](https://www.planttext.com/api/plantuml/png/V5DBReCm4Drp2Y_RHI_0eig2IiqYKgIc1vYOIOfaREGnaQAg9-kYH-eLEeCn42Sf4iZCp7jlVlxz_bbH01_wrXJQ095w9_Jgir3oz7nULwLw2xwnnsWZDAZ35iujsh31yE7gXyVeQg6nWTzTqw86B_QlOgHbW7V6RBtJIEHcYQw6W3VfD1ZTc-WLR4Ot0n9NE_pjpXrUfWnQkzw6jJsuh1OuuQGvSQVqDs3XY5ccYze6wmbCazclY1A3n9MgukyeBvsNe788ZKQqTMuABe1vTRqdHhj-Rt1E_vzUin3iWJ39U-JIyOGlRMVS6L7ygGoX6djQ8S_GKF8aL1BAKPcTanWswEdvUkIbB1If0nz7tnIRztmHEdKn-YJ5ueewoYrMekHjb70gSkg5ciWCKwLxZ1TzB7bYpdDQNPHITMpLBOcxs92q4tZ54vVhzmS00F__0m00)
