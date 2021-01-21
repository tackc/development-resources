# React Resources

* [Ultimate React JS Starter Guide](https://medium.com/javascript-in-plain-english/how-i-learned-react-js-as-a-noob-ultimate-react-js-starter-guide-36a05ab9495e)

* [React Dropdown](https://www.carlrippon.com/react-drop-down-data-binding/)

* [8 Useful Tricks for React Apps](https://medium.com/better-programming/8-useful-tricks-for-react-apps-you-should-know-a15c2678c846)

* [5 Essential Libraries For Your Next React Application](https://medium.com/frontend-digest/5-essential-libraries-for-your-next-react-application-84d8d73e9806)

* [How I Share React Components Between Projects](https://medium.com/javascript-in-plain-english/how-i-share-react-components-between-projects-3896d853cbee)

* [React Folder Structure in 5 Steps](https://www.robinwieruch.de/react-folder-structure)

* [Implementing Dark Mode In React Apps Using styled-components](https://www.smashingmagazine.com/2020/04/dark-mode-react-apps-styled-components/?utm_source=CSS-Weekly&utm_campaign=Issue-409&utm_medium=email)

* [How to Conditionally Render React Components](https://medium.com/better-programming/conditional-rendering-in-react-components-bea51e34f3a1)

* [Understand and use useState Hooks in React](https://dev.to/emmanuel_dal/understand-and-use-usestate-hooks-in-react-jij)

* [React Router](https://reacttraining.com/react-router/web/api/Redirect)

* [React Stack example](https://medium.com/better-programming/my-favourite-react-stack-1beda91ae909) - Great article that breaks down several major options when building a React app

* [Performant Development with React](https://medium.com/dev-red/these-5-tips-will-change-the-way-you-write-react-apps-75e97c90d5c8)

* [Babeljs.io](https://babeljs.io) - Allows you to enter JSX and get code back in javascript

* [React Loader Spinner](https://www.npmjs.com/package/react-loader-spinner) - animated loader animations

* [React Countup](https://www.npmjs.com/package/react-countup) - add a counter to react pages easily

* [React Design Patterns](https://reactpatterns.com)

* [setTimeout in React Components Using Hooks](https://upmostly.com/tutorials/settimeout-in-react-components-using-hooks) - 
  ```js
    useEffect(() => {
      const timer = setTimeout(() => {
        console.log('This will run after 1 second!')
      }, 1000);
      return () => clearTimeout(timer);
    }, []);
  ```
  
  * [Log in with JWT Authentication in Rails and React](https://medium.com/analytics-vidhya/log-in-with-jwt-authentication-in-rails-and-react-a3dddd7f934)

* Optimize list rendering with `useMemo`. For example:
```js
  import React, { useMemo } from 'react';

  function SortedListView ({ title, items, comparisonFunc }) {
    const sortedItems = useMemo(() => {
      const sortedItems = [...items];
      sortedItems.sort(comparisonFunc);
      return sortedItems;
    }, [items, comparisonFunc]);
    return (
      <div>
        <h1> {title} </h1>
        <ul>
          {sortedItems.map(item => <li> {item} </li>)}
        </ul>
      </div>
    );
  }
```

* [Consuming a REST API with React Hooks (using design patterns)](https://medium.com/weekly-webtips/implementing-a-rest-api-with-react-hooks-using-patterns-2ea1476e2a05) - This article discusses abstracting low level calls away to separate business logic from display

## Useful Libraries

* [react-select](https://react-select.com/home) - A flexible and beautiful Select Input control for ReactJS with multiselect, autocomplete, async and creatable support.

* [react-dnd](https://react-dnd.github.io/react-dnd/about) - React DnD is a set of React utilities to help you build complex drag and drop interfaces while keeping your components decoupled. It is a perfect fit for apps like Trello and Storify

* [ react-content-loader](https://github.com/danilowoz/react-content-loader) - SVG powered component to easily create skeleton loadings(like Facebook’s card loading).

* [antd](https://ant.design) - Ant Design - A design system for enterprise-level products. Create an efficient and enjoyable work experience.

* [Flux](https://facebook.github.io/flux/) - Application architecture for building user interfaces
