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
# Phân tích ca sử dụng Maintain Purchase Order
- Các thành phần chính
+ User
+ UI
+ PurchaseOrderManager
+ PayrollDatabase
- Biểu đồ sequence cho ca sử dụng Maintain Purchase Order:
![](https://www.planttext.com/api/plantuml/png/b98nIyD05CVt-nIFJZgKxXsaWw0THA4jT7sz7hrWSgsNYz1H71oSd5mD8aAXW-YKGpgS-3tk4_WLV4c89XP1CmJUo-___l_to8VTz6A3sYHHo92RkOPHB3HRK2lWmGALWTQetmACOTHlje_rL6WuGeKp4Gdg39Qn4L715j_AkYawIJIN68kIW7qqEA6o45K5Ota6QE-H9NHXADqgwWoyNMDdx9uHtcxUKmNItQaPH0aoeeYjMPBeWF00bcwL0FVPOm9dYS_k5OJkjQvdTHKDgI8Kjju-SP21jrSAZCGv69TosFcPPvSn30tn5M7oqHAuUo43eEThQdihvr1JB3ZtzW9EVROnPSxj4OsSrMN6kPkIFblN0svfo_iKD-t28UrpcUFUNkSeGJ1nwRmf4o6bhM_aimS34v-bmJys2hsz3NwFFwovVwD_IrloGaqPwz4x_tq_0G00__y30000)

- Biểu đồ lớp phân tích cho ca sử dụng Maintain Purchase Order:
![](https://www.planttext.com/api/plantuml/png/T5513i8W4Bpp2evww0TwC3ruwS5eD3vWMrPjKcXb5vF6-38FFial2DGs6YidTXXcXk5vVsJ4ODdfMfGr4CazePLN8UFIOE286sVB4n2khK8xcukR6BZvo5GLjJLqaPARG-Df_G6vGbSSyIsU7H9_AaHy5Lqq6jvrnAX7KL1gyEm1rofW_COKriY_sRv2Bu6XyCEeJ731lzA1FIN_nhr5B2b95g61L5Q6qKB99FmOqEbNfPBGA9Ashq5CiyBzwUofLCEsQRqXLuqX8J8l6hxl1G00__y30000)

- Giải thích:
+ User: Đại diện cho người dùng của hệ thống, thường là nhân viên hoặc quản lý mua hàng.

+ managePurchaseOrder(): Phương thức để quản lý đơn hàng mua, như thêm, sửa, hoặc xóa đơn hàng.
UI (User Interface): Giao diện người dùng cho phép User tương tác với hệ thống.

+ displayOrderInfo(): Phương thức để hiển thị thông tin đơn hàng.
submitOrderRequest(): Phương thức để gửi yêu cầu quản lý đơn hàng (thêm, sửa, xóa) đến hệ thống.
Order Management System: Hệ thống quản lý đơn hàng chịu trách nhiệm xử lý các yêu cầu từ UI.

+ addOrder(): Phương thức để thêm đơn hàng mới.
updateOrder(): Phương thức để cập nhật thông tin của đơn hàng.
deleteOrder(): Phương thức để xóa đơn hàng.
Purchase Order Database: Cơ sở dữ liệu chứa thông tin của tất cả đơn hàng mua.

+ saveOrder(): Phương thức để lưu đơn hàng mới vào cơ sở dữ liệu.
updateOrderData(): Phương thức để cập nhật thông tin của đơn hàng trong cơ sở dữ liệu.
deleteOrderData(): Phương thức để xóa đơn hàng khỏi cơ sở dữ liệu.

# Phân tích ca sử dụng Run Payroll
- Biểu đồ sequence cho ca sử dụng Run Payroll
![](https://www.planttext.com/api/plantuml/png/Z5E_IiD06D_p51-T5DeNw2057ImeE5ZGyNg6N6ZyKYztXOpYwEGJs5X4g1GwE2L3XvEynps1h-1TD7gfjNG9nyVlt_tkoqUnwYM2S26l8uzG4NCO93xtncOKqd1CK41hq6y1IM3GRuxFIChZA3ebI0AVLv3cQ2FyY0Wo98dlukkPvrbpw1mOB-Z2fPfBe3f_aI3K0Xc8M6K8GvtFC82eN9OP1fw16aBJsP0FcKnrSOUGhglKn3NAhqWTnwYSwFmv1S7Kct4K8G8ozOGm2TNSVDLqNUo7sjcKwPoRw33HnUqkaly7T1ITNhvvi5SVQ9bzbTKsTkLI5uyOsAFK-QeDL6KKHYos011S5w_xMopTJigbTFCttmFU7zJCVQ_TghcmQP3fV55Tf3AO6WbgRVxcgbV4QNHaRYNWHjh1nXMfTgiBns6r5eBfuduRoUlvU6L_Yqy0003__mC0)

- Biểu đồ lớp cho ca sử dụng Run Payroll
![](https://www.planttext.com/api/plantuml/png/R90x3i8m44Hxdy8b515z2fG22WeaXCG1bcGLMTfyyAuZHOYJKN0ahe2T7r4KTzutdfdrz_r9MC2AAqYb1CpwncZrK-dkM5TUeBKLqMQhNcgKd2O1be9sa1nGm11xPSyompL1Ez0hiYEPsmpW32NaiymKA7K4Wl_a7Z0qkD9cJ0U1Ep1EFZdAiQYfQX43MxCPvjwgspgAzc6tM9km5QJ2ob_3T54rrenbnjhYmo6BMk3PYwbLxCLY3JR8kz20TUQHKeat2f__0m00__y30000)
- Giải thích:
+ User:Người dùng có quyền truy cập vào hệ thống,người này thực hiện thao tác tính toán bảng lương.
+ UI:Giao diện để người dùng nhập và xem thông tin liên quan đến bảng lương, bao gồm các thông tin về nhân viên, số giờ làm việc, và các khoản trừ khác.
+ PayrollManager:Lớp này chịu trách nhiệm thực hiện tính toán lương cho tất cả nhân viên, bao gồm các khoản lương cơ bản, thưởng, thuế, và các khoản trừ.
+ PayrollDatabase:Lưu trữ thông tin về các nhân viên, lương của họ, các khoản thưởng, khoản trừ, cũng như các giao dịch đã được xử lý trong hệ thống.

# Phân tích ca sử dụng Select Payment Method
- Biểu đồ sequence cho ca sử dụng Select Payment Method
![](https://www.planttext.com/api/plantuml/png/f9F1IiD048Rl-nH3xts17gHGGGiA7WnuNTVGBCPft6o47CM31_7W6nYAY4AX1q-RGmyhUOzz0b-XayJGfjPQy9BD3lzyyyzayfNF-x7cIYTN8UD2ZnLuiQzOH24fPCHHGySRTe37u0tRuHEUgd4O7dFa8rzLadPeetoVQtxEOtzLtyGOAuj3TuzgGGy6WSiV4QAWc1KPZa3J_KtGmJ40FROPCjAHkbsMCWzSFfMGslS4X3ElzFmRjGPPOXjtn3rovYMbBFjHCkHM80JIvVS8sfbCidLMTvFjK-NC16vSVhjZ3VQxwoLruCmq0WpeqF-VG35BjdRz-MGdt-FUhUapcudQ7K9OqgdrPyA9SW0_6soMOtLMz5gxiPbifzVxKMrL3mxfWznXPVe1BfsPQxXEYC9OtyUByWzO0000__y30000)

- Biểu đồ lớp cho ca sử dụng Select Payment Method
![](https://www.planttext.com/api/plantuml/png/T94x3i8m44Hxdy8b515z2fI2XY822N60JR8Abcp7U3T84U9a51o9A-1y5IN2dJtZD-Frz_r9YC5pRRJ8DH39Aw6NJo6xHQWnvpCq1YsdoBUgs6p5IupUu-Gi53aDpM0zELQLfU0TE7LcrCYvTD2Wpr51yvNMALWePmLANANtGkqAOFpRRC0TW243meddaRt2n-hYK1FMIa1s8ucYVVlUM2hBw25d4c7RdYwgns5gjY3fUf0q7Iaatsia5Wlt332LZQUQj6ihBLb2926X_R8V0000__y30000)
- Giải thích: User:
+ Người dùng có quyền truy cập vào hệ thống, người này thực hiện việc chọn phương thức thanh toán cho bản thân hoặc cho nhân viên.
+ UI:Giao diện để người dùng chọn phương thức thanh toán (chẳng hạn như chuyển khoản ngân hàng, tiền mặt, séc, v.v.) và hiển thị các tùy chọn phương thức thanh toán cho người dùng.
+ PaymentMethodManager:Lớp này chịu trách nhiệm xử lý lựa chọn phương thức thanh toán của người dùng. Nó sẽ lưu trữ và cập nhật thông tin phương thức thanh toán đã chọn vào hệ thống.
+ PayrollDatabase:Cơ sở dữ liệu lưu trữ thông tin của người dùng, bao gồm các phương thức thanh toán đã chọn và các thông tin liên quan đến tiền lương.
