# football-roster

## Introduction:

A PES Auction ReactJS app focuses on the core concepts ReactJS and uses Google's material design. It also integrates a NodeJS server. Also has the API support and handles CRUD operations.

## Pre-requisites:

- [NodeJS](https://nodejs.org/en/)

## Stack (Tools and Technologies):

- Technologies:
  - <b>ReactJS</b> - Main UI Library
  - <b>Javascript</b> - Scripting language
  - <b>Redux</b> - State management
  - <b>Redux Thunk</b> - Middleware
  - <b>AXIOS</b> - Promise based HTTP client (makes it easy to send asynchronous HTTP requests to REST endpoints and perform CRUD operations)
  - <b>SAAS (SCSS)</b> - Preprocessor for CSS
  - <b>NodeJS</b> - Server side scripting
  - <b>HTML</b> - Structuring the webpages
  - <b>JSX</b> - Allows combining XML/HTML and JS
  - <b>CSS</b> - Styling the webpages
  - <b>SAAS (SCSS)</b> - Preprocessor for CSS
  - <b>Materialize</b> - Modern and Responsive Design Framework
- Tools:
  - <b>Websotorm</b> - IDE (others can also be used like VS Code, Atom, etc)
  - <b>GitBash</b> - Version Control (emulation layer for Git command line interface on windows)
  - <b>Chrome</b> - Web Browser (others can also be used like Chrome, Safari, Firefox)

Setup:
------

In the project directory, you can run:

    npm install

This will install all the dev dependencies defined in the `package.json` file. Then run:

    npm start

Runs the app in the development mode.<br>
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits. You will also see any lint errors in the console.

<br>
To launch the test runner in the interactive watch mode, use:

    npm test
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

<br>
To build the app for production, use:

    npm run build
It builds the app for production to the `build` folder and correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.

<br>
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.


</br>

# Basic Concepts

React is a declarative, efficient, and flexible JavaScript library for building user interfaces. It lets you compose complex UIs from small and isolated pieces of code called “components”.

#### Advantages:

- Declarative
- Effiecient
  
  Because uses `vDOM` to reduce re renders. Functional components `reduces bundle` size. `Pure components` allow less re render levereging `componentDidUpdate` and only checking the shallow references of states/props

- Flexible
- Immutable

  Allows uni directional flow and immutability helps in reusing the components where changing the value of one doesnt affects other. Also a change in state triggers the re-render. Mutating the state/props then have side effects like comparison of prev/next props/states in lifecycle methods/hooks will reference to same objects. Using `concat` or `spread operator` helps avoiding mutation. 

  Mutating a state doesnt triggers a re render. This is because when we mutate, the object reference will still be the same and didUpdate's comparison will fail and results in preventing the re render. 
  
  Also, mutation leads to updating all the references which is not required.


#### Closure:
#### Asyncsronus:
#### Async await:
#### Is react synchronous/asynchrous and single/multi threaded:
#### Mutation:
#### Why react is faster than others:

### <b>Create react app</b>
  - ### <b>Installation:</b>
    Create a new directory for project, we'll name it `pes-app` and `cd` to it. Then execute:

        npx create-react-app pes_app

    Then if dependencies are defined after this, or in an existence project, to install the dev dependencies defined in the `package.json` file, run:

        npm install

    Then, we can run the app by executing:

        npm start

### <b>Webpack</b>

  Webpack also uses/has babel and apart from this, it also helps us bundle all the CSS/SASS/Images etc to file which browser understands and browser downloads that file at the time of page load.

  Also, the webpack combines all the modules (imports/exports) as at the end of the day, browser needs one big js file.


### <b>Babel</b>

  Converts ES6 to browser understandable vanilla/ES5 javascript. Its a transpiler/compiler. 

### <b>VDOM</b>
### <b>Class based components</b>
### <b>Functional components</b>
### <b>States</b>
### <b>Props</b>
### <b>Lifecycle methods in classes</b>
### <b>Lifecycle hooks in functional components</b>
### <b>Fragments</b>

  Lets us group multiple nodes w/o adding an extra node.

### <b>Lifting up the state</b>

  Shifting a components state to its parent so that other sibling components can also use it

### <b>Pure components</b>
  
  It does a shallow comparison on state change and avoid extra re renders leverging `componentDidUpdate`. It compares values when looking at primitive types and references for objects.

  However, two conditions should meet while working/creating a pure component:

  - Component State/Props is an immutable object
  - State/Props should not have a multi-level nested object

  Also, all the children of pure components should also be pure. 

### <b>Child to parent props</b>

  Use of callback methods passed as a prop to the children. When called in the child, returns control to the parent as a callback and can also get data in the params

### <b>Hooks</b>
  - useState
  - useEffect
  - useContext
  - useRef
  - useCallback
  - useReducer
  - useMemo
  - useImperativeHandle
  - useLayoutEffect
  - useDebugValue

### <b>Redux state management</b>
  - Actions types
  - Actions
  - Reducers

### <b>React router</b>
### <b>Protected routes</b>
### <b>Service worker</b>
### <b>Redux persist/localstorage</b>
### <b>Mutable/Immutable</b>
### <b>SSR</b>

  When the browser requests a page, the server loads React in the memory and fetches the data required to render the app. After that, the server sends generated HTML to the browser, which is immediately shown to the user.

## <b>Design Libraries</b>
- Material UI
