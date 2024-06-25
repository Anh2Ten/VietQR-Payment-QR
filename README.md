# VietQR-Payment-QR
VietQR Chậm vãi cức nên mị làm cái project này để tích hợp vào phần mềm quản lý bán hàng bên mị :>

API Tạo QR Thanh Toán VietQR
API Tạo QR Thanh Toán VietQR cho phép bạn tạo mã QR cho các thanh toán một cách dễ dàng. 
Bạn có thể tạo mã QR thanh toán bằng cách thực hiện yêu cầu GET đến endpoint của API với các tham số cần thiết.

## Endpoint API
GET https://dailythuonghien.com/qr/


# Ví Dụ Yêu Cầu: 
curl -X GET "https://dailythuonghien.com/qr/?account=3893662005&amount=0&info=hello%20world&bank=MBBank"


### Tham Số Yêu Cầu

- **account** (string): Số tài khoản ngân hàng nhận thanh toán.
- **amount** (int): Số tiền cần thanh toán.
- **info** (string): Thông tin bổ sung hoặc mô tả cho thanh toán.
- **bank** (string): Tên ngân hàng.
 

## Kết Quả 
Api Trên Sẽ Trả Về HTTP Code 200
Và Một Chuỗi Ký Tự Bạn Hãy Đem Chuỗi Ký Tự Đó Encode Thành QR Là Xong
Cậu Có Thể Tạo QR Qua Api của chúng tớ thông qua:

https://api.dailythuonghien.com/qr/?qr= (Chuỗi Ký Tự Mà Api Trả Về)




----------------------------------------------------------------------------------
Tham Số	Kiểu	Mô Tả
account	string	Số tài khoản nhận thanh toán. Đây phải là số tài khoản hợp lệ.
amount	int	Số tiền cần chuyển. Đây phải là giá trị số nguyên.
info	string	Thông tin bổ sung cho giao dịch, có thể bao gồm mục đích thanh toán.
bank	string	Tên ngân hàng nơi tài khoản được mở. Đây phải là tên ngân hàng được công nhận.
