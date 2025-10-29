+++
title= "Biến, kiểu dữ liệu, truyền kiểu và chú thích (Phần 1)"
date= "2025-10-21"
weight= 4
draft= false
banner = "img/banners/4.jpg"
authors = ["NgocChien"]
categories = ["javascript", "web", "programming"]
tags = ["javascript", "hello-world", "beginner"]
+++


Để sử dụng JavaScript một cách hiệu quả, việc hiểu rõ các khái niệm cơ bản như biến, kiểu dữ liệu, truyền kiểu và chú thích là rất quan trọng. Trong bài viết này, chúng ta sẽ cùng tìm hiểu các khái niệm này một cách chi tiết.

Vì bài viết này tìm hiểu khá nhiều khái niệm nên tôi sẽ chia nó làm nhiều phần.

## 1. Biến là gì?

Bạn hãy tưởng tượng rằng dòng chữ Hello World mà chúng ta in ra trong bài trước chính là một món hàng. Nhưng để có thể sử dụng món hàng đó bất cứ khi nào, chúng ta cần một chiếc hộp để đựng nó. Chiếc hộp đó chính là biến trong lập trình.

Một chiếc hộp (biến) trong JavaScript có thể chứa bất kỳ thứ gì bạn muốn: một con số, một đoạn chữ, hay thậm chí là một mệnh lệnh. Khi bạn đặt món hàng vào chiếc hộp, bạn có thể dán nhãn cho nó để dễ nhớ. Nhãn đó chính là tên biến.

## 2. Cách khai báo biến trong JavaScript

Để tạo ra chiếc hộp này, chúng ta sử dụng các từ khóa `let`, `const`, hoặc `var`. Hãy hình dung rằng những từ khóa này giống như các loại hộp khác nhau, mỗi loại có đặc điểm riêng.

### Khai báo một chiếc hộp (biến)

```js
let message = "Hello, World!";
```
"let" là cách bạn nói với JavaScript: "Hãy tạo một chiếc hộp có thể thay đổi, và tôi đặt tên cho nó là message.". Nội dung bên trong hộp là "Hello, World!".

Giờ bạn có thể dùng chiếc hộp này bất kỳ lúc nào — chỉ cần gọi tên message, JavaScript sẽ lấy dữ liệu bên trong hộp ra cho bạn.

Thay đổi nội dung hộp (biến)

message = Hello, JavaScript!";

Chiếc hộp vẫn giữ nguyên tên, nhưng bạn có thể thay đổi món hàng bên trong.
Khai báo một hộp (biến) không đổi

const pi = 3,14;

Với "const", bạn tạo ra một chiếc hộp mà nội dung bên trong không thể thay đổi. Một khi bạn đã đặt 3.14 vào, bạn không thể thay thế nó bằng một giá trị khác.
### 3. Biến giúp ích gì?

Bạn có thể nghĩ rằng "Tại sao không dùng trực tiếp nội dung như "Hello, World!" mà cần biến?" Câu trả lời là: biến giúp bạn tái sử dụng và tổ chức dữ liệu dễ dàng hơn.

Ví dụ: Tái sử dụng dữ liệu. Thay vì viết đi viết lại "Hello, World!" mỗi lần cần in, bạn chỉ cần dùng biến:

```js
let message = "Hello World!";

console.log(message);

console.log(message);

console.log(message);
```
Ví dụ: Thay đổi dữ liệu linh hoạt. Nếu bạn cần thay đổi nội dung, chỉ cần cập nhật biến:
```js
let message = "Hello, World!";

console.log(message);

message = "Hello, JavaScript!";

console.log(message);
```

Bạn không cần sửa tất cả các chỗ dùng "Hello, World!" trong mã nguồn, giúp bạn tiết kiệm thời gian.

### 4. Tên biến - Ghi nhớ và hiểu

Tên biến giống như nhãn trên hộp. Nếu bạn đặt tên biến rõ ràng, bạn sẽ dễ dàng hiểu được vai trò của biến đó. Một số quy tắc và gợi ý:

Tên biến phải bắt đầu bằng chữ cái, _, hoặc $.

Không được chứa khoảng trắng, các từ khóa hoặc ký tự đặc biệt.

Hãy chọn tên gợi nhớ ý nghĩa, ví dụ:
```js

let userName = "Alice";

let age = 25;
```

### 5. Kết luận

Biến là một khái niệm cốt lõi trong JavaScript. Hãy nghĩ về nó như những chiếc hộp giúp bạn lưu trữ và tổ chức dữ liệu một cách hiệu quả. Khi bạn hiểu cách sử dụng biến, bạn đã bước thêm một bước gần hơn đến việc làm chủ JavaScript!