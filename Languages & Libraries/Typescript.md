# Typescript

* [TypeScript: Interface — Part I: Parameters with Interfaces](https://medium.com/@emok032/typescript-interface-part-i-parameters-with-interfaces-d4dbaa9e1773)

* [Use Null instead of ? operator](https://levelup.gitconnected.com/5-advanced-typescript-tips-to-make-you-a-better-programmer-bd4070aa2ab4)
  * Undefined is something that JS can assign — for example, if we have a textbox and no value is inputted, then it would be undefined. Think of undefined as JS’s automatic null.
  It can be pretty difficult to tell if a field is undefined by design, or if we accidentally left it that way. If I ever intentionally want to leave to value for a field, I’ll use null. That way, everyone knows that that field is intentionally left blank.
  ```js
    interface Foo {
      bar: string | null
    }
  ```
  