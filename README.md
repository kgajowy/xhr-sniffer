# xhr-sniffer ([npm](https://www.npmjs.com/package/xhr-sniffer))

[![npm version](https://badge.fury.io/js/xhr-sniffer.svg)](https://badge.fury.io/js/xhr-sniffer)
[![downloads count](https://img.shields.io/npm/dt/xhr-sniffer.svg)](https://www.npmjs.com/~piecioshka)
[![travis](https://img.shields.io/travis/piecioshka/xhr-sniffer.svg?maxAge=2592000)](https://travis-ci.org/piecioshka/xhr-sniffer)

> Sniff HTTP requests making by XHR in browser or http module in Node.js

## Features

* :white_check_mark: Display logs of `XMLHttpRequests` in DevTools Console
* :white_check_mark: Display logs of `http` module in `Node.js`
* :negative_squared_cross_mark: Sniffing `Fetch API`

## Install

```bash
npm install xhr-sniffer
```

## Usage

### Sniff requests in `Node.js`

```javascript
const xhrSniffer = require('xhr-sniffer');

xhrSniffer.install();

// do XHR requests

xhrSniffer.uninstall();
```

### Sniff requests in `browser`

Attach files in `<head>` tag:

```html
<script src="xhr-sniffer/src/common.js"></script>
<script src="xhr-sniffer/src/browser.js"></script>
```

Next, make some XMLHttpRequests requests.

## Unit tests

Use Jasmine to setup unit test:

```bash
npm test
```

## Code coverage

Use Istanbul to get code coverage ratio:

```bash
npm run coverage
```

## License

[The MIT License](http://piecioshka.mit-license.org) @ 2018
