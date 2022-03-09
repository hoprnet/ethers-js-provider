Where the repo comes from:
--------------------------

Main repo: https://github.com/ethers-io/ethers.js

Fork with memory leak fixes: https://github.com/robertkiel/ethers.js

Creation of this repo:

- Clone, and build https://github.com/robertkiel/ethers.js
- Copy artifacts of `@ethersproject/provider` to this repo.

Why?
----

Ethers.js consists of a package `ethersjs` as well as several packages `@ethersproject/*`. This repo only contains affected `@ethersproject/providers` package to allow NPM / Yarn to fetch this package.

Ethereum Providers
==================

This sub-module is part of the [ethers project](https://github.com/ethers-io/ethers.js).

It contains common Provider classes, utility functions for dealing with providers
and re-exports many of the classes and types needed to implement a custom Provider.

For more information, see the [documentation](https://docs.ethers.io/v5/api/providers/).


Importing
---------

Most users will prefer to use the [umbrella package](https://www.npmjs.com/package/ethers),
but for those with more specific needs, individual components can be imported.

```javascript
const {

    Provider,
    BaseProvider,

    JsonRpcProvider,
    StaticJsonRpcProvider,
    UrlJsonRpcProvider,

    FallbackProvider,

    AlchemyProvider,
    CloudflareProvider,
    EtherscanProvider,
    InfuraProvider,
    NodesmithProvider,

    IpcProvider,

    Web3Provider,

    WebSocketProvider,

    JsonRpcSigner,

    getDefaultProvider,

    getNetwork,

    Formatter,

    // Types

    TransactionReceipt,
    TransactionRequest,
    TransactionResponse,

    Listener,

    ExternalProvider,

    Block,
    BlockTag,
    EventType,
    Filter,
    Log,

    JsonRpcFetchFunc,

    Network,
    Networkish

} = require("@ethersproject/providers");
```


License
-------

MIT License
