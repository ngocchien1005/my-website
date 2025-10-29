+++
title= "Biến, kiểu dữ liệu, truyền kiểu và chú thích (Phần 3)"
date= "2025-10-22"
weight= 6
draft= false
banner = "img/banners/4.jpg"
authors = ["NgocChien"]
categories = ["javascript", "web", "programming"]
tags = ["javascript", "hello-world", "beginner"]
+++
### 1. Chuyển Đổi Kiểu Dữ Liệu trong JavaScript

Chuyển đổi kiểu là quá trình biến đổi một giá trị từ kiểu dữ liệu này sang kiểu dữ liệu khác. JavaScript tự động thực hiện chuyển đổi kiểu trong một số tình huống, nhưng bạn cũng có thể chủ động thực hiện chuyển đổi khi cần thiết.

Chuyển Đổi Kiểu Tự Động (Implicit Type Conversion) JavaScript có thể tự động chuyển đổi kiểu dữ liệu trong các phép toán. Đây là một cơ chế gọi là "chuyển đổi kiểu ngầm định".

Ví dụ:
```js
let a = 5;

let b = 10;

let sum = a + b; //5+10

console.log(sum); //15
```
Trong ví dụ trên, mặc dù a là một chuỗi và b là một số, JavaScript tự động chuyển đổi b thành chuỗi và nối chúng lại với nhau.
Chuyển Đổi Kiểu Thủ Công (Explicit Type Conversion). Bạn có thể chủ động chuyển đổi kiểu dữ liệu bằng các hàm chuyển đổi kiểu như String(), Number(), và Boolean().

Chuyển đổi sang chuỗi:
```js
let num = 123;

let str = String(num); // Chuyển số thành chuỗi

console.log(str); // "123"
```
Chuyển đổi sang số:
```js
let str = "456";

let num = Number(str); // Chuyển chuỗi thành số

console.log(num); //456
```
Chuyển đổi sang Boolean:
```js
let value = 0;

let bool = Boolean(value); // 0 will be converted to false

console.log(bool); // false
```
Các Tình Huống Chuyển Đổi Kiểu Thường Gặp

Sử dụng trong phép toán cộng:
```js
let a = "5";

let b = 2;

let result = a - b; // JavaScript will convert "5" to a number before performing subtraction

console.log(result); // 3
```
So sánh giá trị:
```js
console.log("5" == 5); // true (vì JavaScript chuyển đổi kiểu dữ liệu để so sánh)

console.log("5" === 5); // false (so sánh cả giá trị và kiểu dữ liệu)
```
### 2. Chú Thích trong JavaScript

Chú thích (comments) là những phần trong mã nguồn không được chương trình thực thi. Chúng chỉ để giúp người lập trình khác hiểu mã nguồn. Trong JavaScript, có hai loại chú thích chính:

Chú Thích Một Dòng
```js
Chú thích một dòng được sử dụng để giải thích một đoạn mã cụ thể. Nó bắt đầu bằng //.

// Đây là một chú thích một dòng

let x = 10; // Biến x được khởi tạo với giá trị 10
```
Chú Thích Đa Dòng

Chú thích đa dòng bắt đầu bằng /* và kết thúc bằng */. Chúng có thể được sử dụng để chú thích nhiều dòng mã.
```js
/*
Đây là một chú thích đa dòng.
Bạn có thể viết nhiều dòng chú thích ở đây.
Mã này không được thực thi.
*/

let y = 20;
```
### 3. Lợi Ích của Chuyển Đổi Kiểu và Chú Thích

Chuyển đổi kiểu giúp mã của bạn linh hoạt: Việc hiểu và sử dụng chuyển đổi kiểu sẽ giúp bạn làm việc với nhiều loại dữ liệu khác nhau một cách dễ dàng.

Chú thích giúp mã nguồn dễ đọc hơn: Chú thích là cách tuyệt vời để giải thích lý do tại sao bạn làm điều gì đó trong mã nguồn. Điều này rất quan trọng khi làm việc trong một nhóm phát triển phần mềm.