---
title: "Câu điều kiện if–else & switch trong Java — Hiểu là dùng được ngay"
date: 2025-01-05
---

## Giới thiệu

Trong lập trình, rất nhiều khi bạn cần:

✔ kiểm tra điều kiện  
✔ phân nhánh xử lý  
✔ chạy đoạn code khác nhau tuỳ tình huống  

Khi đó, bạn sẽ dùng **if — else — switch**.

Bài này sẽ giúp bạn hiểu và dùng được **câu điều kiện trong Java** một cách đơn giản nhất.

---

## if — else là gì?

`if` dùng để **kiểm tra điều kiện**.  
Nếu điều kiện đúng → chạy đoạn code bên trong.

Ví dụ:

```java
int age = 18;

if (age >= 18) {
    System.out.println("Bạn đã đủ 18 tuổi");
}
```
Nếu điều kiện sai → Java bỏ qua.

## if — else
Khi bạn muốn xử lý thêm trường hợp ngược lại, dùng else
```
int age = 16;

if (age >= 18) {
    System.out.println("Đủ tuổi");
} else {
    System.out.println("Chưa đủ tuổi");
}
```
🟢 Output:
Chưa đủ tuổi

## if — else if — else
```
Dùng khi có nhiều điều kiện.
int score = 85;

if (score >= 90) {
    System.out.println("Xuất sắc");
} else if (score >= 75) {
    System.out.println("Khá");
} else if (score >= 50) {
    System.out.println("Trung bình");
} else {
    System.out.println("Yếu");
}
```
👉 Java sẽ kiểm tra từ trên xuống.
Gặp điều kiện đúng → dừng lạ

## Lưu ý quan trọng

✔ Điều kiện trong if phải là boolean

✔ Dùng == để so sánh — đừng nhầm với =

Ví dụ đúng:
```
if (a == 5) { }
```

Ví dụ sai:
```
if (a = 5) { }   // lỗi!
```

## Toán tử logic đi kèm if
Toán tử	Ý nghĩa
&&	Và (cả 2 đều đúng)
	
! Phủ định

```
int age = 20;
boolean isStudent = true;

if (age < 25 && isStudent) {
    System.out.println("Giảm giá sinh viên");
}
```

## switch — khi có nhiều lựa chọn cố định
switch phù hợp khi bạn có các giá trị cụ thể như số, ký tự, chuỗi.

Ví dụ:
```
int day = 3;

switch (day) {
    case 1:
        System.out.println("Thứ hai");
        break;
    case 2:
        System.out.println("Thứ ba");
        break;
    case 3:
        System.out.println("Thứ tư");
        break;
    default:
        System.out.println("Ngày không hợp lệ");
}
```
🟢 Output:
```
Thứ tư
```

## Vì sao cần break?
✔ break giúp thoát khỏi switch
Nếu quên break, chương trình sẽ chạy tiếp các case phía dưới.


## switch với String
Java cho phép dùng String trong switch:
```
String role = "admin";

switch (role) {
    case "admin":
        System.out.println("Quản trị viên");
        break;
    case "user":
        System.out.println("Người dùng");
        break;
    default:
        System.out.println("Không xác định");
}
```

## Khi nào dùng if — khi nào dùng switch?

| Trường hợp | Nên dùng |
|-----------|----------|
| Điều kiện phức tạp, nhiều phép so sánh | if — else |
| So sánh giá trị cố định (1, 2, 3… “A”, “B”) | switch |
| Có phạm vi giá trị (>=, <=, <, >) | if — else |


Ví dụ thực tế tổng hợp
```
int age = 22;
boolean hasTicket = true;

if (age >= 18 && hasTicket) {
    System.out.println("Bạn được vào cửa");
} else {
    System.out.println("Không đủ điều kiện");
}
```

Những lỗi người mới thường gặp
❌ Quên dấu { }

❌ Nhầm = với ==

❌ Quên break trong switch

❌ Điều kiện không phải boolean

## Kết luận

Qua bài này, bạn đã hiểu:

✔ Câu lệnh if — else

✔ else if cho nhiều điều kiện

✔ switch và break

✔ Khi nào dùng if, khi nào dùng switch




