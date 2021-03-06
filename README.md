# starter-react-flux 

[![Build Status](https://travis-ci.org/SokichiFujita/starter-react-flux.svg?branch=master)](https://travis-ci.org/SokichiFujita/starter-react-flux) 
[![total](https://img.shields.io/npm/dt/starter-react-flux.svg)](https://www.npmjs.com/package/starter-react-flux) 
[![per year](https://img.shields.io/npm/dy/starter-react-flux.svg)](https://www.npmjs.com/package/starter-react-flux) 
[![per month](https://img.shields.io/npm/dm/starter-react-flux.svg)](https://www.npmjs.com/package/starter-react-flux) 
[![per week](https://img.shields.io/npm/dw/starter-react-flux.svg)](https://www.npmjs.com/package/starter-react-flux) 
[![GitHub license](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/SokichiFujita/starter-react-flux/blob/master/LICENSE) 
[![npm](https://img.shields.io/npm/v/starter-react-flux.svg)](https://www.npmjs.com/package/starter-react-flux) 
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](https://github.com/SokichiFujita/starter-react-flux/blob/master/README.md) 

A starter kit for a React and Flux. You can easily create a standard React and Flux project using awesome libraries.

- [React](http://facebook.github.io/react/), [Flux](https://facebook.github.io/flux/)
- [Jest](https://facebook.github.io/jest/)
- [Babel 7](https://babeljs.io)
  - [@babel/preset-react](http://babeljs.io/docs/plugins/preset-react/)
  - [@babel/preset-env](https://babeljs.io/docs/plugins/preset-env/)
  - All plugins for stage3, stage2, stage1 and stage0!
- [Webpack v4](https://webpack.js.org)
  - [Webpack-dev-server](https://webpack.github.io/docs/webpack-dev-server.html)
  - [Webpack Bundle Analyzer](https://github.com/webpack-contrib/webpack-bundle-analyzer)
- [Prettier](https://prettier.io)
- [ESLint v5](http://eslint.org),
  - [Airbnb JavaScript Style Guide](https://github.com/airbnb/javascript)
- [React-Router v4](https://reacttraining.com/react-router/)
- [Material-UI v3](http://www.material-ui.com)
- [Immutable.js](https://facebook.github.io/immutable-js/)
- [Axios](https://github.com/mzabriskie/axios)

starter-react-flux will install the latest versions.

## Usage

### Create a new project

```
mkdir my-app && cd my-app

//npm >= 5.2.0
npx starter-react-flux init

//npm < 5.2.0
npm install -g starter-react-flux
starter-react-flux init
```

### Launch the application

```
npm start                     // Launch the app with webpack-dev-server.
```

#### Top page with React and Flux

![](./images/app1.png)

#### Client side routing with React Router

![](./images/app2.png)

#### Bundle analyzing with Webpack Bundle Analyzer

```
npm run bundle-analyze
```

![](./images/webpack-bundle-analyzer.png)



#### Testing with Jest
```
npm test                      // Testing with Jest.
```

![](./images/test.png)


#### Static analyze with ESLint

```
npm run lint                  // Check the code by ESLint with AirBnb's style guideline.
```

![](./images/lint.png)

#### Automatic code format with Prettier and ESLint

```
npm run fix                   // Fix the code by Prettier with AirBnb's guidline.
```

![](./images/fix.png)



#### Production build with Webpack

```
npm run build                 // Build the app into the ./public directory.
```

## Directory structure of the generated app

```
.
├── .babelrc          //Configuration for Babel
├── .eslintrc         //Configuration for ESLint
├── __tests__         //Test files for JEST
├── app
│   ├── App.js        //Entry point
│   ├── actions       //Action Creators
│   ├── components    //React Components
│   ├── constants     //Constatns for Action Creators and Stores
│   ├── dispatcher    //Dispatcher
│   ├── stores        //Reduced Store
│   └── utils         //Utils
├── node_modules
├── package.json
├── public            //Build assets and other assets
│   ├── css
│   ├── img
│   ├── index.html
│   └── js
└── webpack.config.js //Configuration for Webpack
```

## Current Packages

### Nov.24, 2018: React Hooks APIs are available!

```
  "devDependencies": {
    "@babel/cli": "^7.1.5",
    "@babel/core": "^7.1.6",
    "@babel/plugin-proposal-class-properties": "^7.1.0",
    "@babel/plugin-proposal-decorators": "^7.1.6",
    "@babel/plugin-proposal-do-expressions": "^7.0.0",
    "@babel/plugin-proposal-export-default-from": "^7.0.0",
    "@babel/plugin-proposal-export-namespace-from": "^7.0.0",
    "@babel/plugin-proposal-function-bind": "^7.0.0",
    "@babel/plugin-proposal-function-sent": "^7.1.0",
    "@babel/plugin-proposal-json-strings": "^7.0.0",
    "@babel/plugin-proposal-logical-assignment-operators": "^7.0.0",
    "@babel/plugin-proposal-nullish-coalescing-operator": "^7.0.0",
    "@babel/plugin-proposal-numeric-separator": "^7.0.0",
    "@babel/plugin-proposal-optional-chaining": "^7.0.0",
    "@babel/plugin-proposal-pipeline-operator": "^7.0.0",
    "@babel/plugin-proposal-throw-expressions": "^7.0.0",
    "@babel/plugin-syntax-dynamic-import": "^7.0.0",
    "@babel/plugin-syntax-import-meta": "^7.0.0",
    "@babel/plugin-transform-runtime": "^7.1.0",
    "@babel/preset-env": "^7.1.6",
    "@babel/preset-react": "^7.0.0",
    "babel-core": "^7.0.0-0",
    "babel-eslint": "^10.0.1",
    "babel-jest": "^23.6.0",
    "babel-loader": "^8.0.4",
    "eslint": "^5.9.0",
    "eslint-config-airbnb": "^17.1.0",
    "eslint-config-prettier": "^3.3.0",
    "eslint-plugin-import": "^2.14.0",
    "eslint-plugin-jsx-a11y": "^6.1.2",
    "eslint-plugin-prettier": "^3.0.0",
    "eslint-plugin-react": "^7.11.1",
    "jest-cli": "^23.6.0",
    "prettier": "^1.15.2",
    "regenerator-runtime": "^0.13.1",
    "webpack": "^4.26.0",
    "webpack-bundle-analyzer": "^3.0.3",
    "webpack-cli": "^3.1.2",
    "webpack-dev-server": "^3.1.10"
  },
  "dependencies": {
    "@material-ui/core": "^3.5.1",
    "@material-ui/icons": "^3.0.1",
    "axios": "^0.18.0",
    "flux": "^3.1.3",
    "immutable": "^4.0.0-rc.12",
    "prop-types": "^15.5.7-alpha.1",
    "react": "^16.7.0-alpha.2",
    "react-dom": "^16.7.0-alpha.2",
    "react-router-dom": "^4.3.1"
  }
```

## License

- MIT License


