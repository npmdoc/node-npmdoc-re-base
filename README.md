# api documentation for  [re-base (v2.7.0)](https://github.com/tylermcginnis/re-base#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-re-base.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-re-base) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-re-base.svg)](https://travis-ci.org/npmdoc/node-npmdoc-re-base)
#### A Relay inspired library for building React.js + Firebase applications.

[![NPM](https://nodei.co/npm/re-base.png?downloads=true)](https://www.npmjs.com/package/re-base)

[![apidoc](https://npmdoc.github.io/node-npmdoc-re-base/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-re-base%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-re-base/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-re-base/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-re-base/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Tyler McGinnis and Jacob Turner"
    },
    "bugs": {
        "url": "https://github.com/tylermcginnis/re-base/issues"
    },
    "dependencies": {
        "firebase": "^3.5.2"
    },
    "description": "A Relay inspired library for building React.js + Firebase applications.",
    "devDependencies": {
        "babel-core": "^6.18.0",
        "babel-loader": "^6.2.7",
        "babel-preset-es2015": "^6.18.0",
        "babel-preset-react": "^6.16.0",
        "coveralls": "^2.11.14",
        "jasmine-core": "^2.5.2",
        "karma": "^1.3.0",
        "karma-chrome-launcher": "^2.0.0",
        "karma-coverage": "^1.1.1",
        "karma-failed-reporter": "0.0.3",
        "karma-firefox-launcher": "^1.0.0",
        "karma-jasmine": "^1.0.2",
        "karma-spec-reporter": "0.0.26",
        "karma-webpack": "^1.8.0",
        "node-libs-browser": "^1.0.0",
        "react": "^15.3.2",
        "react-dom": "^15.3.2",
        "webpack": "^1.13.3"
    },
    "directories": {},
    "dist": {
        "shasum": "a8adcba84ffb483d4f7a6b8ff343123c5d23d81c",
        "tarball": "https://registry.npmjs.org/re-base/-/re-base-2.7.0.tgz"
    },
    "gitHead": "4d40ef2fa05ab6e05f52ecdbb7a904121488dbf5",
    "homepage": "https://github.com/tylermcginnis/re-base#readme",
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "jisraelturner",
            "email": "j.israel.turner@gmail.com"
        },
        {
            "name": "qwales1",
            "email": "qwales1@gmail.com"
        },
        {
            "name": "tylermcginnis",
            "email": "tylermcginnis33@gmail.com"
        }
    ],
    "name": "re-base",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/tylermcginnis/re-base.git"
    },
    "scripts": {
        "build": "webpack",
        "test": "karma start tests/karma.conf.js",
        "travis": "./node_modules/karma/bin/karma start tests/karma.conf.js"
    },
    "version": "2.7.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module re-base](#apidoc.module.re-base)
1.  [function <span class="apidocSignatureSpan">re-base.</span>createClass (config)](#apidoc.element.re-base.createClass)



# <a name="apidoc.module.re-base"></a>[module re-base](#apidoc.module.re-base)

#### <a name="apidoc.element.re-base.createClass"></a>[function <span class="apidocSignatureSpan">re-base.</span>createClass (config)](#apidoc.element.re-base.createClass)
- description and source-code
```javascript
function createClass(config) {
	      var name = arguments.length > 1 && arguments[1] !== undefined ? arguments[1] : '[DEFAULT]';

	      if (typeof apps[name] !== 'undefined') {
	        return apps[name];
	      } else {
	        (0, _validators._validateConfig)(config);
	        var app = _firebase2.default.initializeApp(config, name);
	      }
	      apps[name] = init(app);
	      return apps[name];
	    }
```
- example usage
```shell
...
##### Return Value
  An instance of re-base.

##### Example

'''javascript
var Rebase = require('re-base');
var base = Rebase.createClass({
      apiKey: "apiKey",
      authDomain: "projectId.firebaseapp.com",
      databaseURL: "https://databaseName.firebaseio.com",
      storageBucket: "bucket.appspot.com",
      messagingSenderId: "xxxxxxxxxxxxxx"
}, 'myApp');
'''
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
