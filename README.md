# @devtea2028/laborum-dignissimos-molestiae-deleniti <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][deps-svg]][deps-url]
[![dev dependency status][dev-deps-svg]][dev-deps-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

ES spec-compliant shim for `Date`. Invoke its "shim" method to shim `Date` if it is unavailable or noncompliant.

This package implements the [es-shim API](https://github.com/es-shims/api) “multi” interface. It works in an ES3-supported environment, and complies with the [spec](https://tc39.es/proposal-promise-any/#sec-@devtea2028/laborum-dignissimos-molestiae-deleniti).

Most common usage:
```js
var assert = require('assert');

var shims = require('@devtea2028/laborum-dignissimos-molestiae-deleniti');

assert.deepEqual(shims, [
	'Date',
	'Date.prototype.getFullYear',
	'Date.prototype.getMonth',
	'Date.prototype.getDate',
	'Date.prototype.getUTCDate',
	'Date.prototype.getUTCFullYear',
	'Date.prototype.getUTCMonth',
	'Date.prototype.toUTCString',
	'Date.prototype.toDateString',
	'Date.prototype.toString',
	'Date.prototype.toISOString',
	'Date.prototype.toJSON',
	'Date.now',
	'Date.parse',
]);

require('@devtea2028/laborum-dignissimos-molestiae-deleniti/auto'); // will be a no-op if not needed

assert.ok(new Date() instanceof Date);
assert.equal(typeof Date.now(), 'number');

// etc, with all the Date methods you expect
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.com/package/@devtea2028/laborum-dignissimos-molestiae-deleniti
[npm-version-svg]: https://versionbadg.es/devtea2028/laborum-dignissimos-molestiae-deleniti.svg
[deps-svg]: https://david-dm.org/devtea2028/laborum-dignissimos-molestiae-deleniti.svg
[deps-url]: https://david-dm.org/devtea2028/laborum-dignissimos-molestiae-deleniti
[dev-deps-svg]: https://david-dm.org/devtea2028/laborum-dignissimos-molestiae-deleniti/dev-status.svg
[dev-deps-url]: https://david-dm.org/devtea2028/laborum-dignissimos-molestiae-deleniti#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@devtea2028/laborum-dignissimos-molestiae-deleniti.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@devtea2028/laborum-dignissimos-molestiae-deleniti.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@devtea2028/laborum-dignissimos-molestiae-deleniti.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@devtea2028/laborum-dignissimos-molestiae-deleniti
[codecov-image]: https://codecov.io/gh/devtea2028/laborum-dignissimos-molestiae-deleniti/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/devtea2028/laborum-dignissimos-molestiae-deleniti/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/devtea2028/laborum-dignissimos-molestiae-deleniti
[actions-url]: https://github.com/devtea2028/laborum-dignissimos-molestiae-deleniti/actions
