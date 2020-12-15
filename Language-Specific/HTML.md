# HTML

* [Schema.org](https://schema.org) - Schema.org is a collaborative, community activity with a mission to create, maintain, and promote schemas for structured data on the Internet, on web pages, in email messages, and beyond.
---

## Tips & Tricks
* Color Picker - An ```<input>``` element with a type of “color” provides a UI element that lets the user specify a color.
```CS
  <label for="favcolor">Select your favorite color:</label>
  <input type="color" id="favcolor" name="favcolor">
```

* Datalist - The ```<datalist>``` tag is used to provide an "autocomplete" feature for ```<input>``` elements. You will see a drop-down list of pre-defined options as you type.
```CS
  <input list="animals" name="animal" id="animal">
  <datalist id="animals">
      <option value="Cat">
      <option value="Dog">
      <option value="Chicken">
      <option value="Cow">
      <option value="Pig">
    </datalist>
```

* Picture - The ```<picture>``` tag gives web developers more flexibility in specifying image resources for responsive design
```CS
  <picture>
    <source media="(min-width:1024px)" srcset="dog-big.jpg">
    <source media="(min-width:465px)" srcset="dog-small.jpg">
    <img src="cat.jpg" alt="Flowers" style="width:auto;">
  </picture>
```
