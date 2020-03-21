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