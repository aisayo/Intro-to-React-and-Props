# Intro to React and Props

## What is React? :thinking:

* A JavaScript library, not a framework
* An open source project created by Facebook
* Used to build front end user interfaces
* The view layer of the MVC application
* Component based and uses state and props to streamline how data is stored and used
* You can use a small part of React in website or build interactive SPA with React
* [React JS Docs](https://reactjs.org/)

## React Features

* Virtual DOM - allows for fast, efficient, content rendering [Doc](https://reactjs.org/docs/faq-internals.html#:~:text=The%20virtual%20DOM%20(VDOM)%20is,This%20process%20is%20called%20reconciliation.&text=They%20may%20also%20be%20considered,virtual%20DOM%E2%80%9D%20implementation%20in%20React.)
* Declarative writing structure - allows you to simply express how your app should look and let React handle updates and underlying data changes
* Babel - transpiler that converts modern JavaScript and custom code like JSX into more widely compatible JavaScript; [Doc](https://babeljs.io/docs/en/)
* Webpack - a 'bundler' that takes all our work, along with any required dependency code, and packages it all up in a single, transferable bundle [Doc](https://webpack.js.org/)
* ESLint - helps improve our code [Doc](https://eslint.org/docs/user-guide/getting-started)

## Working with React

### Add React to an existing project

* Need to add 3 CDN’s: React, React DOM, Babel
* React: the top level React API
* React DOM: adds DOM specific methods
* Babel: JS compiler that allows use of ES6 in older browsers

#### Inside index.html file

* Add a div with a root id

 ```<div id="root"></div>```

* Add script tag where react code will live

```
  <body>
    <div id="root"></div>

    <script type="text/babel">
      // React code will go here
    </script>
  </body>
```

### Creating a React app

* ```Npx create-react-app <name of app>```

## React consists of many Components

- “Components let you split the UI into independent, reusable pieces, and think about each piece in isolation.”
- Almost everything in React consists of components
- Used to house modularized front end code
- Like custom, reusable html elements
- Can be class or simple components

## JSX

- JavaScript XML
- Looks like HTML but it’s more JS
- Produces React elements
- [Babel Repl](https://babeljs.io/repl/#?browsers=defaults%2C%20not%20ie%2011%2C%20not%20ie_mob%2011&build=&builtIns=false&spec=false&loose=false&code_lz=MYewdgzgLgBApgGzgWzmWBeGAeAFgRgD4AJRBEAGhgHcQAnBAEwEJsB6AwgbgChRJY_KAEMAlmDh0YWRiGABXVOgB0AczhQAokiVQAQgE8AkowAUAcjogQUcwEpeAJTjDgUACIB5ALLK6aRklTRBQ0KCohMQk6Bx4gA&debug=false&forceAllTransforms=false&shippedProposals=false&circleciRepo=&evaluate=false&fileSize=false&timeTravel=false&sourceType=module&lineWrap=true&presets=react&prettier=false&targets=&version=7.11.1&externalPlugins=)

## Props

- Component properties
- Allow us to pass values into our components
- Allow components to be dynamic and reusable
- Accessible with ```this.props``` in class components
- In simple components: ```props.<name of prop>```
- Read only, can not be changed by component
- Can be any datatype: strings, booleans, numbers, object or function

## Good to know :thought_balloon:

```ReactDOM.render(<App />, document.getElementById('root'))```

- Renders a React element into DOM [ReactDOM Render function](https://reactjs.org/docs/react-dom.html#render)
- Everything inside of a React root DOM node is managed by ReactDOM
- Most React applications only call this one time in entire app
- React DOM compares the element and its children to the previous one, and only applies the DOM updates necessary to bring the DOM to the desired state

```{JS Expressions}```

- Anything that returns a value
- [Mozilla Doc](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#Expressions)

```React Devtools```

- [Chrome Extension](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi)

```React Elements```
- Anything you want to see on the screen
- Not components! Components are made of elements
- Represents the UI at a certain point in time
- Immutable, only way to update UI is to create new element