# npmtest-ts-node

#### basic test coverage for  [ts-node (v3.0.2)](https://github.com/TypeStrong/ts-node)  [![npm package](https://img.shields.io/npm/v/npmtest-ts-node.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-ts-node) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-ts-node.svg)](https://travis-ci.org/npmtest/node-npmtest-ts-node)

#### TypeScript execution environment and REPL for node

[![NPM](https://nodei.co/npm/ts-node.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/ts-node)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-ts-node/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-ts-node/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-ts-node/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-ts-node/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-ts-node/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-ts-node/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-ts-node/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-ts-node/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-ts-node/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-ts-node/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-ts-node/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-ts-node/build/test-report.html](https://npmtest.github.io/node-npmtest-ts-node/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-ts-node/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-ts-node/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-ts-node/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-ts-node/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ts-node/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ts-node/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-ts-node/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-ts-node/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Blake Embrey",
        "url": "http://blakeembrey.me"
    },
    "bin": {
        "ts-node": "dist/bin.js"
    },
    "bugs": {
        "url": "https://github.com/TypeStrong/ts-node/issues"
    },
    "dependencies": {
        "arrify": "^1.0.0",
        "chalk": "^1.1.1",
        "diff": "^3.1.0",
        "make-error": "^1.1.1",
        "minimist": "^1.2.0",
        "mkdirp": "^0.5.1",
        "source-map-support": "^0.4.0",
        "tsconfig": "^6.0.0",
        "v8flags": "^2.0.11",
        "yn": "^1.2.0"
    },
    "description": "TypeScript execution environment and REPL for node",
    "devDependencies": {
        "chai": "^3.0.0",
        "istanbul": "^0.4.0",
        "mocha": "^3.0.0",
        "ntypescript": "^1.201507091536.1",
        "proxyquire": "^1.7.2",
        "rimraf": "^2.5.4",
        "semver": "^5.1.0",
        "tslint": "^4.0.2",
        "tslint-config-standard": "^4.0.0",
        "typescript": "^2.1.4",
        "typings": "^2.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "cfc9516c831b920d7efbe16005915062b1294f8c",
        "tarball": "https://registry.npmjs.org/ts-node/-/ts-node-3.0.2.tgz"
    },
    "engines": {
        "node": ">=4.2.0"
    },
    "files": [
        "dist/",
        "typings.js",
        "register.js",
        "LICENSE"
    ],
    "gitHead": "b6f4ed71b7a845b98f17ba3b2bd70c1ed86dbf7f",
    "homepage": "https://github.com/TypeStrong/ts-node",
    "keywords": [
        "typescript",
        "node",
        "runtime",
        "environment",
        "ts",
        "compiler"
    ],
    "license": "MIT",
    "main": "dist/index.js",
    "maintainers": [
        {
            "name": "blakeembrey"
        }
    ],
    "name": "ts-node",
    "optionalDependencies": {},
    "preferGlobal": true,
    "repository": {
        "type": "git",
        "url": "git://github.com/TypeStrong/ts-node.git"
    },
    "scripts": {
        "build": "npm run clean && npm run tsc",
        "clean": "rimraf dist",
        "lint": "tslint \"src/**/*.ts\"",
        "prepublish": "typings install && npm run build",
        "test": "npm run build && npm run lint && npm run test-cov",
        "test-cov": "istanbul cover node_modules/mocha/bin/_mocha -- \"dist/**/*.spec.js\" -R spec --bail",
        "test-spec": "mocha dist/**/*.spec.js -R spec --bail",
        "tsc": "tsc"
    },
    "version": "3.0.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
