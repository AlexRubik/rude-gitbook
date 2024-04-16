---
description: If this page is not helpful, please look for support on our Discord.
---

# FAQ / Errors

[**Discord**](https://discord.gg/6DTGbMNYuA)

## FAQ

* **Why am I not rich yet?**\
  **Read** [**Optimal Setup**](optimal-setup.md)\
  You can't just turn the bot on and make infinite money. You need to have good connections to [RPC(s)](bot-setup-instructions/rpcs.md) and a [Jupiter v6 API](bot-setup-instructions/jupiter-v6-access.md) and try different [strategies](strategies.md) to see what works.\

* **Can I lose money on a transaction?**\
  **You can't lose on a successful transaction!** (except for transaction fees and fees for opening token accounts)\
  We've written an on chain program (smart contract) that prevents loss. The transaction is designed to fail if your base token balance ends less than or equal to the starting balance. Don't believe us? The bot has produced **over 3 million transactions** that you can analyze [here](https://solscan.io/account/3tZPEagumHvtgBhivFJCmhV9AyhBHGW9VgdsK52i4gwP)!\

* **Transaction fees are killing me. How do I mitigate?**\
  \- Increase minProfitBps\
  \- Lower your priority fee\
  \- Increase your [simulation value](#user-content-fn-1)[^1]

## Errors

* `429 Errors:` you are being rate limited by your [Jupiter API](bot-setup-instructions/jupiter-v6-access.md) or [RPC](bot-setup-instructions/rpcs.md)
* `RangeError: encoding overruns Uint8Array:` transaction size was too large
* `400 Errors from Jupiter`: the ones that we're seeing are from no routes found for some pairs. Will need to handle this in future releases.



[^1]: `PROFIT_BPS_THRESHOLD_FOR_SIM`
