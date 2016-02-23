Tuto react EGGHEAD

# Environment
Create son file on the folder project:
	npm init

Install:
	npm install react react-dom --save
	npm install babel webpack webpack-dev-server
	npm install babel-loader babel-core babel-preset-es2015 babel-preset-react

## The estructure of react:
- App.js:
  ```
  import React from 'react';
  class App extends React.Component {
    render(){
      return <div>¡Hola Pelucho!</div>
    }
  }
  export default App
  ```

- main.js:
  ```
  import React from 'react';
  import ReactDOM from 'react-dom';
  import App from './App';
  ReactDOM.render(<App />, document.getElementById('app'))
  ```
- index.html:
  ```
  <!DOCTYPE html>
  <html lang="es">
    <head>
      <meta charset="utf-8">
      <title>Setup</title>
    </head>
    <body>
      <div id="app"></div>
      <script src="index.js"></script>
    </body>
  </html>
  ```

### The configuration files:
- package.json:
  ```
  {
    "name":
    "version":
    "description":
    "main":
    "dependencies": {......},
    "devDependencies": {},
    "repository"
    "scripts": {},
    "author":
    "license":
  }
  ```
- webpack.config.js:
  ```
  module.exports = {
    entry: './main.js',
    output: {..},
    devServer: {..},
    module: {
      loaders: [{........}]
    }
  }
  ```
