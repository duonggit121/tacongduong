---
title: "Mảng (Array) trong Java — Hiểu nhanh cho người mới"
date: 2025-01-07
---

## Giới thiệu

Khi lập trình, nhiều lúc bạn cần lưu **nhiều giá trị cùng loại** — ví dụ danh sách điểm, danh sách tuổi, danh sách sinh viên…

Nếu dùng từng biến riêng lẻ thì sẽ rất rối:
```
int a = 5;
int b = 7;
int c = 9;
```

👉 Lúc này **mảng (Array)** ra đời để giúp bạn lưu trữ dữ liệu một cách gọn gàng.

---

## Mảng trong Java là gì?

**Mảng là một tập hợp các phần tử cùng kiểu dữ liệu, được lưu liên tiếp trong bộ nhớ.**

Ví dụ mảng số nguyên:
```
int[] numbers = {1, 2, 3, 4, 5};
```


Trong đó:

| Thành phần | Ý nghĩa |
|-----------|---------|
| int | kiểu dữ liệu |
| [] | khai báo mảng |
| numbers | tên mảng |
| {1,2,3,4,5} | giá trị trong mảng |

📌 Lưu ý:  
👉 Các phần tử trong mảng **được đánh số từ 0**

| Vị trí (index) | Giá trị |
|---|---|
| 0 | 1 |
| 1 | 2 |
| 2 | 3 |
| 3 | 4 |
| 4 | 5 |

---

## Khai báo mảng trong Java

Có 2 cách phổ biến:

### 🟢 Cách 1 — Khai báo & gán luôn giá trị
```
int[] numbers = {10, 20, 30};
```

### 🟣 Cách 2 — Khai báo trước, gán sau
```
int[] numbers = new int[3];
numbers[0] = 10;
numbers[1] = 20;
numbers[2] = 30;
```
👉 `new int[3]` nghĩa là mảng có **3 phần tử**

---

## Truy cập phần tử trong mảng

Bạn dùng **index (chỉ số)**:
```
System.out.println(numbers[0]); // in phần tử đầu
System.out.println(numbers[2]); // in phần tử thứ 3
```
⚠️ Nếu truy cập sai index:
```
numbers[10];
```
Java sẽ báo lỗi **ArrayIndexOutOfBoundsException**

---

## Duyệt mảng bằng vòng lặp

### 🔁 for
```
for (int i = 0; i < numbers.length; i++) {
System.out.println(numbers[i]);
}
```
📌 `numbers.length` = số phần tử mảng

---

### 🔁 for–each (cách viết gọn hơn)
```
for (int n : numbers) {
System.out.println(n);
}
```

👉 Cách này dễ đọc — rất hay dùng!

---

## Mảng String

Không chỉ số nhé 😄  
Bạn có thể tạo mảng chuỗi:
```
String[] names = {"An", "Bình", "Lan"};
```
Duyệt:
```
for (String name : names) {
System.out.println(name);
}
```

---

## Khi nào nên dùng mảng?

✔ Khi số phần tử **biết trước**  
✔ Khi các phần tử **cùng kiểu dữ liệu**  
✔ Khi cần lưu trữ cố định

Ví dụ phù hợp:

🟢 Danh sách điểm của 1 lớp  
🟢 Danh sách số nguyên tử trong bảng tuần hoàn  
🟢 Danh sách ngày trong tuần  

---

## Hạn chế của mảng

❌ Kích thước **không thay đổi được sau khi tạo**

Muốn linh hoạt hơn → sau này bạn sẽ học:

✔ `ArrayList`  
✔ `List`  
✔ `Map`  
✔ `Set`

---

## Kết luận

Trong bài này bạn đã hiểu:

✔ Mảng là gì  

✔ Cách khai báo & truy cập phần tử  

✔ Duyệt mảng bằng for & for–each  

✔ Mảng nhiều chiều  

✔ Khi nào nên dùng mảng  

👉 Đây là bước quan trọng trước khi qua **Collection & OOP nâng cao**.

---








