# [redux-storage-decorator-filter][]

[![build](https://travis-ci.org/react-stack/redux-storage-decorator-filter.svg?branch=master)](https://travis-ci.org/react-stack/redux-storage-decorator-filter)
[![dependencies](https://david-dm.org/react-stack/redux-storage-decorator-filter.svg)](https://david-dm.org/react-stack/redux-storage-decorator-filter)
[![devDependencies](https://david-dm.org/react-stack/redux-storage-decorator-filter/dev-status.svg)](https://david-dm.org/react-stack/redux-storage-decorator-filter#info=devDependencies)

[![license](https://img.shields.io/npm/l/redux-storage-decorator-filter.svg?style=flat-square)](https://www.npmjs.com/package/redux-storage-decorator-filter)
[![npm version](https://img.shields.io/npm/v/redux-storage-decorator-filter.svg?style=flat-square)](https://www.npmjs.com/package/redux-storage-decorator-filter)
[![npm downloads](https://img.shields.io/npm/dm/redux-storage-decorator-filter.svg?style=flat-square)](https://www.npmjs.com/package/redux-storage-decorator-filter)

Filter decorator for [redux-storage][] to only store a subset of the whole
state tree.

## Installation

    npm install --save redux-storage-decorator-filter

## Usage

Simply wrap your engine in this decorator, whitelist all keys that should
be passed through and blacklist the keys that shouldn't.

```js
import filter from 'redux-storage-decorator-filter'

engine = filter(engine, [
    'whitelisted-key',
    ['nested', 'key'],
    ['another', 'very', 'nested', 'key']
], [
    'blacklisted-key',
    ['nested', 'blacklisted-key']
]);
```

# A fork of [redux-storage-decorator-filter](https://github.com/michaelcontento/redux-storage-decorator-filter)

The original author of the package [redux-storage-decorator-filter](https://github.com/michaelcontento/redux-storage-decorator-filter) has decided to deprecate the project and no longer maintained. The package will now be maintained here.

Thank you [michaelcontento](https://github.com/michaelcontento) for a great library!

## License

    The MIT License (MIT)

    Copyright (c) 2016- Gunjan Soni <gunjan.soni2002@gmail.com> 
    Copyright (c) 2015-2016 Michael Contento <mail@michaelcontento.de> 

    Permission is hereby granted, free of charge, to any person obtaining a copy of
    this software and associated documentation files (the "Software"), to deal in
    the Software without restriction, including without limitation the rights to
    use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
    the Software, and to permit persons to whom the Software is furnished to do so,
    subject to the following conditions:

    The above copyright notice and this permission notice shall be included in all
    copies or substantial portions of the Software.

    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
    FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
    COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
    IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
    CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.

  [redux-storage]: https://github.com/react-stack/redux-storage
  [redux-storage-decorator-filter]: https://github.com/react-stack/redux-storage-decorator-filter
