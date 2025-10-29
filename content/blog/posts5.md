+++
title= "Biến, kiểu dữ liệu, truyền kiểu và chú thích (Phần 2)"
date= "2025-10-21"
weight= 5
draft= false
banner = "img/banners/4.jpg"
authors = ["NgocChien"]
categories = ["javascript", "web", "programming"]
tags = ["javascript", "hello-world", "beginner"]
+++

JavaScript là một ngôn ngữ linh hoạt và được sử dụng rộng rãi nhờ khả năng làm việc với nhiều kiểu dữ liệu khác nhau. Trong bài viết này, chúng ta sẽ khám phá các kiểu dữ liệu chính trong JavaScript, bao gồm cách chúng hoạt động và khi nào nên sử dụng.

### 1. Kiểu Dữ Liệu Nguyên Thủy (Primitive Types)

Kiểu dữ liệu nguyên thủy là những kiểu dữ liệu cơ bản nhất trong JavaScript. Mỗi giá trị thuộc kiểu nguyên thủ là một giá trị duy nhất và không thể thay đổi. Các kiểu dữ liệu nguyên thủ bao gồm:

### 1.1. String

Đại diện cho các chuỗi ký tự. Cách khai báo:
```js
let name = “Alice”;

let greeting = ‘Hello’;
```
Lưu ý: Chuỗi trong JavaScript có thể được bao bọc bởi dấu nháy đơn (' ') hoặc nháy kép (" ").
### 1.2. Number

Đại diện cho các con số, bao gồm số nguyên và số thực. Cách khai báo:
```js
let age = 25;

let price = 99.99;
```
Lưu ý: JavaScript chỉ có một kiểu số duy nhất, khác với nhiều ngôn ngữ khác.
### 1.3. Boolean

Đại diện cho hai giá trị logic: true và false. Cách khai báo:
```js
let isLoggedIn = true;

let hasPermission = false;
```
### 1.4. Undefined

Biểu thị một biến được khai báo nhưng chưa được gán giá trị. Cách khai báo:
```js
let user = undefined;

console.log(user); //undefined
```
### 1.5. Null

Đại diện cho giá trị "trống" hoặc "không tồn tại". Cách khai báo:
```js
let value = null;
```
### 1.6. Symbol

Được giới thiệu trong ES6, biểu diễn một giá trị duy nhất và không trùng lặp. Cách khai báo:
```js
let uniqueId = Symbol('id');
```
### 2. Kiểu Dữ Liệu Tham Chiếu (Reference Types)

Các kiểu dữ liệu tham chiếu bao gồm Object, Array, và Function. Đặc điểm của chúng là giá trị được lưu trữ bằng tham chiếu, không phải trực tiếp.

### 2.1. Object

Là tập hợp các cặp key-value. Cách khai báo:
```js
let user = {

    name: "Alice",

    age: 25

};
```
### 2.2. Array

Là danh sách các phần tử. Cách khai báo:
```js
let colors = ["red", "green", "blue"];
```
### 2.3. Function

Là khối mã chứa các tác vụ. Cách khai báo:
```js
function greet()

{

console.log("Hello, World!");

}
```

