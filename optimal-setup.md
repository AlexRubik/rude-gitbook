---
description: Suggestions for an optimal setup.
---

# Optimal Setup

* All these servers need to be in the same location AND near a cluster of validators:\
  \- [RPC server](bot-setup-instructions/rpc-+-grpc.md)\
  \- [Jupiter API server](bot-setup-instructions/jupiter-v6-access.md) (Self Hosting is suggested and basically required now)\
  \
  Here are some locations that have a high concentration of validators: Frankfurt, Amsterdam, New York, Chicago, Virginia. Check out this map of Solana validators: [https://www.validators.app/](https://www.validators.app/)
* Connections with little or no rate limit: [Premium RPC](bot-setup-instructions/rpc-+-grpc.md), [Self Hosted Jupiter API](bot-setup-instructions/jupiter-v6-access.md)
* Large trade sizes; your profit will scale with trade size because you will be exposed to opportunities that aren't present at lower trade sizes. E.g., a trade size range of $10 - $500 will almost always be more profitable than a range of $10 - $50 if you have high quality RPC/Jup connections.
* Distribute min/max trade size ranges into different base config objects. E.g., $1 - $20 in one object, $20 - $80 in another, etc.
* Try different minProfitBps values. Start low at 1 and increase
* Frequently put new and popular token mint addresses in your includeMints.json and in your filter mints Jup API arg if you are self hosting. Look into automating this with thes APIs:\
  [https://docs.birdeye.so/reference/get\_defi-token-trending](https://docs.birdeye.so/reference/get\_defi-token-trending)\
  [https://www.geckoterminal.com/dex-api](https://www.geckoterminal.com/dex-api)\
  [https://solana.com/docs/rpc/http/getsignaturesforaddress](https://solana.com/docs/rpc/http/getsignaturesforaddress)
* Ubuntu 22 OS
* [Host your own Jupiter API](bot-setup-instructions/jupiter-v6-access.md) on a [dedicated (bare metal) server](https://billing.nodestop.io/aff.php?aff=88) with at least 8 cores and **24 + cores is optimal** (Ask in Discord if you need help with this).
* Your Jup API will be faster in theory if it uses a Yellowstone gRPC.
* Put many different RPC urls in the rpcs.json file. You can also try duplicating some of them.
* QUOTE\_REQUEST\_INTERVAL\_MS=(As low as possible without killing your jup api, try 10 - 50)\
  SPAM\_RPCS\_ENABLED=true\
  Read the [.env ](bot-setup-instructions/.env.md)page to learn what these are doing and how to use them
* To scale further, you can put this setup in all the validator cluster locations mentioned in the first bullet point above.
