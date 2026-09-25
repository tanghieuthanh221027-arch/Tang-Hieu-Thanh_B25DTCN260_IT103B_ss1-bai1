1 Phân tích kĩ thuật
- Dữ liệu input :
const customerName = "Nguyen Thi Mai"; : Tên khách hàng
const foodItemName = "Com Tam Suon Bi Cha"; : Tên món ăn
const rawFoodPrice = "55000"; : Giá món ăn (dạng string)
const rawToppingPrice = "15000"; : Giá topping (dạng string)
const rawDeliveryFee = "20000"; : Phí giao hàng (dạng string)
const voucherDiscount = 10000; : Tiền giảm giá

- Vấn đề cần xử lí : khi muốn tính tiền : const foodTotal = Number(rawFoodPrice) + Number(rawToppingPrice);
-> kết quả không đúng kiểu dữ liệu
- Cách xử lí :
-> nên ép kiểu về dạng sô để tính toán được (dùng Number() hoặc parseInt())
- Kết quả : 
Khách hàng: Nguyen Thi Mai
Món ăn: Com Tam Suon Bi Cha
Tổng tiền món ăn: 70000 VND
Số tiền thanh toán thực tế: 80000 VND

- testcase 1 : Giữ nguyên input
-> Kết quả :
Khách hàng: Nguyen Thi Mai
Món ăn: Com Tam Suon Bi Cha
Tổng tiền món ăn: 70000 VND
Số tiền thanh toán thực tế: 80000 VND

- test case 2 : Thay giá món ăn : const rawFoodPrice = "60000";
-> Kết quả :
Khách hàng: Nguyen Thi Mai
Món ăn: Com Tam Suon Bi Cha
Tổng tiền món ăn: 75000 VND
Số tiền thanh toán thực tế: 85000 VND

- testcase 3 : Thay giá topping : const rawToppingPrice = "20000";
-> Kết quả : 
Khách hàng: Nguyen Thi Mai
Món ăn: Com Tam Suon Bi Cha
Tổng tiền món ăn: 75000 VND
Số tiền thanh toán thực tế: 85000 VND

- testcase 4 : Thay giá vận chuyển : const rawDeliveryFee = "30000";
-> Kết quả : 
Khách hàng: Nguyen Thi Mai
Món ăn: Com Tam Suon Bi Cha
Tổng tiền món ăn: 70000 VND
Số tiền thanh toán thực tế: 90000 VND

-> Các testcase đều pass 