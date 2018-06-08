# zoop - Unofficial Client for Zoop API

<p align="center">
🇧🇷 <a href="LEIAME.md">LEIAME em Português</a>
<br><br>
<a href="https://www.npmjs.com/package/@coreh/zoop"><img src="https://img.shields.io/npm/v/@coreh/zoop.svg"></a>
<a href="LICENSE"><img src="https://img.shields.io/npm/l/@coreh/zoop.svg"></a>
<a href="https://travis-ci.org/coreh/zop/"><img src="https://img.shields.io/travis/coreh/zoop.svg"></a>
<a href="https://coveralls.io/github/coreh/zoop"><img src="https://img.shields.io/coveralls/github/coreh/zoop.svg"></a>
<a href="https://david-dm.org/coreh/zoop"><img src="https://img.shields.io/david/coreh/zoop.svg"></a>
</p>


## About

- Isomorphic (Browser, Node, ReactNative)
- TypeScript type definitions

## Installing

```bash
npm install @coreh/zoop
```

## Usage

```javascript
import Zoop from '@coreh/zoop';

// Create API Client
const zoop = new Zoop(API_KEY);

// Marketplace Endpoint
const marketplace = zoop.marketplace(MARKETPLACE_ID);

// Buyer Endpoint
const buyer = marketplace.buyer(BUYER_ID);

// Retrieve Buyer Info (async)
const buyerInfo = await buyer.get();

// List Buyers (async iterator)
for await (const buyerInfo of marketplace.listBuyers()) {
    // ...
}
```

## Implemented Endpoints

- Marketplace (Retrieve)
- Buyer (Create, Retrieve, List)
- Transaction (Create, Retrieve, List)
- Seller (Create, Retrieve, List)

## License

MIT
