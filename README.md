# npmdoc-composition

#### api documentation for  [composition (v2.3.0)](https://github.com/thenables/composition#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-composition.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-composition) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-composition.svg)](https://travis-ci.org/npmdoc/node-npmdoc-composition)

#### Compose generator and async/await middleware

[![NPM](https://nodei.co/npm/composition.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/composition)

- [https://npmdoc.github.io/node-npmdoc-composition/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-composition/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-composition/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-composition/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-composition/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-composition/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jonathan Ong",
        "url": "http://jongleberry.com"
    },
    "bugs": {
        "url": "https://github.com/thenables/composition/issues"
    },
    "dependencies": {
        "any-promise": "^1.1.0",
        "co": "^4.0.2"
    },
    "description": "Compose generator and async/await middleware",
    "devDependencies": {
        "bluebird": "^3.1.1",
        "istanbul": "^0.4.2",
        "koa-compose": "^2.3.0",
        "matcha": "^0.6.0",
        "mocha": "^2.0.0",
        "timeout-then": "^1.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "742805374cab550c520a33662f5a732e0208d6f2",
        "tarball": "https://registry.npmjs.org/composition/-/composition-2.3.0.tgz"
    },
    "files": [
        "index.js"
    ],
    "gitHead": "d3cd279c4ed45ceef59cdfb03e41190efbb92b23",
    "homepage": "https://github.com/thenables/composition#readme",
    "keywords": [
        "co",
        "compose",
        "composition",
        "middleware",
        "decorator",
        "decorators",
        "async",
        "await",
        "yield"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "jongleberry"
        },
        {
            "name": "coderhaoxin"
        }
    ],
    "name": "composition",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/thenables/composition.git"
    },
    "scripts": {
        "bench": "matcha bench/run.js",
        "test": "mocha --bail",
        "test-cov": "istanbul cover ./node_modules/.bin/_mocha -- --reporter dot",
        "test-travis": "istanbul cover ./node_modules/.bin/_mocha --report lcovonly -- --reporter dot"
    },
    "version": "2.3.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
