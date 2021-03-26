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

* Extend Clickable Area
```css
button {
  border: none;
  background: #222;
  width: 10px;
  height: 10px;
  border-radius: 50%;
  padding: 0;
  position: relative;
  cursor: pointer;
}
button::after {
  content: "";
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  width: 200%;
  height: 200%;
  display: inline-block;
  /* for demo purpose only - should be removed   */
  background: rgba(0,0,0,0.2);
}
```

* Frosted Glass Effect
```css
.container {
   background-color: rgba(255, 255, 255, .15);
   backdrop-filter: blur(5px);
}
```

### Initial Letter
```css
initial-letter: normal | [<number><integer>];
```

    - normal : It does not apply a scaling effect on the first letter. This can be useful for resetting the value where one might be inherited from the cascade.
    - <number> How many lines the letter should occupy where negative values are not allowed.
    - <integer> How many lines the letter should sink where negative values are not allowed. This is handy should you need to position the letter lower to accommodate tricky spacing issues but, if not specified, it takes the value of <number>.

## Animated gradient background
```html
<div id="gradient">
  <div class="headline">
    <h1>GRADIENT</h1>
  </div>
</div>
```
```css
body {
  margin: 0;
  padding: 0;
}

.headline {

  text-align: center;
  position: absolute;
  margin: auto;
  height: 50%;
  width: 50%;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
}

h1 {
  font-family: 'Montserrat', sans-serif;
  font-weight: 700;
  letter-spacing: -5px;
  color: #fff;
}

.headline h1 {
  border: 3px solid #FFF;
  padding: 20px;
  font-size: 8vw;
}

#gradient {
  width: 100%;
  height: 100%;
  position: absolute;
  background: linear-gradient(270deg, #003366, #b27000, #06617d, #067370);
  background-size: 800% 800%;
  -webkit-animation: colors 30s ease infinite;
  -moz-animation: colors 30s ease infinite;
  animation: colors 30s ease infinite;
}

@-webkit-keyframes colors {
  0%{background-position:0% 50%}
  50%{background-position:100% 50%}
  100%{background-position:0% 50%}
}
@-moz-keyframes colors {
  0%{background-position:0% 50%}
  50%{background-position:100% 50%}
  100%{background-position:0% 50%}
}
@keyframes colors { 
  0%{background-position:0% 50%}
  50%{background-position:100% 50%}
  100%{background-position:0% 50%}
}
```

---

* [Grid Layoutit](https://grid.layoutit.com) - quickly set up a grid layout

* [Autogrowing Textareas](https://css-tricks.com/the-cleanest-trick-for-autogrowing-textareas/)

* [What Can You Put in a CSS Variable?](https://codersblock.com/blog/what-can-you-put-in-a-css-variable/)

* [CSS Grid Layouting made easy in React Apps](https://medium.com/@paramsingh_66174/css-grid-layouting-made-easy-in-react-apps-a8a6b1a23531)

* [CSS Grid Cheatsheet Illustrated](https://dev.to/joyshaheb/css-grid-cheat-sheet-illustrated-in-2021-1a3)

* [Sass Style Guide](https://css-tricks.com/sass-style-guide/)

* [Writing Your CSS like This Will Make Your Code Super-Clean](https://levelup.gitconnected.com/writing-your-css-like-this-will-make-your-code-super-clean-f82d4bfeb468)

* [CSS Tricks](https://css-tricks.com)

* [Bulma](https://bulma.io) - Bulma is a free, open source CSS framework based on Flexbox

* [Tachyons](https://tachyons.io) - Create fast loading, highly readable, and 100% responsive interfaces with as little css as possible.

* [Top 5 CSS Gotchas](https://sargalias.medium.com/the-top-5-css-gotchas-and-a-few-bonus-d39755c79527)

* [Masonry Layout](https://www.smashingmagazine.com/2021/02/things-you-can-do-with-css-today/)

* Use `overflow-x: auto` to allow scrolling on the x-axis
* If entire page is scrolling and / or too wide, check out [this article](https://ishadeed.com/article/min-content-size-css-grid/)

* [Responsive CSS Grid without media queries](https://medium.com/dev-genius/css-grid-responsive-without-media-queries-2351cf3bf386)
```css
grid-template-columns: repeat(auto-fit, minmax([width], 1fr));
```
##  Find unused CSS
  * [UnusedCSS - Clean Your CSS](https://unused-css.com)
  * [PurifyCSS Online](https://purifycss.online) - Remove unused CSS code from your stylesheets
