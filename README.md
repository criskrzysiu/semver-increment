SemVer-Increment
====
[![Build Status](https://travis-ci.org/weflex/semver-increment.svg?branch=master)](https://travis-ci.org/weflex/semver-increment)
[![Coverage Status](https://coveralls.io/repos/github/weflex/semver-increment/badge.svg?branch=master&bust=1)](https://coveralls.io/github/weflex/semver-increment?branch=master)

Handly library to bump Semantic Version numbers.

```js
var bumpVersion = require('semver-increment');
var MAJOR = 0;                                 // don't bump MAJOR
var MINOR = 1;                                 // bump MINOR
var PATCH = 0;                                 // don't bump PATCH
var masks = [MAJOR, MINOR, PATCH];
var nextVersion = bumpVersion(masks, '1.2.3'); // -> 1.3.0
```

Features
----

- [x] Bump SemVer number according to MASKS (for bits are non-zero)
- [x] Bump PATCH number if no MASKS are provided, or MASKS is `[0, 0, 0]`
- [x] Bump the biggest number (e.g. If MAJOR and MINOR are both non-zero, bump MAJOR)

Run Tests
----

```
$ npm test
```

Installation
----

```
$ npm install semver-increment --save
```

LICENSE
----

To be discussed.
