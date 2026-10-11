
<div align="center">

# Arweave Indexer

### Index, discover, and query structured data across Arweave and AO.

A lightweight TypeScript utility for building decentralized applications.

[![npm version](https://img.shields.io/npm/v/arweave-indexer?style=flat-square&color=blue)](https://www.npmjs.com/package/arweave-indexer)
[![npm downloads](https://img.shields.io/npm/dm/arweave-indexer?style=flat-square)](https://www.npmjs.com/package/arweave-indexer)
[![License: MIT](https://img.shields.io/badge/License-MIT-green?style=flat-square)](LICENSE)
[![TypeScript](https://img.shields.io/badge/TypeScript-Ready-3178C6?style=flat-square&logo=typescript&logoColor=white)](https://www.typescriptlang.org/)

[![Hacker House Winner](https://img.shields.io/badge/Arweave%20India%20Hacker%20House-1st%20Place-8A2BE2?style=flat-square)](https://x.com/arweaveindia/status/1867592319870152818)
[![Bounty](https://img.shields.io/badge/Bounty-%243%2C000-f5b942?style=flat-square)](https://x.com/arweaveindia/status/1867592319870152818)

[Website](https://arindexer.vercel.app) · [npm](https://www.npmjs.com/package/arweave-indexer) · [Announcement](https://x.com/arweaveindia/status/1867592319870152818)

</div>

---

## 🏆 Built at Arweave India Hacker House

**1st place · $3,000 bounty · 5 days of building**

Arweave Indexer was built at Arweave India Hacker House #3 in Bangalore.

We picked one of the hardest problems on the board, pivoted twice, and shipped with two hours left before the demo.

Before presenting, we cold-called a founder in the Arweave ecosystem and onboarded them as our first user.

[Read the official winner announcement →](https://x.com/arweaveindia/status/1867592319870152818)

---

## ✨ Features

- **Index structured data** — Publish data for decentralized applications.
- **Query indexed data** — Retrieve results using simple search queries.
- **Filter results** — Narrow queries by AO process and tags.
- **TypeScript support** — Work with a typed developer interface.
- **Arweave + AO** — Build within the Arweave ecosystem.

## 📦 Installation

```bash
npm install arweave-indexer
```

## 🚀 Quick start

### Query data

```ts
import { query } from "arweave-indexer";

const results = await query("web3");
console.log(results);
```

### Index data

```ts
import { index } from "arweave-indexer";

const result = await index(
  JSON.stringify({
    title: "My Web3 Project",
    description: "A decentralized application"
  }),
  window.arweaveWallet
);

console.log(result);
```

### Advanced queries

```ts
const results = await query("web3", {
  process: "custom-process-id",
  tags: [{ name: "Category", value: "Blockchain" }]
});
```

---

## 🌐 Ecosystem

- [Hagrid](https://hagrid_arlink.arweave.net)
- [AR Indexer](https://ar-indexer_arlink.arweave.net)
- [ARLINK](https://arlink.network/)

## 📄 License

MIT
