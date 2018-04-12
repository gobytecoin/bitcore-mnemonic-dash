BIP39 Mnemonics for Bitcore-GoByte
=======

[![NPM Package](https://img.shields.io/npm/v/bitcore-mnemonic-gobyte.svg?style=flat-square)](https://www.npmjs.org/package/bitcore-mnemonic-gobyte)
[![Build Status](https://img.shields.io/travis/gobytecoin/bitcore-mnemonic-gobyte.svg?branch=master&style=flat-square)](https://travis-ci.org/gobytecoin/bitcore-mnemonic-gobyte)
[![Coverage Status](https://img.shields.io/coveralls/gobytecoin/bitcore-mnemonic-gobyte.svg?style=flat-square)](https://coveralls.io/r/gobytecoin/bitcore-mnemonic-gobyte)

A module for [bitcore-gobyte](https://github.com/gobytecoin/bitcore-gobyte) that implements [Mnemonic code for generating deterministic keys](https://github.com/bitcoin/bips/blob/master/bip-0039.mediawiki).

## Getting Started

This library is distributed in both the npm and bower packaging systems.

```sh
npm install bitcore-mnemonic-gobyte
bower install bitcore-mnemonic-gobyte
```

There are many examples of how to use it on the developer guide [section for mnemonic](http://bitcore.io/guide/module/mnemonic/index.html). For example, the following code would generate a new random mnemonic code and convert it to a `HDPrivateKey`.

```javascript
var Mnemonic = require('bitcore-mnemonic-gobyte');
var code = new Mnemonic(Mnemonic.Words.SPANISH);
code.toString(); // natal hada sutil año sólido papel jamón combate aula flota ver esfera...
var xpriv = code.toHDPrivateKey();
```

## Contributing

See [CONTRIBUTING.md](https://github.com/gobytecoin/bitcore-gobyte/blob/master/CONTRIBUTING.md) on the main bitcore-gobyte repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/bitpay/bitcore/blob/master/LICENSE).

Copyright 2013-2015 BitPay, Inc. Bitcore is a trademark maintained by BitPay, Inc.
