---
title: "Cài đặt Java & viết chương trình đầu tiên — Hướng dẫn cho người mới"
date: 2025-01-03
---

![Java programming](https://upload.wikimedia.org/wikipedia/en/3/30/Java_programming_language_logo.svg)

## Giới thiệu

Nếu bạn là người mới và vừa nghe tới Java, chắc hẳn bạn sẽ tự hỏi:

> Làm sao để cài Java và chạy chương trình đầu tiên?

Đừng lo 😊  
Bài viết này sẽ hướng dẫn bạn **từng bước — đơn giản — dễ làm theo**.

---

## Bước 1 — Cài Java Development Kit (JDK)

👉 Java muốn chạy được thì bạn cần cài **JDK**.

JDK bao gồm:

✔ Trình biên dịch Java  
✔ Thư viện Java  
✔ Công cụ chạy chương trình  

### 🔽 Tải JDK tại:

https://www.oracle.com/java/technologies/downloads/

Sau đó:

1️⃣ Chọn phiên bản mới nhất (JDK 21 hoặc 23 đều OK)  
2️⃣ Tải bản phù hợp Windows / macOS / Linux  
3️⃣ Cài đặt như phần mềm bình thường  

💡 Sau khi cài xong, bạn có thể kiểm tra bằng lệnh:

```bash
java -version
```

Nếu hiện ra phiên bản Java là bạn đã làm đúng 👏

## Bước 2 — Tạo file Java đầu tiên

Bạn mở Notepad / VS Code / IntelliJ / Eclipse…
Tạo file:
```
 Hello.java
 ```
```
class Hello {
    public static void main(String[] args) {
        System.out.println("Xin chào Java!");
    }
}
```

## Bước 3 — Biên dịch & chạy chương trình
🟣 Bước 3.1 — Biên dịch

Mở Terminal / CMD tại thư mục chứa file và gõ:
```
 javac Hello.java
 ```
Nếu không lỗi → sẽ xuất hiện file:
```
 Hello.class
 ```
Đây là bytecode Java.

🟢 Bước 3.2 — Chạy chương trình

Chạy tiếp:java Hello
👉 Kết quả: Xin chào Java!
🎉 Chúc mừng! Bạn đã chạy thành công chương trình Java đầu tiên.

## Giải thích chương trình trên
```
class Hello {
    public static void main(String[] args) {
        System.out.println("Xin chào Java!");
    }
}
```

✔ class Hello → khai báo 1 lớp tên Hello
✔ main() → điểm bắt đầu chương trình
✔ System.out.println() → in ra màn hình

👉 Không có main() thì chương trình không chạy được.

## Những lỗi người mới hay gặp
❌ Quên tên file phải trùng tên class
```
File: Hello.java
Class: Hello
```
Phải giống nhau!

❌ Sai dấu ngoặc {}
Java rất nghiêm về cú pháp. Thiếu 1 dấu ngoặc cũng lỗi.

❌ Gõ nhầm lệnh
Phải là:
```
javac Hello.java
java Hello
```
⚠️ Không có .java ở lệnh thứ hai.

## Nên dùng IDE nào?

Nếu mới học, bạn có thể dùng:

🟢 VS Code
🟣 IntelliJ IDEA (phổ biến nhất)
🔵 Eclipse

IDE sẽ giúp:

✔ Báo lỗi khi gõ code
✔ Tự động format
✔ Chạy code dễ dàng

## Kết luận

Trong bài này, bạn đã biết cách:

✔ Cài đặt JDK

✔ Tạo file Java đầu tiên

✔ Biên dịch & chạy chương trình

✔ Hiểu cấu trúc cơ bản của Java

👉 Đây là bước khởi đầu quan trọng trước khi học OOP, Collection, Spring Boot,…