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

* [Centering in CSS: A Complete Guide](https://css-tricks.com/centering-css-complete-guide/)

### [Scroll Snap](https://blog.logrocket.com/how-to-use-css-scroll-snap/) - Customize scroll-stop points on a page
There are two primary properties needed: `scroll-snap-type` & `scroll-snap-align`
``` CSS
.container {
 scroll-snap-type: [ x | y | block | inline | both ] [ mandatory | proximity ];
}
```
``` CSS
.children {
 scroll-snap-align: [ none | start | end | center ] 1,2;
}
```

### [Pattern.css](https://bansal.io/pattern-css) - CSS only library to fill empty background with beautiful patterns. [GitHub](https://github.com/bansal-io/pattern.css)

### [Responsive Images the Simple Way](https://cloudfour.com/thinks/responsive-images-the-simple-way/)

---

* Disable right-click 
``` CSS
    <body oncontextmenu="return false">
        <div></div>
    </body>
```
* [Useful Guide to CSS Variables](https://increment.com/frontend/a-users-guide-to-css-variables/)

* To make a child element fill the parent completely:
``` CSS
    div {
        position: 'absolute',
        top: 0,
        right: 0,
        bottom: 0,
        left: 0,
    }
```

* CSS comes with a `:optional` and `:required` pseudo-class for the input, select, and textarea tag.

* Adding `loading="lazy"` to the img instructs the browser to only start fetching the image as it gets closer to the screen and is likely to actually be rendered.

* Check for user color theme preference
```css
@media (prefers-color-scheme: dark) {
   // your code for dark mode here
}
```

---

* [Grid Layoutit](https://grid.layoutit.com) - quickly set up a grid layout

* [Autogrowing Textareas](https://css-tricks.com/the-cleanest-trick-for-autogrowing-textareas/)

* [What Can You Put in a CSS Variable?](https://codersblock.com/blog/what-can-you-put-in-a-css-variable/)

* [CSS Grid Layouting made easy in React Apps](https://medium.com/@paramsingh_66174/css-grid-layouting-made-easy-in-react-apps-a8a6b1a23531)

* [Sass Style Guide](https://css-tricks.com/sass-style-guide/)

* [Writing Your CSS like This Will Make Your Code Super-Clean](https://levelup.gitconnected.com/writing-your-css-like-this-will-make-your-code-super-clean-f82d4bfeb468)

* [CSS Tricks](https://css-tricks.com)

* [Bulma](https://bulma.io) - Bulma is a free, open source CSS framework based on Flexbox

* [Tachyons](https://tachyons.io) - Create fast loading, highly readable, and 100% responsive interfaces with as little css as possible.

* [Top 5 CSS Gotchas](https://sargalias.medium.com/the-top-5-css-gotchas-and-a-few-bonus-d39755c79527)

* [Masonry Layout](https://www.smashingmagazine.com/2021/02/things-you-can-do-with-css-today/)

* Use `overflow-x: auto` to allow scrolling on the x-axis
* If entire page is scrolling and / or too wide, check out [this article](https://ishadeed.com/article/min-content-size-css-grid/)
