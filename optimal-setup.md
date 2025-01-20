---
description: Suggestions for an optimal setup.
---

# Optimal Setup

* Connections with no rate limit: [RPC/GRPC](bot-setup-instructions/rpc-+-grpc.md)
* Large trade sizes; your profit will scale with trade size because you will be exposed to opportunities that aren't present at lower trade sizes. E.g., a trade size range of $500 - $10,000 will almost always be more profitable than a range of $10 - $50.
* Distribute min/max trade size ranges into different base config objects. E.g., $1 - $20 in one object, $20 - $80 in another, etc.
* Try different minProfitBps values. Start low at 1 and increase
* Frequently put new and popular token mint addresses in your includeMints.json and in your filter mints Jup API arg if you are self hosting. Look into automating this with thes APIs:\
  [https://docs.birdeye.so/reference/get\_defi-token-trending](https://docs.birdeye.so/reference/get_defi-token-trending)\
  [https://www.geckoterminal.com/dex-api](https://www.geckoterminal.com/dex-api)\
  [https://solana.com/docs/rpc/http/getsignaturesforaddress](https://solana.com/docs/rpc/http/getsignaturesforaddress)
* Ubuntu 22 OS
* [Host your own Jupiter API](bot-setup-instructions/jupiter-v6-access.md) on a [server](https://billing.nodestop.io/aff.php?aff=88) with at least 12 cores and **24 + cores is optimal** (Ask in Discord if you need help with this).
* Your Jup API will be faster in theory if it uses a Yellowstone gRPC.
* Put many different RPC urls in the rpcs.json file. You can also try duplicating some of them.
* QUOTE\_REQUEST\_INTERVAL\_MS=(As low as possible without killing your jup api, try 10 - 80)\
  SPAM\_RPCS\_ENABLED=true\
  Read the [.env ](bot-setup-instructions/.env.md)page to learn what these are doing and how to use them
* To scale further, you can put this setup in all the validator cluster locations mentioned in the first bullet point above.
