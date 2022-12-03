
# Javascript Study Notes

JavaScript study notes for interview preparation and answers to some basic interview questions which will be helpful for cracking interviews.

# Table of Contents
- [Async vs Defer](#async-vs-defer)
- [Temporal Dead Zone (TDZ)](#temporal-dead-zone-tdz)
- [Abstract Equality Comparison (x==y)](#abstract-equality-comparison-xy)
- [Basic Math Operations in JavaScript](#basic-math-operations-in-javascript)
- [Call vs Apply vs Bind](#call-vs-apply-vs-bind)


# Async vs Defer
<img width="768" alt="aync vs defer" src="https://user-images.githubusercontent.com/19211475/205461042-f046efb3-00fd-49f9-a391-c73b6bb39219.png">

#### References
 - https://youtube.com/watch?v=IrHmpdORLu8&t=5m10s
 - https://www.growingwiththeweb.com/2014/02/async-vs-defer-attributes.html


# Temporal Dead Zone (TDZ)

`Let` and `const` declarations are hoisted too, but they are in the temporal dead zone (it is a state where variables are unreachable) until some value is initialised to `let` or `const`. In other words, the `let` and `const` variables exist in the TDZ from the start of their enclosing scope until they are declared.

#### References
 - https://www.freecodecamp.org/news/what-is-the-temporal-dead-zone/


# Abstract Equality Comparison (x==y)

 - If type of *x* and *y* are same then compare the value using Strict Equality Comparison i.e. *x* **===** *y*
 - If *x* and *y* are not of the same type, then JavaScript will cast (coercion) one value to another before comparing, like if string and number are compared, the string is always cast into a number and then compared.


# Basic Math Operations in JavaScript

 1. If one of the operands is *STRING* **--->**  then the other one will also be considered *STRING*. Objects will be converted to strings as `[object Object]`
 1. If both operands are *BOOLEAN* or one of them is a *BOOLEAN* and another one is a *NUMBER* **--->** then *BOOLEAN* will be converted to *NUMBER*
 1. An empty array is converted either to an empty string or into 0 whenever possible.

![js-operations](https://user-images.githubusercontent.com/19211475/205461672-f82c6ba4-729c-44d2-89ca-63ac2827e27a.jpg)


#### References
 - https://learn.coderslang.com/0002-basic-javascript-arithmetics/


# Call vs Apply vs Bind

### Call()

 1. Using call() method we can do the function borrowing.
 1. The first argument in *call()* is the reference to other data (where we want *this* should point to) and rest of the other arguments are parameters for the function on which we are calling the *call()* method.

### Apply()

 1. The only difference between *Apply* and *Call* methods is the way how we pass the arguments.
 1. The second arguments in Apply method is the array of arguments. And in call method we pass the arguments individually as comma separated.
 
 ### Bind()
 1. The Bind method is similar to Call method, instead of directly calling or invoking the methods in case of call and apply, the bind method will returns a new method which can be called/invoked later in the program.

<img width="1512" alt="Screenshot 2022-12-04 at 2 54 28 AM" src="https://user-images.githubusercontent.com/19211475/205462913-144d2a8d-dd4e-47cd-936b-448da6616913.png">

#### References
 - https://www.youtube.com/watch?v=75W8UPQ5l7k
