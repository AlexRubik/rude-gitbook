---
description: >-
  Some basic strategies to try or gain inspiration from. We also post strategies
  in the Discord.
---

# Strategies

## Small Trade Sizes

Everyone should try small trade sizes first because they're the easiest to hit so it's a good baseline test for your connections. If you can't hit anything with small trade sizes and small minProfitBps values then something is wrong with your connections. You need a higher quality Jup API or RPC or both.\
\
For example:

```json
    {
      "mint": "EPjFWdd5AufqSSqeM2qN1xzybapC8G4wEGGkZwyTDt1v",
      "name": "USDC",
      "decimals": 6,
        "enabled": true,
        "minTradeSize": 1,
        "maxTradeSize": 4,
        "balance": 4,
        "tradeSizeDecimals": 1,
        "minProfitBps": 30,
        "directRoutesOnly": false,
        "maxAccounts": 28,
        "profitBpsThresholdForSim": 35,
        "minFeeLamports": 1000,
        "maxFeeLamports": 3000
    },
```

## Stalker

Look at successful transactions associated with the bots program id to see what works for others. It might work for you too. Here are links to the bot program: [Solscan](https://solscan.io/account/3tZPEagumHvtgBhivFJCmhV9AyhBHGW9VgdsK52i4gwP) [SolanaFM](https://solana.fm/address/3tZPEagumHvtgBhivFJCmhV9AyhBHGW9VgdsK52i4gwP?cluster=mainnet-alpha)
