---
description: Suggestions for an optimal setup.
---

# Optimal Setup

* All servers in the same location\
  \- [RPC server](bot-setup-instructions/rpcs.md)\
  \- [Jupiter API server](bot-setup-instructions/jupiter-v6-access.md) (QuickNode's server is in Ashburn, VA)\
  \- Server that runs the bot (look in rent-servers channel in [Discord](./) for cheapest options the community finds)
* RPC optimized for sending transactions
* Large trade sizes; your profit will scale with trade size because you will be exposed to opportunities that aren't present at lower trade sizes. E.g., a trade size range of $10 - $1000 will almost always be more profitable than a range of $10 - $50.
* Distribute trade size ranges into different base config objects. E.g., $50 - $100 in one object, $100 - $150 in another, etc.
* Base config objects with minProfitBps values that decrease as the trade size increases. E.g., a trade size range of $100 - $300 should have a minProfitBps of 5 - 15 but a range of $1 - $10 should have a minProfitBps > 30. These are suggestions. You should test these values yourself.
