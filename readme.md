# React-Redux To Do App

Tech:
React, Redux, Webpack, SCSS/CSS/HTML

Branch basic
https://rajaraodv.medium.com/step-by-step-guide-to-building-react-redux-apps-using-mocks-48ca0f47f9a

1. Can filter by "active" or "completed"
2. basic UI - CSS

Branch advanced

1. can filter by "to do", "doing", "done"
2. better UI -- Use SCSS instead of CSS

```
npm i --save-dev babel-core babel-loader babel-preset-env babel-preset-es2015 babel-preset-react webpack webpack-cli webpack-dev-server

npm install -D babel-loader@7 babel-core babel-preset-env babel-preset-es2015 babel-preset-react webpack webpack-dev-server webpack-cli

npm i react redux react-redux

```

Steps:

1. Mock up screen
2. Divide app into components

- AddTodo
- TodoList
- Filter

3. List state and actions for each component
   a. AddTodo

- ADD_TODO - action
  b. TodoList
- Todos (array) - state
- VisibilityFilter (boolean) - state
- TOGGLE_TODO - action
  c. Filter
- CurrentFilter - state
- SET_VISIBILITY_FILTER - ACTION

4. Create action creators for each action
5. Write reducers for each action
6. Implement presentational components (react)
   a. AddTodoForm
   b. TodoList
   c. 3 Link Components (filters)
7. Create container component for components
   a. AddTodo
   b. TodoList
   c. Filter
8. Bring it together (create store, create App.js)

```
├── dist
│   ├── bundle.js
│   └── index.html
├── src
│   ├── actions
│   │   └── index.js
│   ├── app
│   │   └── store.js
│   ├── components
│   │   ├── AddTodoForm.js
│   │   ├── App.js
│   │   ├── Filter.js
│   │   ├── Link.js
│   │   ├── Todo.js
│   │   └── TodoList.js
│   ├── containers
│   │   ├── AddTodo.js
│   │   ├── FilterLink.js
│   │   └── VisibleTodoList.js
│   ├── index.js
│   └── reducers
│       ├── index.js
│       ├── todos.js
│       └── visibilityFilter.js
└── webpack.config.js

```
