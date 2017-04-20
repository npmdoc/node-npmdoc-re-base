# npmdoc-re-base

#### api documentation for  re-base (v2.7.0)  [![npm package](https://img.shields.io/npm/v/npmdoc-re-base.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-re-base) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-re-base.svg)](https://travis-ci.org/npmdoc/node-npmdoc-re-base)

#### A Relay inspired library for building React.js + Firebase applications.

[![NPM](https://nodei.co/npm/re-base.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/re-base)

- [https://npmdoc.github.io/node-npmdoc-re-base/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-re-base/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-re-base/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-re-base/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-re-base/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-re-base/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "re-base",
    "version": "2.7.0",
    "description": "A Relay inspired library for building React.js + Firebase applications.",
    "main": "index.js",
    "repository": {
        "type": "git",
        "url": "https://github.com/tylermcginnis/re-base"
    },
    "author": "Tyler McGinnis and Jacob Turner",
    "dependencies": {
        "firebase": "^3.5.2"
    },
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
    "scripts": {
        "build": "webpack",
        "test": "karma start tests/karma.conf.js",
        "travis": "./node_modules/karma/bin/karma start tests/karma.conf.js"
    },
    "license": "MIT"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
