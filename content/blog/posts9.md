+++
title = "Hàm trong JavaScript"
date = "2025-10-24"
weight = 9
draft = false
banner = "img/banners/1.jpg"
authors = ["NgocChien"]
categories = ["javascript", "web", "programming"]
tags = ["javascript", "operator", "beginner"]
+++

Hàm (function) trong JavaScript là một khối mã có thể được gọi và thực thi khi cần thiết. Hàm giúp tổ chức mã nguồn tốt hơn, giảm thiểu sự trùng lặp và dễ dàng tái sử dụng. JavaScript cung cấp nhiều cách để khai báo và sử dụng hàm.

### 1. Khai Báo Hàm trong JavaScript

Có hai cách phổ biến để khai báo hàm trong JavaScript: khai báo hàm thông thường và khai báo hàm dưới dạng biểu thức hàm.

a. Hàm Cơ Bản (Function Declaration)

Cách đơn giản nhất để khai báo một hàm trong JavaScript là sử dụng cú pháp function. Hàm được khai báo với từ khóa function, sau đó là tên hàm, danh sách tham số trong dấu ngoặc đơn và phần thân hàm trong dấu ngoặc nhọn.
```js
function greet(name) {

console.log("Hello, " + name + "!");

}

greet("John"); //In ra: Hello, John!
```
Trong ví dụ trên, hàm greet nhận một tham số name và in ra một thông điệp chào mừng.

b. Biểu Thức Hàm (Function Expression)

Hàm có thể được khai báo dưới dạng biểu thức hàm và có thể được gán cho một biến. Điều này cho phép bạn tạo các hàm vô danh (anonymous functions), tức là hàm không có tên.
```js
let sum = function(a, b) {

return a + b;

};

console.log(sum(2, 3)); // In ra: 5
```
Trong ví dụ trên, hàm không có tên và được gán cho biến sum, sau đó có thể gọi hàm thông qua biến này.

### 2. Hàm với Tham Số và Trả Về Giá Trị

Hàm có thể nhận một hoặc nhiều tham số và trả về một giá trị. Tham số của hàm là những giá trị được truyền vào hàm khi nó được gọi, còn giá trị trả về có thể được sử dụng trong các phép toán khác.

a. Tham Số

Tham số là các biến được khai báo trong dấu ngoặc đơn của hàm và được sử dụng trong thân hàm.
```js
function multiply(x, y) {

return x * y;

}

console.log(multiply(2, 3)); //In ra: 6
```
Hàm multiply nhận hai tham số x và y, và trả về giá trị của phép nhân chúng.

b. Giá Trị Trả Về (Return)

Hàm có thể trả về một giá trị sử dụng từ khóa return. Khi một giá trị được trả về, hàm sẽ kết thúc và không thực thi các mã còn lại.
```js
function square(number) {

return number * number;

}

let result = square(4);

console.log(result); // In ra: 16
```
### 3. Hàm với Tham Số Mặc Định

JavaScript cho phép bạn gán giá trị mặc định cho các tham số hàm. Nếu không có giá trị được truyền vào khi gọi hàm, giá trị mặc định sẽ được sử dụng.
```js
function greet(name = "Guest") {

console.log("Hello, " + name + "!");

}

greet(); // In ra: Hello, Guest!

greet("Alice"); // In ra: Hello, Alice!
```
Trong ví dụ trên, nếu không truyền tham số name, giá trị mặc định là “Guest” sẽ được sử dụng.

### 4. Hàm Nhanh (Arrow Function)

Trong ES6, JavaScript giới thiệu một cách khai báo hàm mới gọi là arrow function. Cú pháp của arrow function ngắn gọn hơn và không có từ khóa function, thay vào đó sử dụng dấu =>.
```js
let add = (a, b) => a + b;

console.log(add(2, 3)); // In ra: 5
```
Arrow function rất hữu ích khi bạn muốn viết hàm ngắn gọn, nhưng cũng có những điểm khác biệt như không có this và không thể sử dụng làm hàm khởi tạo.

### 5. Hàm Tự Gọi (IIFE - Immediately Invoked Function Expression)

IIFE là một biểu thức hàm được gọi ngay sau khi được khai báo. Cú pháp của IIFE là hàm được bao trong dấu ngoặc đơn, và sau đó được gọi ngay lập tức.
```js
(function() {

console.log("This is an IIFE!");

})();
```
IIFE thường được sử dụng để tạo ra một phạm vi (scope) riêng biệt cho các biến trong hàm mà không làm ảnh hưởng đến phạm vi toàn cục.

### 6. Hàm Tham Chiếu và Hàm Gọi Lại (Callback Functions)

Hàm trong JavaScript có thể được truyền như một tham số cho một hàm khác. Hàm nhận tham số này gọi là callback function.
```js
function processData(data, callback) {

console.log("Processing: " + data);

callback();

}

function showResult() {

console.log("Processing Complete!");

}

processData("File 1", showResult);
```
Trong ví dụ trên, hàm showResult là một hàm callback được truyền vào hàm processData và được gọi sau khi quá trình xử lý dữ liệu hoàn tất.

### 7. Hàm Đệ Quy (Recursive Functions)

Hàm đệ quy là hàm gọi chính nó trong quá trình thực thi. Hàm đệ quy rất mạnh mẽ và hữu ích trong việc giải quyết các bài toán phức tạp như tính toán giai thừa, tìm kiếm trong cây,…
```js
function factorial(n) {

if (n === 0) {

return 1;

}

return n * factorial(n - 1);

}

console.log(factorial(5)); // In ra: 120
```
Trong ví dụ trên, hàm factorial tính giai thừa của một số thông qua việc gọi chính nó.

### 8. Kết luận

Hàm là một phần quan trọng trong JavaScript, giúp bạn tổ chức và tái sử dụng mã dễ dàng. Từ việc khai báo các hàm cơ bản, đến việc sử dụng hàm dưới dạng biểu thức, arrow function, hàm đệ quy và callback function, JavaScript cung cấp nhiều công cụ mạnh mẽ để xử lý các tác vụ phức tạp.