# Useful CSS Selectors

### prefers-color-scheme
* This one lets you react to whether the user has turned on so-called “dark mode” on their device. It has three possible values – light, dark, and no-preference.
```CSS
@media (prefers-color-scheme: dark) {
    body { background: #1e1e1e; color: white; }
}
```

### Simple way to center things
``` CSS
.class {
    display: grid;
    place-items: center center;
}
```

### [Scroll Snap](https://blog.logrocket.com/how-to-use-css-scroll-snap/) - Customize scroll-stop points on a page
There are two primary properties needed: `scroll-snap-type` & `scroll-snap-align`
``` CSS
.container {
 scroll-snap-type: [ x | y | block | inline | both ] [ mandatory | proximity ];
}
```
``` CSS
.children {
 scroll-snap-align: [ none | start | end | center ]{1,2};
}
```

### [Pattern.css](https://bansal.io/pattern-css) - CSS only library to fill empty background with beautiful patterns. [GitHub](https://github.com/bansal-io/pattern.css?utm_source=hackernewsletter&utm_medium=email&utm_term=design)
