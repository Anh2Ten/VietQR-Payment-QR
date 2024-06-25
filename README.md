# VietQR-Payment-QR 🫶
VietQR Chậm vãi cức nên mị làm cái project này để tích hợp vào phần mềm quản lý bán hàng bên mị :>
API Tạo QR Thanh Toán VietQR cho phép bạn tạo mã QR cho các thanh toán một cách dễ dàng. 
Bạn có thể tạo mã QR thanh toán bằng cách thực hiện yêu cầu GET đến endpoint của API với các tham số cần thiết.

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

# Ví Dụ Yêu Cầu: 
curl -L -X GET "https://dailythuonghien.com/qrpay/?account=3893662005&amount=10000&info=hello world&bank=MBBank"

## Ghi Chú 📝
Api Trên Sẽ Trả Về HTTP Code 200
Và Một Chuỗi Ký Tự Bạn Hãy Đem Chuỗi Ký Tự Đó Encode Thành QR Là Xong
Cậu Có Thể Tạo QR Qua Api của bên khác hoặc tự tạo server QR CODE :


