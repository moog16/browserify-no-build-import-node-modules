# browserify-no-build-import-node-modules

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
