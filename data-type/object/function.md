<p align="center">
  <h1 align="center">JavaScript</h1>
  <h3 align="center">--- function ---</h3>

- [Normal Function](#Normal-Function)
  - [Function expression](#Function-expression)
- [Arrow Function](#Arrow-Function)
  - [single parameter arrow function](#single-parameter-arrow-function)
  - [multi parameter arrow function](#multi-parameter-arrow-function)
  - [empty parameter arrow function](#empty-parameter-arrow-function)


## Normal Function

```js
function doubleIt(num) {
    return num * 2;
}
const result = doubleIt(7);
console.log(result); //output: 14
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