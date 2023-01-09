# react-tutorial

https://reactjs.org/tutorial/tutorial.html

# Step 1. Create application structure
```console
$ npx create-react-app my-app
$ mv my-app/* my-app/.gitignore .
$ rm -rf my-app
$ rm -rf src/*
$ touch src/index.css
$ touch src/indes.js
```

Add empty application contents to src/index.js
```js:src/index.js
import React from 'react';
import ReactDOM from 'react-dom/client';
import './index.css';
```

Run server
```console
$ npm start
```

Check web<br/>
http://localhost:3000

# Step 2. Create base components

See code.

# Step 3. Making an Interactive Component

## Add onClick event function.

```js:src/index.js
class Square extends React.Component {
    render() {
        return (
            <button className="square" onClick={() => console.log('click')}>
                {this.props.value}
            </button>
        )
    };
}
```

## Add state property

```js:src/index.js
class Square extends React.Component {
    constructor(props) {
        super(props);
        this.state = {
            value: null,
        };
    }

    render() {
        return (
            <button
                className="square"
                onClick={() => this.setState({value: 'X'})}
            >
                {this.state.value}
            </button>
        )
    };
}
```
