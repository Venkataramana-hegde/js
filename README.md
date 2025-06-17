## 📘 README: JavaScript Beginner Projects

### 🚀 Project Overview

This document includes a collection of beginner-friendly JavaScript exercises and interactive UI features built using **vanilla JS**. The key focus areas are:

* DOM Manipulation
* Event Handling
* Promises
* Async/Await
* setTimeout
* Closures
* LocalStorage

---

### Features Implemented

#### Counter App (DOM Manipulation)

* **Buttons**: Increase, Decrease, Reset
* **Displays**: Dynamic count update via `.innerHTML`
* **Handled With**: `getElementById`, `querySelector`, `onclick` event listeners

#### Async Joke Generator

* `getJoke()` returns a `Promise` that resolves after 2 seconds
* Button triggers async call and displays "Loading joke..." followed by the joke
* Demonstrates `await` behavior in UI updates

#### Random Dog Image Fetcher

* API: `https://dog.ceo/api/breeds/image/random`
* Button fetches and displays a new dog image
* Wrapped in `try...catch` to handle network errors

#### LocalStorage with Username

* On first visit, user prompted to enter name
* Name saved in `localStorage` and persists across reloads
* A button lets the user reset their name
* Uses `prompt()`, `localStorage.setItem()` and `getItem()`

#### Closures & Scope Practice

```js
for (var i = 0; i < 3; i++) {
  setTimeout(() => console.log("var:", i), 1000); // logs 3, 3, 3
}
for (let j = 0; j < 3; j++) {
  setTimeout(() => console.log("let:", j), 1000); // logs 0, 1, 2
}
```

* Shows how `var` leaks to function/global scope
* Shows how `let` has block scope

---

### Difficulties Faced

* **Understanding Promises**: Initially confusing to know when `.then()` runs and how `.then()` chaining works.
* **Async/Await Timing**: Mixing `await` with sync code was tricky to mentally model.
* **`setTimeout` Execution**: Needed clarity on why all `var` examples logged the same value.
* **Closure Behavior**: Understanding how a function retains access to variables even after outer execution completed.

---

### Technologies Used

* HTML5
* JavaScript (ES6+)
* Public API: [dog.ceo](https://dog.ceo/dog-api/)
* Browser LocalStorage

---

### Next Steps

* Build a Todo App with persistent storage
* Use `fetch()` with error retries
* Revise previous day concepts and programs and try implementing them again
* Learn more about  `Prmoises`, `async await`

---

###


