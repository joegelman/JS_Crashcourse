# JS Crash Course Notes
## Based on [this](https://youtu.be/hdI2bqOjy3c) tutorial

---
# 1. The `<Script>` Tag
<!-- <button>Time Stamp</button> -->

<!-- <br> -->

Syntax for external JS is:

> `<script src="main.js"></script>`

<br>

---

# 2. The Console

Console shows up in dev tools when you click inspect in the browser (can also access from IDE). 

> ` console.log('Hello World');`

*This is what it looks like*

![Console Log Image](images/console_log_error.min.png)

Also have the ability to do things other than .log

> `console.error('this is an error');`
> `console.warn('this is a warning);`

<br>

---

# 3. Variables

Three types of variables
- var
- let
- const

## `Var`

Var is the OG variable – but it's outdated since ES6. Especially since it's globally scoped.

## Let + Const

These are both at "Block-Level" Scope

### Let

Let is unique becase it "lets" you redesignate variables.

### Const

Is a "constant" meaning, once it's assigned it can never be reassigned.

Must assign a value right from the start.

### When to use let vs. const

Some people say it's best to have the flexibility of Let all the time.

But best practice is to always use Const, unless you know you're going to need Let *(leads to more robust, secure code)*

<br>

___

# 4. Data Types

## Data Primitives

Primitive datatypes mean data is directly assigned to memory. It's not a resource.

### String
```js  
const name = 'John';
```
### Number
```js
const age = 30;
```
### Boolean
```js
const isCool = true;
```
### null
```js
const x = null;
```
### undefined
```js
const y = undefined;
```
### *Symbol**
> *Symbol was only added in ES6 and beyond the scope of beginners*

## Strings

Let's say we have:

```js
const name = 'John';
const age = 30;
```

and we want to log:

```js
console.log('My name is *name* and I am *age*');
```

We have the following ways to do it:

### Concatenation

```js
console.log('My name is ' + name + ' and I am' + age);
```

### Template String

```js
const hello = 'My name is ${name} and I am ${age}';

--then--

console.log(hello);
```

## String Methods

Say we have a string:

```js
const s = 'Hello World!';
```

Now what if we want to get the length of the string we could use the length property (*properties* do not have parentheses, if it has parentheses it's a *method*)

```js
console.log(s.length);
```
This will output:

```
12
```

---
We can also change the case `toUpperCase()`*:

```js
console.log(s.toUpperCase());
```

Will output:
```
HELLO WORLD!
```

*Because `toUpperCase()` is a *method* it needs parentheses. And basically methods are *functions* associated with an *object*.

We can do the opposite as well, `toLowerCase()`:

```js
console.log(s.toLowerCase());
```

Will output:
```
hello world!
```











