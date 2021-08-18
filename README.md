# football-roster

## Introduction:

A PES Auction ReactJS app focuses on the core concepts ReactJS and uses Google's material design. It also integrates a NodeJS server. Also has the API support and handles CRUD operations.

## Pre-requisites:

- NodeJS (https://nodejs.org/en/)

## Stack (Tools and Technologies):

- Technologies:
  - <b>ReactJS</b> - Main UI Library
  - <b>Javascript</b> - Scripting language
  - <b>Redux</b> - State management
  - <b>Redux Thunk</b> - Middleware
  - <b>ESLint</b> - Code linting and analysis
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
  - <b>GitBash</b> - Version Control
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

## Javascript
- Classes
- Functions
- Inheritence (`extends`)

  Inherits properties/functions from its parent class

- Interfaces (`has`)

  Defines a shape objects/classes can take

- Abstraction
- JS methods
  - forEach
  - map
  - shift
  - unshift
  - splice
  - reduce
    
    Takes 2 arguments, the first one is a callback method, which further takes
    two arguments where first one is the `total` or `accumalator` and second 
    one is the `current` of this iteration, where and second parameter of reduce
    is the initial value of accumalator. It returns a single value

        const myReducedArray = myArray.reduce((total, item) => total + (item.num1 + item.num2), 0) 

- Pure components
- HOCs

  Its a function that either takes a function as a parameter or returns a function

   - Function accepting a function

          document.addEventListener("click", () => myFunction());
  - Function returning a function

          const createMultiplier = (multiplier) => {
            return (x) => {
              return x * multiplier
            }
          };

          // OR

          const createMultiplier = (multiplier) => (x) => x * multiplier;

          let doubleMe = createMultiplier(2);
          let tripleMe = createMultiplier(3);
      In JS, functions are considered as first class citizens like numbers, 
      strings and we can assign a variable or a const a function. We can pass
      them as a param and can return them from functions
  - Popular HOCs
      
      - forEach()
      - map()
      - filter()
      - reduce()
      - sort()

- lodash


## Middlewares

## APIs
- CRUD
- Axios
- REST Arch & RestFul APIs

## Design Libraries
- Material UI
- ANTd

## Linting
- ESLint

## CSS/SAAS
- SCSS

  Sass is a preprocessor scripting language that is interpreted or compiled into Cascading Style Sheets

- Media queries

  It uses the @media rule to include a block of CSS properties only if a certain condition is true

      /* For mobile phones: */
      [class*="col-"] {
        width: 100%;
      }

      @media only screen and (min-width: 600px) {
        /* For tablets: */
        .col-s-1 {width: 8.33%;}
        .col-s-2 {width: 16.66%;}
        .col-s-3 {width: 25%;}
        .col-s-4 {width: 33.33%;}
        .col-s-5 {width: 41.66%;}
        .col-s-6 {width: 50%;}
        .col-s-7 {width: 58.33%;}
        .col-s-8 {width: 66.66%;}
        .col-s-9 {width: 75%;}
        .col-s-10 {width: 83.33%;}
        .col-s-11 {width: 91.66%;}
        .col-s-12 {width: 100%;}
      }

      @media only screen and (min-width: 768px) {
        /* For desktop: */
        .col-1 {width: 8.33%;}
        .col-2 {width: 16.66%;}
        .col-3 {width: 25%;}
        .col-4 {width: 33.33%;}
        .col-5 {width: 41.66%;}
        .col-6 {width: 50%;}
        .col-7 {width: 58.33%;}
        .col-8 {width: 66.66%;}
        .col-9 {width: 75%;}
        .col-10 {width: 83.33%;}
        .col-11 {width: 91.66%;}
        .col-12 {width: 100%;}
      } 

- mixin
  
  They allow us to write reusable styles. We can pass variables as well to intanciate them at run time like

      @mixin important-text {
        color: red;
        font-size: 25px;
        font-weight: bold;
        border: 1px solid blue;
      }
      
      .danger {
        @include important-text;
        background-color: green;
      }

## Test Cases
- JEST
- Enzymes

## JWTs

## JSON Server
 - ### <b>Installation:</b>

    To install, go in any project folder or install it globally using `-g` like

        npm install -g json-server

    To run, execute command

        json-server --watch db.json --port 3001

    where `db.json` can have static json

## Express Server
- ### <b>Installation</b>
    Can install in any empty directory. Just cd into a folder and create a new dir, we'll create `pes-app`
		  
        mkdir pes-app
			  
    cd to `pes-app` and execute

		npm init --yes
    
    This will create `pcakage.json` in this folder i.e. `pes-app`. Then, create server.js file in root dir of `pes-app`.
    We can install (optional) `nodemon` to terminate and restart the server i.e. server.js after each change. We can execute command:
		
        npm i -g nodemon
    
    After installing, we can start it by executing:

		nodemon server.js
			  
    For setting environment var PORT and using in server.js, execute:

        set PORT=3006
			  
    Use server.js for HTTP requests i.e. GET, POST. For validation use joi library

## Sockets
- sockets.io
