# npmtest-axios-es6

#### basic test coverage for  [axios-es6 (v0.11.1)](https://github.com/mzabriskie/axios)  [![npm package](https://img.shields.io/npm/v/npmtest-axios-es6.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-axios-es6) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-axios-es6.svg)](https://travis-ci.org/npmtest/node-npmtest-axios-es6)

#### Promise based HTTP client for the browser and node.js

[![NPM](https://nodei.co/npm/axios-es6.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/axios-es6)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-axios-es6/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-axios-es6/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-axios-es6/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-axios-es6/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-axios-es6/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-axios-es6/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-axios-es6/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-axios-es6/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-axios-es6/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-axios-es6/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-axios-es6/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-axios-es6/build/test-report.html](https://npmtest.github.io/node-npmtest-axios-es6/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-axios-es6/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-axios-es6/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-axios-es6/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-axios-es6/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-axios-es6/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-axios-es6/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-axios-es6/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-axios-es6/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "axios-es6",
    "version": "0.11.1",
    "description": "Promise based HTTP client for the browser and node.js",
    "main": "index.js",
    "scripts": {
        "test": "grunt test",
        "start": "node ./sandbox/server.js",
        "build": "NODE_ENV=production grunt build",
        "preversion": "npm test",
        "version": "npm run build && grunt version && git add -A dist && git add CHANGELOG.md bower.json package.json",
        "postversion": "git push && git push --tags",
        "examples": "node ./examples/server.js",
        "coveralls": "cat coverage/lcov.info | ./node_modules/coveralls/bin/coveralls.js"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/mzabriskie/axios.git"
    },
    "keywords": [
        "xhr",
        "http",
        "ajax",
        "promise",
        "node"
    ],
    "author": "Matt Zabriskie",
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/mzabriskie/axios/issues"
    },
    "homepage": "https://github.com/mzabriskie/axios",
    "devDependencies": {
        "coveralls": "2.11.8",
        "es6-promise": "3.1.2",
        "grunt": "0.4.5",
        "grunt-banner": "0.6.0",
        "grunt-cli": "0.1.13",
        "grunt-contrib-clean": "1.0.0",
        "grunt-contrib-nodeunit": "1.0.0",
        "grunt-contrib-watch": "0.6.1",
        "grunt-eslint": "18.0.0",
        "grunt-karma": "0.12.1",
        "grunt-ts": "5.3.2",
        "grunt-webpack": "1.0.11",
        "istanbul-instrumenter-loader": "^0.2.0",
        "jasmine-core": "2.4.1",
        "karma": "0.13.21",
        "karma-chrome-launcher": "^0.2.2",
        "karma-coverage": "0.5.4",
        "karma-firefox-launcher": "^0.1.7",
        "karma-jasmine": "0.3.7",
        "karma-jasmine-ajax": "0.1.13",
        "karma-opera-launcher": "^0.3.0",
        "karma-phantomjs-launcher": "1.0.0",
        "karma-safari-launcher": "^0.1.1",
        "karma-sauce-launcher": "^0.3.1",
        "karma-sinon": "1.0.4",
        "karma-sourcemap-loader": "0.3.7",
        "karma-webpack": "1.7.0",
        "load-grunt-tasks": "3.4.1",
        "minimist": "1.2.0",
        "phantomjs-prebuilt": "2.1.6",
        "sinon": "1.17.3",
        "webpack": "1.12.14",
        "webpack-dev-server": "1.14.1"
    },
    "browser": {
        "./lib/adapters/http.js": "./lib/adapters/xhr.js"
    },
    "typescript": {
        "definition": "./axios.d.ts"
    },
    "dependencies": {
        "follow-redirects": "0.0.7"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
