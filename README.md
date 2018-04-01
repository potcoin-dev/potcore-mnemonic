<img src="http://potcore.io/css/images/module-mnemonic.png" alt="potcore mnemonics" height="35">
BIP39 Mnemonics for potcore
=======

[![NPM Package](https://img.shields.io/npm/v/potcore-mnemonic.svg?style=flat-square)](https://www.npmjs.org/package/potcore-mnemonic)
[![Build Status](https://img.shields.io/travis/potcoin-dev/potcore-mnemonic.svg?branch=master&style=flat-square)](https://travis-ci.org/potcoin-dev/potcore-mnemonic)
[![Coverage Status](https://img.shields.io/coveralls/potcoin-dev/potcore-mnemonic.svg?style=flat-square)](https://coveralls.io/r/potcoin-dev/potcore-mnemonic)

A module for [potcore](https://github.com/potcoin-dev/potcore) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install potcore-mnemonic
bower install potcore-mnemonic
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://potcore.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('potcore-mnemonic');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/potcoin-dev/potcore/blob/master/CONTRIBUTING.md) on the main potcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/potcoin-dev/potcore/blob/master/LICENSE).

Copyright 2013-2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
