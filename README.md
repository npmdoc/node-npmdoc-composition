# api documentation for  [composition (v2.3.0)](https://github.com/thenables/composition#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-composition.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-composition) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-composition.svg)](https://travis-ci.org/npmdoc/node-npmdoc-composition)
#### Compose generator and async/await middleware

[![NPM](https://nodei.co/npm/composition.png?downloads=true)](https://www.npmjs.com/package/composition)

[![apidoc](https://npmdoc.github.io/node-npmdoc-composition/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-composition%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-composition/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-composition/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-composition/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jonathan Ong",
        "email": "me@jongleberry.com",
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
            "name": "jongleberry",
            "email": "jonathanrichardong@gmail.com"
        },
        {
            "name": "coderhaoxin",
            "email": "coderhaoxin@outlook.com"
        }
    ],
    "name": "composition",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
    "version": "2.3.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module composition](#apidoc.module.composition)
1.  [function <span class="apidocSignatureSpan">composition.</span>Wrap (fn, ctx, next)](#apidoc.element.composition.Wrap)
1.  object <span class="apidocSignatureSpan">composition.</span>Wrap.prototype

#### [module composition.Wrap](#apidoc.module.composition.Wrap)
1.  [function <span class="apidocSignatureSpan">composition.</span>Wrap (fn, ctx, next)](#apidoc.element.composition.Wrap.Wrap)

#### [module composition.Wrap.prototype](#apidoc.module.composition.Wrap.prototype)
1.  [function <span class="apidocSignatureSpan">composition.Wrap.prototype.</span>_getGenerator ()](#apidoc.element.composition.Wrap.prototype._getGenerator)
1.  [function <span class="apidocSignatureSpan">composition.Wrap.prototype.</span>_getPromise ()](#apidoc.element.composition.Wrap.prototype._getPromise)
1.  [function <span class="apidocSignatureSpan">composition.Wrap.prototype.</span>_getValue ()](#apidoc.element.composition.Wrap.prototype._getValue)
1.  [function <span class="apidocSignatureSpan">composition.Wrap.prototype.</span>catch (reject)](#apidoc.element.composition.Wrap.prototype.catch)
1.  [function <span class="apidocSignatureSpan">composition.Wrap.prototype.</span>next (val)](#apidoc.element.composition.Wrap.prototype.next)
1.  [function <span class="apidocSignatureSpan">composition.Wrap.prototype.</span>then (resolve, reject)](#apidoc.element.composition.Wrap.prototype.then)
1.  [function <span class="apidocSignatureSpan">composition.Wrap.prototype.</span>throw (err)](#apidoc.element.composition.Wrap.prototype.throw)



# <a name="apidoc.module.composition"></a>[module composition](#apidoc.module.composition)

#### <a name="apidoc.element.composition.Wrap"></a>[function <span class="apidocSignatureSpan">composition.</span>Wrap (fn, ctx, next)](#apidoc.element.composition.Wrap)
- description and source-code
```javascript
function Wrap(fn, ctx, next) {
  if (typeof fn !== 'function') throw TypeError('Not a function!');
  this._fn = fn;
  this._ctx = ctx;
  this._next = next;
  this._called = false;
  this._value = undefined;
  this._promise = undefined;
  this._generator = undefined;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.composition.Wrap"></a>[module composition.Wrap](#apidoc.module.composition.Wrap)

#### <a name="apidoc.element.composition.Wrap.Wrap"></a>[function <span class="apidocSignatureSpan">composition.</span>Wrap (fn, ctx, next)](#apidoc.element.composition.Wrap.Wrap)
- description and source-code
```javascript
function Wrap(fn, ctx, next) {
  if (typeof fn !== 'function') throw TypeError('Not a function!');
  this._fn = fn;
  this._ctx = ctx;
  this._next = next;
  this._called = false;
  this._value = undefined;
  this._promise = undefined;
  this._generator = undefined;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.composition.Wrap.prototype"></a>[module composition.Wrap.prototype](#apidoc.module.composition.Wrap.prototype)

#### <a name="apidoc.element.composition.Wrap.prototype._getGenerator"></a>[function <span class="apidocSignatureSpan">composition.Wrap.prototype.</span>_getGenerator ()](#apidoc.element.composition.Wrap.prototype._getGenerator)
- description and source-code
```javascript
_getGenerator = function () {
  if (this._generator === undefined) {
    var value = this._getValue();
    this._generator = isGenerator(value)
      ? value
      : promiseToGenerator.call(this._ctx, value);
  }
  return this._generator
}
```
- example usage
```shell
...
* 'yield*' works on the '[@@iterator]' method.
*
* @returns {Iterator}
*/

if (typeof Symbol !== 'undefined') {
 Wrap.prototype[Symbol.iterator] = function () {
   return this._getGenerator();
 }
}

/**
* This creates a generator from a promise or a value.
*
* TODO: try to avoid using a generator function for this.
...
```

#### <a name="apidoc.element.composition.Wrap.prototype._getPromise"></a>[function <span class="apidocSignatureSpan">composition.Wrap.prototype.</span>_getPromise ()](#apidoc.element.composition.Wrap.prototype._getPromise)
- description and source-code
```javascript
_getPromise = function () {
  if (this._promise === undefined) {
    var value = this._getValue();
    this._promise = isGenerator(value)
      ? co.call(this._ctx, value)
      : Promise.resolve(value);
  }
  return this._promise
}
```
- example usage
```shell
...
}

/**
 * Proxy generator and promise methods.
 */

Wrap.prototype.then = function (resolve, reject) {
  return this._getPromise().then(resolve, reject);
}

Wrap.prototype.catch = function (reject) {
  return this._getPromise().catch(reject);
}

Wrap.prototype.next = function (val) {
...
```

#### <a name="apidoc.element.composition.Wrap.prototype._getValue"></a>[function <span class="apidocSignatureSpan">composition.Wrap.prototype.</span>_getValue ()](#apidoc.element.composition.Wrap.prototype._getValue)
- description and source-code
```javascript
_getValue = function () {
  if (!this._called) {
    this._called = true;
    try {
      this._value = this._fn.call(this._ctx, this._next);
    } catch (e) {
      this._value = Promise.reject(e);
    }
  }
  return this._value
}
```
- example usage
```shell
...
 * Lazily create a promise from the return value.
 *
 * @returns {Promise}
 */

Wrap.prototype._getPromise = function () {
  if (this._promise === undefined) {
    var value = this._getValue();
    this._promise = isGenerator(value)
      ? co.call(this._ctx, value)
      : Promise.resolve(value);
  }
  return this._promise
}
...
```

#### <a name="apidoc.element.composition.Wrap.prototype.catch"></a>[function <span class="apidocSignatureSpan">composition.Wrap.prototype.</span>catch (reject)](#apidoc.element.composition.Wrap.prototype.catch)
- description and source-code
```javascript
catch = function (reject) {
  return this._getPromise().catch(reject);
}
```
- example usage
```shell
...

// compose it into a function
var fn = compose(stack);

// this function returns a promise
fn.call(this).then(function (val) {
  console.log(val);
}).catch(function (err) {
  console.error(err.stack);
  process.exit(1);
})
'''

[gitter-image]: https://badges.gitter.im/thenables/composition.png
[gitter-url]: https://gitter.im/thenables/composition
...
```

#### <a name="apidoc.element.composition.Wrap.prototype.next"></a>[function <span class="apidocSignatureSpan">composition.Wrap.prototype.</span>next (val)](#apidoc.element.composition.Wrap.prototype.next)
- description and source-code
```javascript
next = function (val) {
  return this._getGenerator().next(val);
}
```
- example usage
```shell
...
}

Wrap.prototype.catch = function (reject) {
  return this._getPromise().catch(reject);
}

Wrap.prototype.next = function (val) {
  return this._getGenerator().next(val);
}

Wrap.prototype.throw = function (err) {
  return this._getGenerator().throw(err);
}

/**
...
```

#### <a name="apidoc.element.composition.Wrap.prototype.then"></a>[function <span class="apidocSignatureSpan">composition.Wrap.prototype.</span>then (resolve, reject)](#apidoc.element.composition.Wrap.prototype.then)
- description and source-code
```javascript
then = function (resolve, reject) {
  return this._getPromise().then(resolve, reject);
}
```
- example usage
```shell
...
  return await Promise.resolve(true);
});

// compose it into a function
var fn = compose(stack);

// this function returns a promise
fn.call(this).then(function (val) {
  console.log(val);
}).catch(function (err) {
  console.error(err.stack);
  process.exit(1);
})
'''
...
```

#### <a name="apidoc.element.composition.Wrap.prototype.throw"></a>[function <span class="apidocSignatureSpan">composition.Wrap.prototype.</span>throw (err)](#apidoc.element.composition.Wrap.prototype.throw)
- description and source-code
```javascript
throw = function (err) {
  return this._getGenerator().throw(err);
}
```
- example usage
```shell
...
}

Wrap.prototype.next = function (val) {
 return this._getGenerator().next(val);
}

Wrap.prototype.throw = function (err) {
 return this._getGenerator().throw(err);
}

/**
* Check if 'obj' is a generator.
*
* @param {Mixed} obj
* @return {Boolean}
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
