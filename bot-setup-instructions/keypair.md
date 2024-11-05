---
description: >-
  Use this JavaScript code to convert your string/base58 private key to a json
  array. Paste this into Claude or ChatGPT and ask how to execute the code.
---

# Keypair

```javascript
const fs = require('fs');
const { Keypair } = require('@solana/web3.js');
const bs58 = require('bs58');

const base58PrivateKey = 'private key as string here...';
const uint8ArrayPrivateKey = bs58.decode(base58PrivateKey);

// Create a Keypair from the Uint8Array
const keypair = Keypair.fromSecretKey(uint8ArrayPrivateKey);

// Write the keypair to a JSON file in same directory
const keypairPath = './keypair.json';
fs.writeFileSync(keypairPath, `[${Array.from(keypair.secretKey)}]`);

```
