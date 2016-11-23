This is temporary version of @ngtools/webpack package that doesn't strip off custom decorators from code.
It will be deprecated when https://github.com/angular/angular-cli/issues/2799 is resolved.

Get it from npm: 

`npm install --save ngtools-webpack-keep-decorators`

Change ngtools import:

`const ngtools = require('@ngtools/webpack')` => `const ngtools = require('ngtools-webpack-keep-decorators')`

And update your loader:

`loaders: ['@ngtools/webpack']` => `loaders: ['ngtools-webpack-keep-decorators']`
