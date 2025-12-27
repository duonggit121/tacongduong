---
title: "Mảng (Array) trong Java — Hiểu là dùng được ngay"
date: 2025-01-08
---


## Giới thiệu

Trong lập trình, đôi khi bạn cần lưu **nhiều giá trị cùng loại**  
Ví dụ:

✔ danh sách điểm  
✔ danh sách tên sinh viên  
✔ danh sách số điện thoại  

Nếu dùng biến riêng lẻ:

```java
int a = 5;
int b = 7;
int c = 9;
```

👉 Rất bất tiện!

Vì vậy Java cung cấp **Array (Mảng)**.

---

##  Mảng là gì?

**Mảng là một tập hợp nhiều phần tử có cùng kiểu dữ liệu.**

Ví dụ:

```java
int[] numbers = {1, 2, 3, 4, 5};
```

Ở đây:

✔ `int` → kiểu dữ liệu  
✔ `[]` → đánh dấu mảng  
✔ `{1,2,3,4,5}` → danh sách giá trị  

---

##  Khai báo mảng trong Java

Có 2 cách phổ biến:

### 🔹 Cách 1 — Khai báo & gán giá trị luôn

```java
String[] names = {"An", "Bình", "Chi"};
```

### 🔹 Cách 2 — Khai báo trước, gán sau

```java
int[] a = new int[3];

a[0] = 10;
a[1] = 20;
a[2] = 30;
```

👉 `new int[3]` nghĩa là mảng có **3 phần tử**

---

##  Truy cập phần tử mảng

Chỉ số (index) trong Java:

🟣 Bắt đầu từ **0**

Ví dụ:

```java
int[] nums = {5, 10, 15};

System.out.println(nums[0]); // 5
System.out.println(nums[1]); // 10
System.out.println(nums[2]); // 15
```

❌ Nếu truy cập sai index:

```java
nums[3];
```

👉 Sẽ bị lỗi **ArrayIndexOutOfBoundsException**

---

##  Duyệt mảng bằng vòng lặp

### 🔹 for thường

```java
int[] a = {1, 2, 3};

for (int i = 0; i < a.length; i++) {
    System.out.println(a[i]);
}
```

### 🔹 for–each (ngắn gọn hơn)

```java
for (int value : a) {
    System.out.println(value);
}
```

---

##  Độ dài mảng

Dùng thuộc tính:

```java
a.length
```

Ví dụ:

```java
System.out.println(a.length);
```

---

##  Mảng chỉ có kích thước cố định

Sau khi tạo:

```java
int[] arr = new int[5];
```

👉 bạn **không thể tăng/giảm số phần tử**

Nếu cần linh hoạt → dùng:

✔ `ArrayList` (sẽ học ở phần sau)

---

##  Tổng kết nhanh

| Khái niệm | Ý nghĩa |
|----------|--------|
| Mảng | Chứa nhiều giá trị cùng kiểu |
| Index | Bắt đầu từ 0 |
| length | Độ dài mảng |
| Kích thước | Cố định sau khi tạo |

---

##  Kết luận

Mảng là nền tảng quan trọng trong Java giúp bạn:

✔ Lưu trữ dữ liệu nhiều phần tử  
✔ Duyệt dữ liệu bằng vòng lặp  
✔ Xử lý danh sách hiệu quả  

👉 Hiểu vững mảng = Bạn đã tiến thêm 1 bước lớn trong Java 🚀
