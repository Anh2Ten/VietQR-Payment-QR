# VietQR-Payment-QR 🫶
VietQR Chậm vãi cức nên mị làm cái project này để tích hợp vào phần mềm quản lý bán hàng bên mị :>
API Tạo QR Thanh Toán VietQR cho phép bạn tạo mã QR cho các thanh toán một cách dễ dàng. 
Bạn có thể tạo mã QR thanh toán bằng cách thực hiện yêu cầu GET đến endpoint của API với các tham số cần thiết.

https://documenter.getpostman.com/view/28551106/2sA3drJFEQ

Contact If u found any bug :> https://facebook.com/anh2ten
Tui cần tìm thím nào viết cái tài liệu về api này tại tui lười zl :))

## Endpoint API
GET https://dailythuonghien.com/qrpay/

### Tham Số Yêu Cầu

- **account** (string): Số tài khoản ngân hàng nhận thanh toán.
- **amount** (int): Số tiền cần thanh toán.
- **info** (string): Thông tin bổ sung hoặc mô tả cho thanh toán.
- **bank** (string): Tên ngân hàng.
 
### Các bank khả dụng 😍
POST đến api https://dailythuonghien.com/qrpay/
api sẽ trả về các giá trị mà tham số bank có thể nhận 

bạn có thể xem bản UI tại đây: (Hiển thị các bank mà bên mình support)
https://dailythuonghien.com/qrpay/bank.php

# Ví Dụ Yêu Cầu: 
curl -L -X GET "https://dailythuonghien.com/qrpay/?account=3893662005&amount=10000&info=hello&bank=MBBank"

## Ghi Chú 📝
Api Trên Sẽ Trả Về HTTP Code 200 (Nếu code khác có nghĩa yêu cầu thất bại)
Và Một Chuỗi Ký Tự Bạn Hãy Đem Chuỗi Ký Tự Đó Encode Thành QR Là Xong
Cậu Có Thể Tạo QR Qua Api của bên khác hoặc tự tạo server QR CODE :>



Follow tui đi mấy ní ui :>
<img width="1710" alt="Ảnh màn hình 2024-06-25 lúc 11 17 22" src="https://github.com/Anh2Ten/VietQR-Payment-QR/assets/83670932/1c710e20-0a48-4eaa-9515-0117cb7bde28">
