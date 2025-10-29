+++
title = "Toán tử gán, số học và logic"
date = "2025-10-23"
weight = 7
draft = false
banner = "img/banners/1.jpg"
authors = ["NgocChien"]
categories = ["javascript", "web", "programming"]
tags = ["javascript", "operator", "beginner"]
+++
### 1. Toán Tử Gán
Toán tử gán trong JavaScript được sử dụng để gán giá trị cho biến. Cách sử dụng phổ biến nhất là toán tử "=". Tuy nhiên, JavaScript cung cấp một số toán tử gán mở rộng để giúp việc gán trở nên dễ dàng hơn.

Toán tử “=:” Gán giá trị cho biến.
```js
let a = 10; // Gán giá trị 10 cho biến a
```
Toán tử +=: Gán giá trị mới bằng cách cộng thêm một giá trị vào giá trị hiện tại.
```js
let b = 5;

b += 3; // b = b + 3 => b = 8
```
Toán tử -=: Gán giá trị mới bằng cách trừ đi một giá trị.
```js
let c = 10;

c -= 4; // c = c - 4 => c = 6
```
Toán tử =: Gán giá trị mới bằng cách nhân với một giá trị.
```js
let d = 2;

d *= 5; // d = d * 5 => d = 10
```
Toán tử /=: Gán giá trị mới bằng cách chia cho một giá trị.
```js
let e = 20;

e /= 4; // e = e / 4 => e = 5
```
Toán tử %=: Gán giá trị mới bằng phép chia lấy dư.
```js
let f = 10;

f %= 3; // f = f % 3 => f = 1
```
### 2. Toán Tử Số Học

Toán tử số học trong JavaScript được sử dụng để thực hiện các phép toán cơ bản.

Toán tử +: Cộng hai giá trị lại.
```js
let sum = 10 + 5; // sum = 15
```
Toán tử -: Trừ hai giá trị.
```js
let difference = 10 - 5; // difference = 5
```
Toán tử * : Nhân hai giá trị.
```js
let product = 10 * 5; // product = 50
```
Toán tử /: Chia hai giá trị.
```js
let quotient = 10 / 2; // quotient = 5
```
Toán tử %: Lấy dư của phép chia.
```js
let remainder = 10 % 3; // remainder = 1
```
### 3. Toán Tử Logic

Toán tử logic trong JavaScript được sử dụng để thực hiện các phép toán logic với các giá trị boolean (true hoặc false).

Toán tử && (AND): Trả về true nếu cả hai biểu thức đều đúng.
```js
let a = true;

let b = false;

let result = a && b; // result = false
```
Toán tử || (OR): Trả về true nếu ít nhất một trong các biểu thức đúng.
```js
let a = true;

let b = false;

let result = a || b; // result = true
```
Toán tử ! (NOT): Đảo ngược giá trị boolean của biểu thức.
```js
let a = true;

let result = !a; // result = false
```
Toán tử ?? (Nullish Coalescing): Trả về giá trị bên trái nếu nó khác null hoặc undefined, nếu không thì trả về giá trị bên phải.
```js
let a = null;

let b = "Hello";

let result = a ?? b; // result = "Hello"
```
### 4. Kết luận
Các toán tử trong JavaScript giúp bạn thực hiện các phép toán cơ bản, từ gán giá trị, thực hiện các phép toán số học đến các phép toán logic. Việc hiểu rõ cách sử dụng chúng sẽ giúp bạn viết mã hiệu quả hơn và dễ dàng giải quyết các vấn đề trong lập trình.