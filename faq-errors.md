# FAQ / Errors

## FAQ

* **Why am I not rich yet?**\
  You can't just turn the bot on and make infinite money. You need to have dedicated connections to RPC(s) and a [Jupiter v6 API](setup/jupiter-v6-access.md) and try different [strategies](strategies.md) to see what works.\

* **There is no slippage variable? Can I lose?**\
  **You can't lose on a successful transaction!** (except for transaction fees and fees for opening token accounts)\
  I've written an on chain program that prevents loss. The transaction is designed to fail if your base token balance ends less than or equal to the starting balance.  \

* **Transaction fees are killing me. How do I mitigate?**\
  \- Increase your [simulation value](#user-content-fn-1)[^1]\
  \- Increase min profit\
  \- Lower your priority fee

## Errors

* `429 Errors:` you are being rate limited by your [Jupiter API](setup/jupiter-v6-access.md) or [RPC](setup/rpcs.md)
* `RangeError: encoding overruns Uint8Array:` transaction size was too large
* `400 Errors from Jupiter`: the ones that I'm seeing are from no routes found for some pairs I'm testing. Will need to handle this in future releases.



[^1]: `PROFIT_BPS_THRESHOLD_FOR_SIM`
