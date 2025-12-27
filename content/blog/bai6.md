---
title: "Vòng lặp trong Java — for, while, do-while giải thích dễ hiểu"
date: 2025-01-06
---

## Giới thiệu

Trong lập trình, sẽ có lúc bạn cần **lặp đi lặp lại một công việc** — ví dụ:

✔ In 10 lần câu “Xin chào”  
✔ Duyệt danh sách học sinh  
✔ Tính tổng từ 1 → 100  

Nếu không dùng vòng lặp, bạn sẽ phải viết code lặp lại rất dài và xấu 😅  
Vì vậy, Java cung cấp 3 loại vòng lặp chính:

👉 `for`  
👉 `while`  
👉 `do…while`  

---

## Vòng lặp for

Dùng khi **biết trước số lần lặp**.

```java
for (int i = 1; i <= 5; i++) {
    System.out.println("Lần thứ: " + i);
}
```

🔍 Giải thích:
| Phần       | Ý nghĩa                  |
|------------|--------------------------|
| int i = 1  | Giá trị bắt đầu          |
| i <= 5     | Điều kiện tiếp tục lặp   |
| i++        | Mỗi lần tăng 1           |

👉 Kết quả:
```
Lần thứ: 1
Lần thứ: 2
Lần thứ: 3
Lần thứ: 4
Lần thứ: 5
```

## Vòng lặp while
Dùng khi chưa biết trước số lần lặp, chỉ biết điều kiện tiếp tục.
```
int i = 1;

while (i <= 5) {
    System.out.println(i);
    i++;
}
```
⚠️ Nếu quên tăng i++ → vòng lặp vô hạn 😨

## Vòng lặp do — while
Khác biệt lớn nhất:
👉 Luôn chạy ít nhất 1 lần, dù điều kiện sai.
```
int x = 10;

do {
    System.out.println("Xin chào");
    x++;
} while (x < 5);
```
👉 Dù x < 5 sai, chương trình vẫn in 1 lần.

So sánh nhanh
| Loại vòng lặp | Dùng khi nào?                 |
|---------------|-------------------------------|
| for           | Biết trước số lần lặp         |
| while         | Lặp theo điều kiện chưa biết trước |
| do–while      | Muốn chạy ít nhất 1 lần       |


## break và continue trong vòng lặp
🔴 break — dừng hẳn vòng lặp
```
for (int i = 1; i <= 5; i++) {
    if (i == 3) break;
    System.out.println(i);
}
```
👉 Chỉ in: 1 2

🟡 continue — bỏ qua lần lặp hiện tại
```
for (int i = 1; i <= 5; i++) {
    if (i == 3) continue;
    System.out.println(i);
}
```
👉 In: 1 2 4 5

Ví dụ thực tế — tính tổng từ 1 đến 10
```
int sum = 0;

for (int i = 1; i <= 10; i++) {
    sum += i;
}

System.out.println("Tổng = " + sum);
```
👉 Kết quả: Tổng = 55


## Kết luận
Qua bài này bạn đã hiểu:

✔ 3 loại vòng lặp trong Java

✔ Khi nào dùng for, while, do-while

✔ Cách dùng break & continue







