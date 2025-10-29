+++
title = "Điều kiện và vòng lặp trong JavaScript"
date = "2025-10-24"
weight = 8
draft = false
banner = "img/banners/1.jpg"
authors = ["NgocChien"]
categories = ["javascript", "web", "programming"]
tags = ["javascript", "operator", "beginner"]
+++

### 1. Điều Kiện trong JavaScript

Điều kiện trong JavaScript giúp chúng ta kiểm tra các biểu thức và thực hiện các hành động khác nhau dựa trên kết quả của việc kiểm tra. JavaScript cung cấp các cấu trúc điều kiện như if, else, else if, và switch để xử lý các tình huống khác nhau.

a. Câu Lệnh if

Câu lệnh if cho phép bạn kiểm tra một điều kiện và thực hiện một hành động nếu điều kiện đó đúng (true).
```js
let age = 18

if (age >= 18) {

console.log("Bạn đã đủ tuổi để lái xe.");

}
```
b. Câu Lệnh else

Câu lệnh else được sử dụng sau câu lệnh if để thực hiện một hành động nếu điều kiện trong if không đúng (false).
```js
let age = 16;

if (age >= 18) {

console.log("Bạn đã đủ tuổi để lái xe.");

} else {

console.log("Bạn chưa đủ tuổi để lái xe.");

}
```
c. Câu Lệnh else if

Khi bạn cần kiểm tra nhiều điều kiện, bạn có thể sử dụng else if để kiểm tra các điều kiện bổ sung.
```js
let age =20;

if (age < 18) {

console.log("Bạn là thiếu niên.");

} else if (age >= 18 && age <= 60) {

console.log("Bạn là người trưởng thành.");

} else {

console.log("Bạn là người cao tuổi.");

}
```
d. Câu Lệnh switch

Câu lệnh switch là một cách khác để kiểm tra nhiều điều kiện, nhưng với cú pháp ngắn gọn hơn so với chuỗi các câu lệnh if-else.
```js
let day = 2;

let dayName;

switch (day) {

case 1:

dayName = "Thứ Hai";

break;

case 2:

dayName = "Thứ Ba";

break;

case 3:

dayName = "Thứ Tư";

break;

default:

dayName = "Ngày không hợp lệ";

}

console.log(dayName); // In ra "Thứ Ba"
```
### 2. Vòng Lặp trong JavaScript

Vòng lặp là một cấu trúc điều khiển giúp bạn thực hiện một đoạn mã nhiều lần. JavaScript hỗ trợ nhiều loại vòng lặp khác nhau, bao gồm for, while, do...while, và vòng lặp for...in và for...of.

a. Vòng Lặp for

Vòng lặp for được sử dụng khi bạn biết trước số lần lặp. Cú pháp cơ bản của vòng lặp for gồm ba phần: khởi tạo, điều kiện và bước nhảy.
```js
for (let i = 0; i < 5; i++) {

console.log(i);

}
```
Trong ví dụ trên, vòng lặp sẽ in ra các số từ 0 đến 4.
b. Vòng Lặp while

Vòng lặp while sẽ tiếp tục thực hiện một khối mã cho đến khi điều kiện kiểm tra trở thành false. Điều này có nghĩa là nếu điều kiện không được thỏa mãn ngay từ đầu, vòng lặp có thể không thực thi một lần nào.
```js
let i = 0;

while (i < 5) {

console.log(i);

i++;

}
```
Vòng lặp trên sẽ cho kết quả giống như vòng lặp for, nhưng cú pháp khác.
c. Vòng Lặp do…while

Vòng lặp do...while tương tự như vòng lặp while, nhưng nó đảm bảo rằng khối mã sẽ được thực thi ít nhất một lần, vì điều kiện được kiểm tra sau khi khối mã thực thi.
```js
let i = 0;

do {

console.log(i);

i++;

} while (i < 5);
```
d. Vòng Lặp for…in

Vòng lặp for...in được sử dụng để lặp qua các thuộc tính của một đối tượng.
```js
let person = { name: "John", age: 30, city: "New York" };

for (let key in person) {

console.log(key + ": " + person[key]);

}

Kết quả sẽ là:

name: John

age: 30

city: New York
```
e. Vòng Lặp for…of

Vòng lặp for...of được sử dụng để lặp qua các phần tử của một mảng hoặc các đối tượng có thể lặp khác như chuỗi (string).
```js
let numbers = [1, 2, 3, 4, 5];

for (let number of numbers) {

console.log(number);

}
```
Kết quả sẽ là:
1

2

3

4

5

### 3. Kết luận

Điều kiện và vòng lặp là những công cụ quan trọng trong JavaScript giúp bạn kiểm tra các giá trị và lặp lại các thao tác một cách linh hoạt. Việc hiểu và sử dụng thành thạo các cấu trúc này giúp bạn viết mã hiệu quả và dễ dàng quản lý luồng chương trình.