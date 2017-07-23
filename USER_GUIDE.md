## User Guide

This file contains explainations for components in this template.

### Structure

|    Name    |                      Explanation                      |
|------------|-------------------------------------------------------|
| build      | Contains the compiled source files.                   |
| public     | Contains the static files to be served to the client. |
| src        | Contains the source files.                            |
| views      | Contains the front-end UI.                            |
| components | Contains React components.                            |
| .babelrc      | Babel config file                                                      |
| USER_GUIDE.md | This file.                                                             |
| package.json  | Contains the project information as well as dependencies.              |
| yarn.lock     | Auto-generated by the [Yarn](https://yarnpkg.com/en/) package manager. |

*For detail on the role of any file, you can read it inside the file. Pay attention to the 'NOTE' tag*

### Work Flow

In development, you mainly put your code inside 2 folders `src` and `views`.

To compile, run:
```
npm run build
```

To bundle and run the app, run:
```
npm start
```

To make the command above run automatically everytime you change your code, run:
```
npm run watch
```

### How it works

First, at the back-end, we use [Express](https://expressjs.com/) to serve the page (and optionally do server-side rendering).

The front-end is handled by [React](https://facebook.github.io/react/).

We use [Babel](https://babeljs.io/) to compile later version of Javascript into ES5 to support most browsers.

We also use webpack to merge all the files into a compact package in the `public` folder.

We then make the build automated by using [npm-watch](https://www.npmjs.com/package/npm-watch). We specified what to be "watched" inside section `watch` in `package.json`.
