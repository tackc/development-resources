# JavaScript

* [You Don't Know JS (2nd Edition)](https://github.com/getify/You-Dont-Know-JS/blob/2nd-ed/preface.md)

* [Eloquent Javascript (book)](https://eloquentjavascript.net/)

* [TypeScript](https://www.typescriptlang.org/docs)

* [Thinking in React Hooks](https://wattenberger.com/blog/react-hooks)

* [Linked Lists](https://codeburst.io/js-data-structures-linked-list-3ed4d63e6571)

* [JavaScript Style Guide and Coding Conventions](https://www.w3schools.com/js/js_conventions.asp)

* [Working with Arrays](https://zellwk.com/blog/how-i-work-with-arrays/?ck_subscriber_id=316695587)

* [The 7 JS Array Methods you will need in 2021](https://medium.com/dailyjs/the-7-js-array-methods-you-will-need-in-2021-a9faa83b50e8)

* [JS Cheatsheet](https://htmlcheatsheet.com/js/)

* [JavaScript: Basic, Advanced, & More Cheat Sheet](https://cheatography.com/acwinter/cheat-sheets/javascript-basic-advanced-and-more/)

## Testing
* [Mocha JS](https://mochajs.org) - Mocha is a feature-rich JavaScript test framework running on Node.js and in the browser, making asynchronous testing simple and fun. Mocha tests run serially, allowing for flexible and accurate reporting, while mapping uncaught exceptions to the correct test cases.

* [Chai Assertion Library](https://www.chaijs.com) - Chai is a BDD / TDD assertion library for node and the browser that can be delightfully paired with any javascript testing framework.

## Tips & Tricks

### Convert number to string || binary || hexadecimal
JavaScript numbers natively support conversion to binary representations via the toString method:
```
(255).toString(); // "255" (default is radix 10)
(255).toString(2); // "11111111" (radix 2, i.e. binary)
(255).toString(16); // "ff" (radix 16, i.e. hexadecimal)
```

* [CREATING UNIQUE, MERGED ARRAYS USING JAVASCRIPT'S SET](https://robkendal.co.uk/blog/2020-02-04-creating-unique-merged-arrays-using-javascripts-set-and-more)

### [Event Handler vs addEventListner](https://medium.com/dailyjs/whats-the-difference-between-event-handlers-addeventlistener-in-js-963431f05c34)
* If you add two of the same event handlers to the same element, the second one will overwrite the first:
```
  const button = document.querySelector(".btn")
    
  button.onclick = () => {
    console.log("Hello!");
  };

  button.onclick = () => {
    console.log("How are you?");
  };

  // This wil log "How are you?" to the console.
```

* You can add multiple event listeners to the same element:
```
  const button = document.querySelector(".btn")
  
  button.addEventListener("click", event => {
    console.log("Hello!");
  })
  
  button.addEventListener("click", event => {
    console.log("How are you?");
  })

  // This wil log 
  // "Hello!"
  // "How are you?"
  // to the console
```

* [TensorFlow.js](https://www.tensorflow.org/js/) - Develop ML models in JavaScript, and use ML directly in the browser or in Node.js

* [ES2021 New Features](https://medium.com/javascript-in-plain-english/whats-new-in-es2021-99921c01f220)

* [Factory Function](https://medium.com/javascript-scene/javascript-factory-functions-with-es6-4d224591a8b1)

* [State of JS 2020](https://stateofjs.com/)

* [Unit Testing](https://www.freecodecamp.org/news/how-to-start-unit-testing-javascript/)

## Useful JavaScript Snippets

* Check if the current tab is in view / focus
```js
  const isBrowserTabInView = () => document.hidden;
  isBrowserTabInView();
  // Result: returns true or false depending on if tab is in view / focus
```

* Get the time from a date
```js
  const timeFromDate = date => date.toTimeString().slice(0, 8);
  console.log(timeFromDate(new Date(2021, 0, 10, 17, 30, 0))); 
  // Result: "17:30:00"
  console.log(timeFromDate(new Date()));
  // Result: will log the current time
```

* Check if an element is currently in focus
```js
  const elementIsInFocus = (el) => (el === document.activeElement);
elementIsInFocus(anyElement)
// Result: will return true if in focus, false if not in focus
```

* Check if the current user is on an Apple device
```js
  const isAppleDevice = /Mac|iPod|iPhone|iPad/.test(navigator.platform);
  console.log(isAppleDevice);
  // Result: will return true if user is on an Apple device
```

* Scroll to top of the page
```js
  const goToTop = () => window.scrollTo(0, 0);
goToTop();
  // Result: will scroll the browser to the top of the page
```

* Get average value of arguments
```js
  const average = (...args) => args.reduce((a, b) => a + b) / args.length;
  average(1, 2, 3, 4);
  // Result: 2.5
```

* Convert Fahrenheit / Celsius
```js
  const celsiusToFahrenheit = (celsius) => celsius * 9/5 + 32;
  const fahrenheitToCelsius = (fahrenheit) => (fahrenheit - 32) * 5/9;
  // Examples
  celsiusToFahrenheit(15);    // 59
  celsiusToFahrenheit(0);     // 32
  celsiusToFahrenheit(-20);   // -4
  fahrenheitToCelsius(59);    // 15
  fahrenheitToCelsius(32);    // 0
```

# ES2021 (ES 12)

* ```js
  String.prototype.replaceAll()
  ```

* Logical Assignment Operators
  ```js
  // The Old Way
  if (!a) {
    a = b
  }
  // or 
  a = a || b
  // Using a Logical Assignment Operator
  a ||= b
  ```

* Numeric Separators
  ```js
  // You can break the digits in any way
  const BIGNUMBER = 1234_5678_9_0;  // 1234567890
  // Even after the comma/period
  const PI = 3.1415_9265_3589;     // 3.141592653589
  // However, ending or beginning with an underscore will return an error!
  const BAD_PI = 3.14_15_;          // SyntaxError
  const NO_MILLION = _1_000_000;    // ReferenceError
  ```

* Promise.any - The Promise.any method takes an array of Promises and will return as soon as the first one is Fulfilled.
