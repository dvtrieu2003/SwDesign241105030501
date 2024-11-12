# Phân tích ca sử dụng login
- Các thành phần chính:
  + User
  + UI
  + Authentication system
  + Payroll Database
- Biểu đồ sequence phân tích ca sử dụng login :
  ![](https://www.planttext.com/api/plantuml/png/T98nIWGn58RxdEAnbO9xWIra1K4NGGGTiCrcWnESIOOaequfMrXOUGE7BGHX2y5gKbZCNYGdy0g-P1cTMJ1LNjx__-zBoBVxcXfBjItpZ9XR8K4hmmbbLcb83DUamAPWeg3ImYYPZO0QI6R3uwFIfbnYJQrG4YuhOtaUbQ6pBOUE2rffbMN7rD8vDJngkuAGC1Z6XpW79d2U-cPTW4tRJta35X4tBvibRcLi41IXz6yGMawyMmkeslSIc6_UIdXeQuO9tdqms2inNTAS7q11ZRbNUh5FUdOCwqWmwanujyp1Qle_0I60wzSqtiMvqhvPmPrtZvZZcpg4f6qj085M1MJUFSM4FaHt--iUEPfUPGeiO4J3zkhnjIPm6aXbr3vthFEsLaFOdP0GGyYKoqNu03y0003__mC0)

- Biểu đồ lớp phân tích ca ứng dụng login:
  ![](https://www.planttext.com/api/plantuml/png/f95DQWCn38NtEeMMASGN2AMaFvj25uNG0oYsaeXux21vKeQIasNH8_KA7G_JGATTjGQ1BJrz3qiVv_Ub5TBIDX5iBmar6uEFP8OlneflWFrnsFQFH0qlS5LKqdPC7thXQzRmBOqOyrRIx6g1Tpb7fWGd-88-ZaZ487Q8r3rLxSehyz1np196WRNhHifGdqtzvp-iVtExRSkEKn5FHNAwE1zPPTFTAuTQf6X_n3zJfpd61ogq9kCBt-_Ox_-37qRlt4qT5_HHhvE_04pThvsRY639ATJLVW800F__0m00)

  - Giải thích :
    + User: Đại diện cho người sử dụng hệ thống (như nhân viên hoặc quản trị viên) muốn đăng nhập vào hệ thống Payroll.
    + UI:Là giao diện mà người dùng tương tác, được sử dụng để hiển thị form đăng nhập và tiếp nhận thông tin đăng nhập từ người dùng.
    + Authentication system:Chịu trách nhiệm xác thực thông tin đăng nhập của người dùng.
    + Payroll Database: Lưu trữ thông tin đăng nhập và thông tin tài khoản của tất cả người dùng hệ thống Payroll.
# Phân tích ca sử dụng Maintain Employee Information
- Các thành phần chính
  + User
  + UI
  + Employee Management System:
  + Payroll Database
- Biểu đồ sequence phân tích ca sử dụng Maintain Employee Information
  ![](https://www.planttext.com/api/plantuml/png/b9B1IiD048Rl-nH3JteelVSWFIZQWo2qXLwdSMcMRZOnsHHo50yUV02lLX6Xq8FeAOlqi4-oJ-0hE4c8fgsAvh2GsV__vvjXtyswbsYCTHf8bio4WZXCE4DFXp6C4XwpY2w59o9K6bgZVWimWL5_itmKH3BCE8TJL3Zb0QVY84iq3qfvVLsLDgrdcCMXb7286YUOyD9G_p1M843xW3f25uQ-NGQTWJChx8pj2uBsxQkQWYPivTjx1NDXbugHc2oRNSb-J4O1cLscuBdyAOMBrEKF2gHzQoInBHybrJWbWZFF7lZ2cMj5BWn1suK7Uzji-uoXrAIl5TJXJldW5NqOqFUPsluETXWJ6yoTkOIPozUwWjrDsQQjTpKkUYhVvQicvewzMbMvvIwSq5HNXToPcteZ4xi8VmhWakYR4xhyKSF4vGlnlmcbCxVYrt663PelzT_eAprNvuprw2nU-WS0003__mC0)

- Biểu đồ lớp phân tích cho ca sử dụng Maintain Employee Information
  ![](https://www.planttext.com/api/plantuml/png/T5512i8m4BplAtBKGxyW7lJGWo2A3zYQLOf9Mhk94CINUV19Vi6ccc1R6WY4dTcPdStx-LgonSOwhO0lfH5DnIJWg91P79WQSGVH7Oq6pxJMjQeyKMvErMmE3uZKF15boRL2Fs1-CNQ5Bcs4TdHrnFPV9qARpasJiNlFbdHIHoaZ9wcwMgAbKLcIebuvkMpHDvLIAxHOO9itYZFUnZ9zzT0puV23MfTkSLcs26k1zeRdL3AOZ1owXfC2BCd8y5iV0000__y30000)

- Giải thích :
  + User:Người sử dụng hệ thống (như quản lý hoặc nhân sự), là người chịu trách nhiệm quản lý thông tin nhân viên.
  + UI: Giao diện người dùng, nơi các chức năng quản lý thông tin nhân viên được cung cấp.
  + Employee Management System:Xử lý các yêu cầu quản lý thông tin nhân viên.
  + Payroll Database:Cơ sở dữ liệu lưu trữ thông tin của tất cả nhân viên trong hệ thống.
