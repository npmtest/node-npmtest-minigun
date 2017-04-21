# npmtest-minigun

#### basic test coverage for  minigun (v1.3.4)  [![npm package](https://img.shields.io/npm/v/npmtest-minigun.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-minigun) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-minigun.svg)](https://travis-ci.org/npmtest/node-npmtest-minigun)

#### Load-testing for HTTP and WebSocket-based applications

[![NPM](https://nodei.co/npm/minigun.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/minigun)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-minigun/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-minigun/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-minigun/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-minigun/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-minigun/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-minigun/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-minigun/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-minigun/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-minigun/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-minigun/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-minigun/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-minigun/build/test-report.html](https://npmtest.github.io/node-npmtest-minigun/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-minigun/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-minigun/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-minigun/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-minigun/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-minigun/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-minigun/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-minigun/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-minigun/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "minigun",
    "version": "1.3.4",
    "description": "Load-testing for HTTP and WebSocket-based applications",
    "main": "./bin/minigun",
    "engines": {
        "node": ">= 4.2.0"
    },
    "scripts": {
        "test": "bash test/runner.sh",
        "is_formatted": "find . -name '*.js' | grep -v node_modules | grep -v coverage | xargs jscs --preset=google",
        "is_linted": "find . -name '*.js' | grep -v node_modules | grep -v coverage | xargs eslint",
        "coverage": "ISTANBUL=y npm test && istanbul check-coverage",
        "postinstall": "echo '******* Minigun is now Artillery. Install with: npm install -g artillery. https://artillery.io *******'"
    },
    "keywords": [
        "load testing",
        "stress testing",
        "benchmark",
        "performance",
        "blackbox testing"
    ],
    "author": "Hassy Veldstra <h@veldstra.org>",
    "contributors": [
        "Kieran Gorman (https://github.com/kjgorman)"
    ],
    "license": "ISC",
    "preferGlobal": true,
    "man": "./man/minigun.1",
    "bin": {
        "minigun": "./bin/minigun"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/shoreditch-ops/minigun.git"
    },
    "bugs": {
        "url": "https://github.com/shoreditch-ops/minigun/issues"
    },
    "dependencies": {
        "async": "^1.0.0",
        "cli": "^0.6.6",
        "commander": "^2.8.1",
        "csv-parse": "^0.1.1",
        "debug": "^2.2.0",
        "lodash": "^3.9.1",
        "minigun-core": "latest",
        "open": "0.0.5",
        "yamljs": "^0.2.4"
    },
    "devDependencies": {
        "bats": "^0.4.2",
        "eslint": "^0.21.2",
        "good": "^6.4.0",
        "good-console": "^5.2.0",
        "hapi": "^12.1.0",
        "istanbul": "^0.3.14",
        "jscs": "^2.3.0",
        "pre-commit": "^1.0.7",
        "tape": "^4.0.0",
        "uuid": "^2.0.1"
    },
    "pre-commit": [
        "is_linted"
    ]
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
