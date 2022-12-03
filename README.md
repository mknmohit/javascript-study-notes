
# Javascript Study Notes

JavaScript study notes for interview preparation and answers to some basic interview questions which will be helpful for cracking interviews.

# Table of Contents
- [Async vs Defer](#async-vs-defer)
- [Temporal Dead Zone (TDZ)](#temporal-dead-zone-tdz)


## Async vs Defer
<img width="768" alt="aync vs defer" src="https://user-images.githubusercontent.com/19211475/205461042-f046efb3-00fd-49f9-a391-c73b6bb39219.png">

#### References
 - https://youtube.com/watch?v=IrHmpdORLu8&t=5m10s
 - https://www.growingwiththeweb.com/2014/02/async-vs-defer-attributes.html


## Temporal Dead Zone (TDZ)

`Let` and `const` declarations are hoisted too, but they are in the temporal dead zone (it is a state where variables are unreachable) until some value is initialised to `let` or `const`. In other words, the `let` and `const` variables exist in the TDZ from the start of their enclosing scope until they are declared.

#### References
 - https://www.freecodecamp.org/news/what-is-the-temporal-dead-zone/


## Abstract Equality Comparison (x==y)

 - If type of *x* and *y* are same then compare the value using Strict Equality Comparison i.e. *x* **===** *y*
 - If *x* and *y* are not of the same type, then JavaScript will cast (coercion) one value to another before comparing, like if string and number are compared, the string is always cast into a number and then compared.


## Basic Math Operations in JavaScript

 1. If one of the operands is *STRING* **--->**  then the other one will also be considered *STRING*. Objects will be converted to strings as `[object Object]`
 2. If both operands are *BOOLEAN* or one of them is a *BOOLEAN* and another one is a *NUMBER* **--->** then *BOOLEAN* will be converted to *NUMBER*
 3. An empty array is converted either to an empty string or into 0 whenever possible.
![js-operation](https://user-images.githubusercontent.com/19211475/205461672-f82c6ba4-729c-44d2-89ca-63ac2827e27a.jpg)


#### References
 - https://learn.coderslang.com/0002-basic-javascript-arithmetics/
