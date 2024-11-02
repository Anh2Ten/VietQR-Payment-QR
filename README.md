# VietQR-Payment-QR 🫶
## Cậu Nên Sử Dụng IP Việt Nam Để Tránh Hệ Thống Của Chúng Tớ Block Nhé
API Tạo QR Thanh Toán VietQR cho phép cậu tạo mã QR cho các thanh toán một cách dễ dàng. 
Cậu có thể tạo mã QR thanh toán bằng cách thực hiện yêu cầu GET đến endpoint của API với các tham số cần thiết.
 
If You Found Any Issue Contact Facebook: @Anh2Ten
Only Support Api Issue Thanks 🫶🏻

# Ví Dụ Yêu Cầu: 
curl -L -X GET "https://api.quanlybanhang.store/qrpay/?account=3893662005&amount=10000&info=hello&bank=MBBank"

### Tham Số Yêu Cầu

- **account** (string): Số tài khoản ngân hàng nhận thanh toán.
- **amount** (int): Số tiền cần thanh toán.
- **info** (string): Thông tin bổ sung hoặc mô tả cho thanh toán.
- **bank** (string): Tên ngân hàng.
 
### Các bank khả dụng 😍
POST đến api https://api.quanlybanhang.store/qrpay/
api sẽ trả về các giá trị mà tham số bank có thể nhận 
dưới đây là mẫu các bank:
["VietinBank","Vietcombank","BIDV","Agribank","OCB","MBBank","Techcombank","ACB","VPBank","TPBank","Sacombank","HDBank","VietCapitalBank","SCB","VIB","SHB","Eximbank","MSB","CAKE","Ubank","Timo","ViettelMoney","VNPTMoney","SaigonBank","BacABank","PVcomBank","Oceanbank","NCB","ShinhanBank","ABBANK","VietABank","NamABank","PGBank","VietBank","BaoVietBank","SeABank","COOPBANK","LienVietPostBank","KienLongBank","KBank","KookminHN","KEBHanaHCM","KEBHANAHN","MAFC","Citibank","KookminHCM","VBSP","Woori","VRB","UnitedOverseas","StandardChartered","PublicBank","Nonghyup","IndovinaBank","IBKHCM","IBKHN","HSBC","HongLeong","GPBank","DongABank","DBSBank","CIMB","CBBank"]

## Ghi Chú 📝
Api Trên Sẽ Trả Về HTTP Code 200 
Nếu status code khác có nghĩa yêu cầu thất bại
kiểm tra kỹ các tham số !

api sẽ trả về một string, encode string đó thành qrcode là xong


Follow tui đi mấy ní ui :>
<img width="1710" alt="Ảnh màn hình 2024-06-25 lúc 11 17 22" src="https://github.com/Anh2Ten/VietQR-Payment-QR/assets/83670932/1c710e20-0a48-4eaa-9515-0117cb7bde28">
