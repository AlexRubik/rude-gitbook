---
description: >-
  You basically need the suggested specifications at minimum, but the minimum
  requirements section is technically the least you can do to run the bot. You
  just won't hit much.
---

# Requirements

[**Discord**](https://discord.gg/6DTGbMNYuA)

## Minimum Requirements

* [Quiknode's free Jupiter ](https://marketplace.quicknode.com/add-on/metis-jupiter-v6-swap-api)[API](https://marketplace.quicknode.com/add-on/metis-jupiter-v6-swap-api) (10 requests per second) or Jupiter's free v6 API (https://quote-api.jup.ag/v6 , heavily rate limited)
* Access to an [RPC node](setup/rpcs.md)
* Linux or Windows Operating System\
  \- Windows users can use [WSL](https://learn.microsoft.com/en-us/windows/wsl/install)
* Funds for transaction fees and your preferred trade sizes (for a minimal testing setup: 4 USDC, 0.05 SOL)

## Suggested Specifications

* [Jupiter v6 API](setup/jupiter-v6-access.md) with no or high rate limit
* [RPC node](setup/rpcs.md) with no or high rate limit
* Linux OS
* Base token balances to cover the trade sizes you want to capture and SOL for transaction fees

## Ideal Specifications

* Run your own RPC node
* On a separate server in the same data center as your RPC node, host your Jup API using your RPC node. Run your bots on these servers if they can spare CPU and RAM usage. If you want a complete separation of concerns, run your bots on a 3rd separate server in the same data center.
* Linux OS
* Base token balances to cover the trade sizes you want to capture and SOL for transaction fees
