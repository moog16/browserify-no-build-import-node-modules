# browserify-no-build-import-node-modules

This is an example to illustrate that exporting ES6 modules is a problem. The solution is use package.json's main property to point to an ES5 file as described below.


This project includes the node_modules already, so DO NOT `npm install` or `yarn`. Instead do:

```
yarn build;
```

* Notice the build error
* To fix, open file: `./node_modules/@material/textfield/package.json`
  * update "main" to:
  
```
{
  ...
  "main": "./dist/mdc.textfield.js",
  ...
}
```

Working build project: https://github.com/moog16/browserify-build-import-node-modules/tree/master


