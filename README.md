# @erboladaiteas/dolore-odio <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

`Object.defineProperty`, but not IE 8's broken one.

## Example

```js
const assert = require('assert');

const $defineProperty = require('@erboladaiteas/dolore-odio');

if ($defineProperty) {
    assert.equal($defineProperty, Object.defineProperty);
} else if (Object.defineProperty) {
    assert.equal($defineProperty, false, 'this is IE 8');
} else {
    assert.equal($defineProperty, false, 'this is an ES3 engine');
}
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

## Security

Please email [@ljharb](https://github.com/ljharb) or see https://tidelift.com/security if you have a potential security vulnerability to report.

[package-url]: https://npmjs.org/package/@erboladaiteas/dolore-odio
[npm-version-svg]: https://versionbadg.es/ljharb/@erboladaiteas/dolore-odio.svg
[deps-svg]: https://david-dm.org/ljharb/@erboladaiteas/dolore-odio.svg
[deps-url]: https://david-dm.org/ljharb/@erboladaiteas/dolore-odio
[dev-deps-svg]: https://david-dm.org/ljharb/@erboladaiteas/dolore-odio/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@erboladaiteas/dolore-odio#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@erboladaiteas/dolore-odio.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@erboladaiteas/dolore-odio.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@erboladaiteas/dolore-odio.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@erboladaiteas/dolore-odio
[codecov-image]: https://codecov.io/gh/ljharb/@erboladaiteas/dolore-odio/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@erboladaiteas/dolore-odio/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@erboladaiteas/dolore-odio
[actions-url]: https://github.com/erboladaiteas/dolore-odio/actions
