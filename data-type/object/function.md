<p align="center">
  <h1 align="center">JavaScript</h1>
  <h3 align="center">--- function ---</h3>

- [Normal Function](#Normal-Function)
  - [Calling a Function](#Calling-a-Function)
  - [Function expression](#Function-expression)
  - [Returning Function](#Returning-Function)
  - [Parameterized Function](#Parameterized-Function)
  - [Rest Parameterized Function](#Rest-Parameterized-Function)
- [Arrow Function](#Arrow-Function)
  - [single parameter arrow function](#single-parameter-arrow-function)
  - [multi parameter arrow function](#multi-parameter-arrow-function)
  - [empty parameter arrow function](#empty-parameter-arrow-function)


## Normal Function

### Calling a Function

```js
function addition(){
    var num = 5;
    var result = num + num;
    console.log("Addition = " + result);
}

// calling a function
addition(); // output: Addition = 10
```

### Returning Function

```js
function subtraction(num3, num4){
    var result = num3 - num4;
    return result;
}

var x = subtraction(25, 6);
console.log("Subtraction = " + x);  // output: Subtraction = 19

console.log("Subtraction = " + subtraction(5, 7));  // output: Subtraction = -2
```

### Parameterized Function

- Single Parameterized Function

```js
function doubleIt(num) {
    return num * 2;
}
const result = doubleIt(7);
console.log(result); //output: 14
```

- Multi Parameterized Function

```js
function multiplication(num1, num2){
    var result = num1 * num2;
    return result;
}

var x = multiplication(4, 6);
console.log("Multiplication = " + x); // Multiplication = 24
```

### Rest Parameterized Function

-  print all elements of parameter

```js
function something(...x){
    console.log(x); // output: (6) [2, 4, 5, 6, 'rs', 'shonjoy']
}
something(2,4,5,6,"rs","shonjoy")
```

- print specify index value

```js
function something2(...x){
    console.log(x[4]);  // output: rs
}
something2(2,4,5,6,"rs","shonhoy")
```

- do sum in rest parameter

```js
function calculator(...numbers){
    let sum = 0;
    for(let i of numbers){
        sum = sum + i;
    }
    return sum;
}
var result = calculator(2,3,4,6,7,5)
console.log("rest parameter = " + result)  // rest parameter = 27
```

- normal + Rest parameterized function

```js
function calculator2(a, b, ...numbers){
    let add = a + b;
    let sum = 0;
    for(let i of numbers){
        sum = sum + i;
    }
    return sum ;
}
var result = calculator2(20,30,4,6,7,5)
console.log( "normal + Rest parameter = " + result) // normal + Rest parameter = 22
```

### Function expression
```js
const doubleIt = function (num) {
    return num * 2;
}
const result = doubleIt(7);
console.log(result); // output: 14
```

## Arrow Function

### single parameter arrow function

```js
const multiply = num => num * 2;

const result = multiply(7);
console.log(result); // output: 14
```

### multi parameter arrow function

- example 1
```js
const addition = (x, y) => x + y;

const result = addition(18, 19);
console.log(result); // output: 37
```

- example 2

```js
const doMath = (x, y) => {
    const add = x + y;
    const sub = x - y;
    const result = add * sub;
    return result;
}

const result = doMath(7, 5)
console.log(result);  // output: 24
```

### empty parameter arrow function

- exapmle 1

```js
const num = () => 37;

const result = num();
console.log(result) // output: 37
```

- example 2

```js
const num = () => 18 + 19;

const result = num();
console.log(result) // output: 37
```