# @stackline/path-browserify

> the path module from node core for browsers.

[![npm version](https://img.shields.io/npm/v/@stackline/path-browserify.svg?style=flat-square)](https://www.npmjs.com/package/@stackline/path-browserify)
[![license](https://img.shields.io/npm/l/@stackline/path-browserify.svg?style=flat-square)](https://github.com/alexandroit/stackline-path-browserify)
[![GitHub repository](https://img.shields.io/badge/GitHub-repository-181717?style=flat-square&logo=github)](https://github.com/alexandroit/stackline-path-browserify)
[![Docs](https://img.shields.io/badge/docs-alexandro.net-0f766e?style=flat-square)](https://alexandro.net/docs/vanilla/path-browserify/)
[![Reddit community](https://img.shields.io/badge/community-r%2FStackline-ff4500?style=flat-square&logo=reddit&logoColor=white)](https://www.reddit.com/r/Stackline/)

**[Documentation](https://alexandro.net/docs/vanilla/path-browserify/)** | **[npm](https://www.npmjs.com/package/@stackline/path-browserify)** | **[Issues](https://github.com/alexandroit/stackline-path-browserify/issues)** | **[Repository](https://github.com/alexandroit/stackline-path-browserify)**

**Current package version:** `1.0.2`

---

## Why this package?

`@stackline/path-browserify` is the Stackline-maintained distribution of `path-browserify@1.0.1`. It is an independent continuation of [path-browserify](https://github.com/browserify/path-browserify); original authors and licenses remain credited below.

## Compatibility

| Item | Value |
| :--- | :--- |
| Package | `@stackline/path-browserify@1.0.2` |
| API target | `path-browserify@1.0.1` |
| Supported Node.js | `See supported framework requirements` |
| License | `MIT` |
| Main entry | `index.js` |
| Runtime dependencies | `none` |

## Installation

```bash
npm install @stackline/path-browserify
```

Preserve existing imports and plugin resolution with an npm alias:

```bash
npm install path-browserify@npm:@stackline/path-browserify
```

## Usage and API reference

### path-browserify [![Build Status](https://travis-ci.org/browserify/path-browserify.png?branch=master)](https://travis-ci.org/browserify/path-browserify)

> The `path` module from Node.js for browsers

This implements the Node.js [`path`][path] module for environments that do not have it, like browsers.

> `path-browserify` currently matches the **Node.js 10.3** API.

## Install

You usually do not have to install `path-browserify` yourself! If your code runs in Node.js, `path` is built in. If your code runs in the browser, bundlers like [browserify](https://github.com/browserify/browserify) or [webpack](https://github.com/webpack/webpack) include the `path-browserify` module by default.

But if none of those apply, with npm do:

```
npm install @stackline/path-browserify
```

## Usage

```javascript
var path = require('path')

var filename = 'logo.png';
var logo = path.join('./assets/img', filename);
document.querySelector('#logo').src = logo;
```

## API

See the [Node.js path docs][path]. `path-browserify` currently matches the Node.js 10.3 API.
`path-browserify` only implements the POSIX functions, not the win32 ones.

## Contributing

PRs are very welcome! The main way to contribute to `path-browserify` is by porting features, bugfixes and tests from Node.js. Ideally, code contributions to this module are copy-pasted from Node.js and transpiled to ES5, rather than reimplemented from scratch. Matching the Node.js code as closely as possible makes maintenance simpler when new changes land in Node.js.
This module intends to provide exactly the same API as Node.js, so features that are not available in the core `path` module will not be accepted. Feature requests should instead be directed at [nodejs/node](https://github.com/nodejs/node) and will be added to this module once they are implemented in Node.js.

If there is a difference in behaviour between Node.js's `path` module and this module, please open an issue!

## License

[MIT](./LICENSE)

[path]: https://nodejs.org/docs/v10.3.0/api/path.html

## Credits and original authors

- Original project: [path-browserify](https://github.com/browserify/path-browserify).
- James Halliday.
- Copyright (c) 2013 James Halliday.
- Stackline maintenance: [Alexandro Paixao Marques](https://www.linkedin.com/in/aleinfo/) and [Stackline contributors](https://github.com/alexandroit).

Original copyright, license notices and contributor acknowledgements remain part of this distribution. Stackline maintenance does not replace authorship of the original work.

## Community and Links

- [Stackline website](https://alexandro.net/)
- [GitHub projects](https://github.com/alexandroit)
- [npm packages](https://www.npmjs.com/~alex360qc)
- [Reddit community — r/Stackline](https://www.reddit.com/r/Stackline/)
- [Maintainer LinkedIn](https://www.linkedin.com/in/aleinfo/)

Use this repository's issue tracker for reproducible bugs and feature requests. Join r/Stackline for examples, usage questions and release discussions.
