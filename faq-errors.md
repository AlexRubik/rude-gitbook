---
description: If this page is not helpful, please look for support on our Discord.
---

# FAQ / Errors

[**Discord**](https://discord.gg/6DTGbMNYuA)

## FAQ

* **Why am I not rich yet?**\
  You can't just turn the bot on and make infinite money. You need to have good connections to [RPC(s)](bot-setup-instructions/rpcs.md) and a [Jupiter v6 API](bot-setup-instructions/jupiter-v6-access.md) and try different [strategies](strategies.md) to see what works.\

* **There is no slippage variable? Can I lose?**\
  **You can't lose on a successful transaction!** (except for transaction fees and fees for opening token accounts)\
  I've written an on chain program that prevents loss. The transaction is designed to fail if your base token balance ends less than or equal to the starting balance.  \

* **Transaction fees are killing me. How do I mitigate?**\
  \- Increase minProfitBps\
  \- Lower your priority fee\
  \- Increase your [simulation value](#user-content-fn-1)[^1]

## Errors

* `429 Errors:` you are being rate limited by your [Jupiter API](bot-setup-instructions/jupiter-v6-access.md) or [RPC](bot-setup-instructions/rpcs.md)
* `RangeError: encoding overruns Uint8Array:` transaction size was too large
* `400 Errors from Jupiter`: the ones that I'm seeing are from no routes found for some pairs I'm testing. Will need to handle this in future releases.



[^1]: `PROFIT_BPS_THRESHOLD_FOR_SIM`
