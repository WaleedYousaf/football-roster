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

## React
- Create react app
  - ### <b>Installation:</b>
    Create a new directory for project, we'll name it `pes-app` and `cd` to it. Then execute:

        npx create-react-app pes_app

    Then if dependencies are defined after this, or in an existence project, to install the dev dependencies defined in the `package.json` file, run:

        npm install

    Then, we can run the app by executing:

        npm start

- Webpack
- Babel

  Converts ES6 to browser understandable vanilla script

- VDOM
- Class based components
- Functional components
- States
- Props
- Lifecycle methods in classes
- Lifecycle hooks in functional components
- Child to parent props

  Use of callback methods passed as a prop to the children. When called in the child, returns control to the parent as a callback and can also get data in the params

- Hooks
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

- Redux state management
  - Actions types
  - Actions
  - Reducers

- React router
- Protected routes
- Service worker
- Redux persist/localstorage
- Mutable/Immutable

## Design Libraries
- Material UI
