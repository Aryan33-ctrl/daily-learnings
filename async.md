# 📘 Module: Asynchronous Behaviour in JavaScript

## 🚀 Introduction
Asynchronous behaviour allows JavaScript to perform tasks without blocking the execution of other code.
JavaScript is single-threaded but can handle multiple operations efficiently using async programming.

---

## 🧠 Synchronous vs Asynchronous

### Synchronous (Blocking)
```js
console.log("Start");

for(let i=0;i<1000000000;i++){}

console.log("End");
