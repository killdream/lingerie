# Lingerie

[![Build Status](https://secure.travis-ci.org/robotlolita/lingerie.png?branch=master)](https://travis-ci.org/robotlolita/lingerie)
[![NPM version](https://badge.fury.io/js/lingerie.png)](http://badge.fury.io/js/lingerie)
[![Dependencies Status](https://david-dm.org/robotlolita/lingerie.png)](https://david-dm.org/robotlolita/lingerie)
[![experimental](http://hughsk.github.io/stability-badges/dist/experimental.svg)](http://github.com/hughsk/stability-badges)


Sexy and fashionable string manipulation in JavaScript.

This modules provides basic services for manipulating and interacting with
strings in JavaScript:

  - Building strings (cycling/concatenating).
  - Trimming whitespace.
  - Common predicates (starts with?, ends with?, empty?)
  - Declarative slicing (first, rest, ...)

Oh, everything is curried for great goodness!


### Platform support

This library assumes an ES5 environment, but can be easily supported in ES3
platforms by the use of shims. Just include [es5-shim][] :3

[![browser support](http://ci.testling.com/robotlolita/lingerie.png)](http://ci.testling.com/robotlolita/lingerie)


### Example

```js
var l = require('lingerie')

l.isEmpty('foo')
// => (Boolean) false

// Most functions are curried though, so take advantage of it:
var fooStuff = l.startsWith('foo')
fooStuff('fooBar')
// => (Boolean) true
```


### Installing

Just grab it from NPM:

    $ npm install lingerie


### Documentation

A quick reference of the API can be built using [Calliope][]:

    $ npm install -g calliope
    $ calliope build


### Tests

You can run all tests using Mocha:

    $ npm test


### Licence

MIT/X11. ie.: do whatever you want.

[Calliope]: https://github.com/robotlolita/calliope
[es5-shim]: https://github.com/kriskowal/es5-shim
