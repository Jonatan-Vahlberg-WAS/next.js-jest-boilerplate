# Next.js + jest + testing-library boilerplate code

This project serves the singular function of being a clonable repository for quick start to a Next.js project

## Notable changes
first and foremost is the imports in [package.json](package.json)
```json
"dependencies": {
    "@types/jest": "^27.0.1",
    "jest": "^27.0.6",
  },
"devDependencies": {
    "@testing-library/dom": "^8.1.0",
    "@testing-library/jest-dom": "^5.14.1",
    "@testing-library/react": "^12.0.0",
    "@testing-library/user-event": "^13.2.1",
    "babel-jest": "^27.0.6",
  }
```
There are also some commands namely `npm run test(:watch)`.

A .bablerc have to be added for compiling the tests

finally jest itself the setup and config for using them resides in [jest.config.js](jest.config.js) and  [jest.setup.ts](jest.setup.ts)

## Inorder to run tests using this library
append at the top of .spec.ts(x) or .test.ts(x) file this jest enviroment [declaration](https://jestjs.io/docs/configuration#testenvironment-string)

```js
/**
 * @jest-environment jsdom
 */

```

## Clone repository
If you clone this repository change the **name** field in [package.json](package.json)
