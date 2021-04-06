# React Resources

* [Ultimate React JS Starter Guide](https://medium.com/javascript-in-plain-english/how-i-learned-react-js-as-a-noob-ultimate-react-js-starter-guide-36a05ab9495e)

* [React Cheat Sheet](https://reactcheatsheet.com) - React cheat sheet with search  

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

* [Organizing React Projects](https://dev.to/chrisachard/tips-for-organizing-react-projects-191)

* [Javascript Closures and React](https://medium.com/swlh/javascript-closures-and-react-4c0e3f705a6c)

* [Simple tips for writing clean React components](https://itnext.io/simple-tips-for-writing-clean-react-components-c3facbf6680e)

## Best Practices

* Keep files to 200 lines or less
* Move helper functions into a separate `component.utils.ts` file and constants into a `component.constants.ts` file to make the component smaller and easier to read.
* Destructure props so you aren't writing 'props' everywhere.
  ```js
    // Don't repeat props everywhere :(
    const Input = (props) => {
      return <input value={props.value} onChange={props.onChange}/>
    }

    // Destructure and use the straight values :)
    const Input = ({value, onChange}) => (
      <input value={value} onChange={onChange} />
    )
  ```
* Avoid nesting render functions
* Short circuit operators are a very short and easy way to do conditional rendering:
  ```js
    // Short circuit operator
    const Counter = ({count}) => {
      return <div>
        {count && <h1>Count: {count}</h1>}
      </div>
    }
  ```
* Assign default props when destructuring
* Move lists into separate components
  ```js
    // Don't write lops with the rest of the code
    const Component = ({title, cards}) => {
      return <div>
        <h1>{title}</h1>
        {
          cards.map(({title: cardTitle, subtitle, image}) => ({
            <div>
              <h3>{cardTitle}</h3>
              <h5>{subtitle}</h5>
              <img src={image} />
            </div>
          }))
        }
      </div>
    }

    // Break it up into a separate list component
    const Component = ({title, cards}) => {
      return <div>
        <h1>{title}</h1>
        <CardsList cards={cards} />
      </div>
    }
  ```

## Useful Libraries

* [react-select](https://react-select.com/home) - A flexible and beautiful Select Input control for ReactJS with multiselect, autocomplete, async and creatable support.

* [react-dnd](https://react-dnd.github.io/react-dnd/about) - React DnD is a set of React utilities to help you build complex drag and drop interfaces while keeping your components decoupled. It is a perfect fit for apps like Trello and Storify

* [react-content-loader](https://github.com/danilowoz/react-content-loader) - SVG powered component to easily create skeleton loadings(like Facebook’s card loading).

* [antd](https://ant.design) - Ant Design - A design system for enterprise-level products. Create an efficient and enjoyable work experience.

* [Flux](https://facebook.github.io/flux/) - Application architecture for building user interfaces

* Form handling libraries:
  * [Formik](https://formik.org) - Formik is the world's most popular open source form library for React and React Native.
  * [React Hook Form](https://react-hook-form.com) - Performant, flexible and extensible forms with easy-to-use validation.

  * [Chakra UI](https://chakra-ui.com) - Chakra UI is a simple, modular and accessible component library that gives you the building blocks you need to build your React applications.
