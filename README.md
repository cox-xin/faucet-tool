# Handshake Faucet Tool
This tool generates the first receiving address, in the first account of a
BIP44 HD wallet. It also generates the 24 word BIP39 mnemonic phrase which was
used to seed the wallet. **It is important that you keep this seed phrase
private. It is the only way to access your HNS coins. Do not share your
mnemonic seed phrase with anyone that should not have access to the contents
of the wallet.**

>Note: **running this software on compromised hardware will leave you in
danger of losing funds.**

## Requirements
* Linux, OSX or Windows
* git
* node.js >=v8.0.0
* npm >=v4.0.0

### Additional requirements to build binaries
* [ pkg ](https://github.com/zeit/pkg)
* tar

## Browser tool
```
$ git clone git@github.com:handshake-org/faucet-tool.git
$ cd faucet-tool
$ npm install
$ npm run webpack
$ open browser/index.html
```

## CLI tool
```
$ git clone git@github.com:handshake-org/faucet-tool.git
$ cd faucet-tool
$ npm install
$ ./bin/faucet-tool createaddress
```

## Notes

This tool uses faucet-tool.js for generating mnemonic seed phrases.

Forked from https://github.com/handshake-org/hskd

HD keys and mnemonics (BIP32, BIP39).

Parts of this software were originally based on bitcore-lib:

- https://github.com/bitpay/bitcore-lib/blob/master/lib/hdprivatekey.js
- https://github.com/bitpay/bitcore-lib/blob/master/lib/hdpublickey.js
- https://github.com/ryanxcharles/fullnode/blob/master/lib/bip32.js
- https://github.com/bitpay/bitcore-mnemonic/blob/master/lib/mnemonic.js

BIP32

```
Copyright (c) 2015-2016, Christopher Jeffrey (MIT License).
https://github.com/bcoin-org/bcoin

Copyright (c) 2013-2015 BitPay, Inc.

Parts of this software are based on Bitcoin Core
Copyright (c) 2009-2015 The Bitcoin Core developers

Parts of this software are based on fullnode
Copyright (c) 2014 Ryan X. Charles
Copyright (c) 2014 reddit, Inc.

Parts of this software are based on BitcoinJS
Copyright (c) 2011 Stefan Thomas <justmoon@members.fsf.org>

Parts of this software are based on BitcoinJ
Copyright (c) 2011 Google Inc.

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
```

BIP39

```
The MIT License (MIT)

Copyright (c) 2014 BitPay

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```
