---
title: "JavaScript là gì? Cách chạy JavaScript đơn giản cho người mới"
date: 2025-01-09
---



##  Giới thiệu

Nếu Java phổ biến ở backend và Android, thì **JavaScript** lại là “linh hồn của web hiện đại”.

Bạn nhìn thấy:

✔ Nút bấm động  
✔ Popup  
✔ Hiệu ứng trang web  
✔ Ứng dụng web như Gmail, Facebook  

👉 Rất nhiều trong đó chạy bằng **JavaScript (JS)**.

Trong bài này, bạn sẽ hiểu **JavaScript là gì và chạy như thế nào — thật đơn giản**.

---

##  JavaScript là gì?

**JavaScript là ngôn ngữ lập trình dùng để tạo các tính năng động trên website.**

JavaScript có thể chạy ở:

✔ Trình duyệt (Chrome, Edge, Firefox…)  
✔ Backend (runtime Node.js)  

📌 Lưu ý quan trọng:

❌ JavaScript **không phải** Java  
✔ Chúng là hai ngôn ngữ khác nhau hoàn toàn

---

##  JavaScript chạy ở đâu?

Trình duyệt web đã tích hợp sẵn **JavaScript Engine**.

Ví dụ:

| Trình duyệt | Engine |
|------------|--------|
| Chrome | V8 |
| Firefox | SpiderMonkey |
| Safari | JavaScriptCore |

👉 Vì vậy bạn **không cần cài thêm gì để chạy JS trên trình duyệt**.

---

##  Chạy JavaScript trực tiếp trên trình duyệt

### 🔹 Cách 1 — Mở Console

1️⃣ Mở trang web  
2️⃣ Nhấn:

- **F12** hoặc  
- **Ctrl + Shift + I**  

3️⃣ Chọn tab **Console**  
4️⃣ Gõ:

```javascript
console.log("Xin chào JavaScript!");
```

Kết quả xuất hiện ngay 👇

---

##  Chạy JavaScript trong file HTML

Tạo file `index.html`:

```html
<!DOCTYPE html>
<html>
<head>
  <title>Demo JS</title>
</head>
<body>
  <h1>Xin chào!</h1>

  <script>
    console.log("JavaScript đang chạy!");
  </script>
</body>
</html>
```

👉 Mở file bằng trình duyệt để chạy

---

##  Cú pháp cơ bản JavaScript

### 🔹 Khai báo biến

```javascript
let name = "An";
const age = 20;
var city = "Hanoi";
```

📌 Khuyến nghị:

✔ Dùng `let` và `const`  
❌ Hạn chế `var`

---

### 🔹 In ra màn hình console

```javascript
console.log("Hello JS");
```

---

### 🔹 Hàm đơn giản

```javascript
function sayHello() {
  console.log("Xin chào!");
}

sayHello();
```

---

##  Java vs JavaScript — khác nhau không?

| Tiêu chí | Java | JavaScript |
|--------|------|-----------|
| Loại ngôn ngữ | Biên dịch & chạy trên JVM | Thông dịch (runtime JS) |
| Dùng cho | Backend, Android, doanh nghiệp | Web & ứng dụng web |
| Kiểu dữ liệu | Chặt chẽ | Linh hoạt |
| Cú pháp | Nghiêm ngặt | Dễ viết hơn |

👉 **Tên giống nhau nhưng bản chất khác nhau hoàn toàn**

---

##  Tổng kết nhanh

| Nội dung | Ghi nhớ |
|--------|--------|
| JavaScript là gì? | Ngôn ngữ lập trình web động |
| Chạy ở đâu? | Trình duyệt & Node.js |
| Console | Dùng `console.log()` |
| Mục đích | Tạo tương tác trên web |

---

##  Kết luận

JavaScript là nền tảng của web hiện đại.  
Nếu bạn muốn:

✔ Làm website  
✔ Làm frontend  
✔ Làm full-stack  

👉 Thì JavaScript **là kỹ năng bắt buộc phải biết**.

Ở các bài tiếp theo, chúng ta sẽ cùng tìm hiểu:

🔹 Biến  
🔹 Hàm  
🔹 Cấu trúc điều kiện  
🔹 DOM  
🔹 ES6  

…theo cách **dễ hiểu — học tới đâu nắm chắc tới đó** 🚀
