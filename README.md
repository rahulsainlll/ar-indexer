# @arindexer — Arweave Indexer

## Overview

Arweave Indexer (`arindexer`) is a lightweight indexing and query utility for the Arweave network. It enables developers to efficiently index, discover, and retrieve structured data for decentralized applications built on Arweave and the AO ecosystem.

## Features

* Fast querying of indexed data
* Simple API for indexing structured content
* Native support for Arweave and AO ecosystem
* Fully typed TypeScript interface
* Integration-ready for ARLINK deployments

## Installation

```bash
npm install arweave-indexer
```

## Usage

### Query Data

```ts
import { query } from "arweave-indexer";

async function search() {
  const results = await query("web3");
  console.log(results);
}
```

### Index Data

```ts
import { index } from "arweave-indexer";

async function indexProject() {
  const result = await index(
    JSON.stringify({
      title: "My Web3 Project",
      description: "A decentralized application"
    }),
    window.arweaveWallet
  );

  console.log(result);
}
```

### Advanced Querying

```ts
const results = await query("web3", {
  process: "custom-process-id",
  tags: [
    { name: "Category", value: "Blockchain" }
  ]
});
```

## API Reference

### query(searchTerm: string, options?: IndexerOptions)

Queries indexed data on the AO network.

Returns an array of results or `null`.

### index(data: string, wallet: any, options?: IndexerOptions)

Indexes structured data into the AO network.

Returns the message result or `null`.

## Types

```ts
interface Project {
  title: string;
  link: string;
  description: string;
  twitter?: string;
}

interface IndexerOptions {
  process?: string;
  tags?: { name: string; value: string }[];
}
```

## Ecosystem

* Hagrid — Search and browse Arweave ecosystem projects
  [https://hagrid_arlink.arweave.net](https://hagrid_arlink.arweave.net)

* ARLINK — Deployment platform with automatic indexing support

* AR Indexer — Project discovery and indexing layer
  [https://ar-indexer_arlink.arweave.net](https://ar-indexer_arlink.arweave.net)

## Package Information

* Version: 1.1.0
* Weekly Downloads: 100+
* License: MIT
