# component-mocker

This package provides functionality for mocking objects easily (including functions and classes).
It has been extracted from [jest](https://github.com/facebook/jest).
You can find detailed documentation in the `index.js` file.
The LICENSE and PATENTS files are copies from the jest project.

## Example usage

```javascript
var mocker = require('component-mocker');
var myModule = ...; // Your module that you want to mock
var myModuleMetadata = mocker.getMetadata(myModule);
var myModuleMock = mocker.generateFromMetadata(myModuleMetadata);
```

## In browser usage

You can also use the `index.js` script in the browser.
The module is then available on the global scope under the name `mocker`.
You can also run it in no conflict mode by calling `var mocker = mocker.noConflict()`.
