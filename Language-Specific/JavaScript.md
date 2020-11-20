# JavaScript

* [You Don't Know JS (2nd Edition)](https://github.com/getify/You-Dont-Know-JS/blob/2nd-ed/preface.md)

* [Eloquent Javascript (book)](https://eloquentjavascript.net/)

* [TypeScript](https://www.typescriptlang.org/docs)

* [Thinking in React Hooks](https://wattenberger.com/blog/react-hooks)

* [Linked Lists](https://codeburst.io/js-data-structures-linked-list-3ed4d63e6571)

* [JavaScript Style Guide and Coding Conventions](https://www.w3schools.com/js/js_conventions.asp)

*[Working with Arrays](https://zellwk.com/blog/how-i-work-with-arrays/?ck_subscriber_id=316695587)

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

* You can add multiple event listners to the same element:
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
