# includeMints.json

Whenever the bot looks for an arb opportunity it gets price quotes like this: \
TokenA1 -> TokenB \
TokenB -> TokenA2 \
\
If TokenA1 < TokenA2 then it is potentially profitable. \
\
**includeMints.json** has all the **TokenBs**. \
Each object/mint in the baseConfig.json has all the **TokenAs**.

### It's important to put trending and high volume mints in this json file. You can use DEX analytics websites like [Birdeye](https://birdeye.so/?chain=solana) to find trending tokens to put in includeMints.json.
