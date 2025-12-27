---
title: "Biến, kiểu dữ liệu & toán tử trong Java — Nền tảng cho người mới"
date: 2025-01-04
---

## Giới thiệu

Sau khi bạn đã cài đặt Java và chạy được chương trình đầu tiên, bước tiếp theo rất quan trọng là:

> Hiểu biến, kiểu dữ liệu và toán tử trong Java.

Đây là **kiến thức nền tảng** — nếu hiểu vững, bạn sẽ học tiếp OOP, Collections, Spring Boot dễ hơn rất nhiều.

---

## Biến trong Java là gì?

**Biến (variable)** là “cái hộp” dùng để chứa dữ liệu trong chương trình.

Cú pháp khai báo biến:

```java
kiểu_dữ_liệu tên_biến = giá_trị;
```

Ví dụ:
```
int age = 20;
String name = "An";
double score = 8.5;
```
👉 Java bắt buộc phải khai báo kiểu dữ liệu trước — đây gọi là ngôn ngữ kiểu tĩnh.

## Các kiểu dữ liệu cơ bản trong Java

Java có 2 nhóm lớn:
🟣 1 — Kiểu nguyên thuỷ (Primitive Types)
| Tiêu chí | Java | JavaScript |
|---------|------|-------------|
| Các kiểu nguyên thuỷ | `byte`, `short`, `int`, `long`, `float`, `double`, `char`, `boolean` | `number`, `bigint`, `string`, `boolean`, `undefined`, `symbol`, `null` |
| Kiểu số | Tách ra: số nguyên & số thực (`int`, `double`...) | Chỉ có `number` (bao gồm cả số nguyên & số thực) + `bigint` |
| Chuỗi ký tự | Không phải kiểu nguyên thuỷ (`String` là object) | `string` là kiểu nguyên thuỷ |
| null / undefined | `null` (đại diện giá trị rỗng) | `null` và `undefined` là 2 khái niệm khác nhau |
| boolean | `true` / `false` | `true` / `false` |
| Ký tự | `char` (chỉ 1 ký tự) | Không có `char`, dùng `string` |

Ví dụ:
```
int year = 2025;
double price = 9.99;
boolean isJavaFun = true;
char grade = 'A';
```

🟢 2 — Kiểu tham chiếu (Reference Types)
Phổ biến nhất là:
```
String name = "Java";
```
Khác với C/C++, trong Java:
👉 String là một kiểu đối tượng (class)

## Quy tắc đặt tên biến trong Java
Bạn nên nhớ:
✔ Bắt đầu bằng chữ / _ / $

❌ Không bắt đầu bằng số

✔ Có phân biệt hoa — thường

✔ Nên dùng camelCase

Ví dụ đúng:
```
int studentAge;
String fullName;
boolean isOnline;
```
Ví dụ sai:
```
int 1age;       // sai
int class;      // sai vì class là từ khóa
```

## Toán tử trong Java
Toán tử (operator) là các ký hiệu dùng để thực hiện phép tính hoặc xử lý logic.
Java có 3 nhóm chính:
🔹 1 — Toán tử số học
Dùng cho phép tính cơ bản

🔹 2 — Toán tử so sánh
Dùng để so sánh hai giá trị

🔹 3 — Toán tử logic
Dùng cho biểu thức điều kiện

## Ép kiểu dữ liệu (Casting)
Đôi khi bạn cần chuyển kiểu dữ liệu.

🔹 Ép kiểu tự động (nhỏ → lớn)
```
int a = 10;
double b = a;   // OK
```
🔹 Ép kiểu tường minh (lớn → nhỏ)
```
double x = 9.8;
int y = (int) x;   // y = 9
```
👉 Nếu không ép kiểu sẽ bị lỗi.

Những lỗi người mới hay gặp

❌ Quên dấu ;

❌ Sai kiểu dữ liệu

❌ Nhầm = và ==

❌ Đặt tên biến sai quy tắc

Ví dụ sai:
```
if (a = 5) { }   // sai
```


Ví dụ đúng:
```
if (a == 5) { }
```

## Kết luận

Trong bài này, bạn đã nắm được:

✔ Biến là gì

✔ Các kiểu dữ liệu trong Java

✔ Quy tắc đặt tên biến

✔ Hằng số với final

✔ Các toán tử cơ bản

✔ Cách ép kiểu dữ liệu






