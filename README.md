# react-tutorial

https://reactjs.org/tutorial/tutorial.html

Step 1. Create application structure
```console
$ npx create-react-app my-app
$ mv my-app/* my-app/.gitignore .
$ rm -rf my-app
$ rm -rf src/*
$ touch src/index.css
$ touch src/indes.js
```

Add empty application contents to src/index.js
```javascript:src/index.js
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
