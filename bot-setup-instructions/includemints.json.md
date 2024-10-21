# includeMints.json

Whenever the bot looks for an arb opportunity it gets price quotes like this: \
TokenA1 -> TokenB \
TokenB -> TokenA2 \
\
If TokenA1 < TokenA2 then it is potentially profitable. \
\
**includeMints.json** has all the **TokenBs**. \
Each object/mint in the baseConfig.json has all the **TokenAs**.

