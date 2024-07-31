---
# You can also start simply with 'default'
theme: seriph
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://cover.sli.dev
# some information about your slides (markdown enabled)
title: Welcome to Slidev
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
# apply unocss classes to the current slide
class: text-center
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# https://sli.dev/guide/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations#slide-transitions
transition: slide-left
# enable MDC Syntax: https://sli.dev/guide/syntax#mdc-syntax
mdc: true
---

# Function as First-Class Citizens

---

# What is Function ❓

<v-clicks>

- A function is a "subprogram"
- Promoting reusability

</v-clicks>

---

<v-clicks>

# Passed as arguements to other functions

```js
function square(x) {
  return x * x;
}

function performOperation(operation, number) {
  let result = operation(number);
  console.log(`The result of the operation is: ${result}`);
}

performOperation(square, 5);
```

> Ouptut : The result of the operation is: 25

</v-clicks>

---

# A Function can return another function

<v-clicks>

```js
function createMultiplier(factor) {
  return function (number) {
    return number * factor;
  };
}

let double = createMultiplier(2);
let triple = createMultiplier(3);

console.log(double(5)); // Output: 10
console.log(triple(5)); // Output: 15
```

</v-clicks>

---

# A Function can be assigned to a variable

<v-clicks>

```js
let greet = function () {
  console.log("Hey there! How's it going?");
};

greet();
```

</v-clicks>

---

# Conclusion

<v-clicks>

<h1 style="color:black">Function can be treated as <b style="color:red"> VALUES 😊</b></h1>

</v-clicks>

---

# Thank You
