# Setup

1. [Download zip file](https://github.com/AlexRubik/rude-bot-solana/releases) (you can use the wget command) onto the machine you will run the bot on, unzip the zip file, and keep all files in the same folder.\
   e.g., `wget https://github.com/AlexRubik/rude-bot-solana/releases/download/v0.2.1-alpha/rude-bot-alpha0_2_1.zip`
2. Modify your .env.example file (see [.env page](.env-file-less-than-v0.1.1-alpha.md)) with nano or whatever text editor you use: \
   `nano .env.example`\
   \
   \- Rename it to .env with this command: \
   `mv .env.example .env`
3. Modify your [baseConfig.json](baseconfig.json.md)
4. Run the executable provided:\
   `./rude-bot-alpha0_2_1`&#x20;

&#x20;\
or once you've figured out your preferred .env values, you can run it in the \
background with nohup:\
\
`nohup ./rude-bot-alpha0_1_1 >> bot1.log 2>&1 &`\
`nohup ./rude-bot-alpha0_1_1 >> bot2.log 2>&1 &`\
\
Watch the logs with `tail -f bot1.log`\
\
Run however many instances you think will be optimal. More instances does not always mean a better overall performance. You will have to test to find out what is best for your setup.
