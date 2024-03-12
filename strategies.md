---
description: Some basic strategies to try or gain inspiration from.
---

# Strategies

## Small Trade Sizes

Everyone should try small trade sizes first because they're the easiest to hit so it's a good baseline test for your connections. If you can't hit anything with small trade sizes and small profitBps values then something is wrong with your connections. You need a higher quality Jup API or RPC or both.\
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
        "minProfitBps": 50,
        "directRoutesOnly": false
    },
```

##
