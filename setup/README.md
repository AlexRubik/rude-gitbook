# Setup

1. [Download zip file](https://github.com/AlexRubik/rude-bot-solana/releases) (you can use the wget command) onto the machine you will run the bot on, unzip the zip file, and keep all files in the same folder.\
   e.g.,&#x20;

```
wget https://github.com/AlexRubik/rude-bot-solana/releases/download/v0.2.4-alpha/rude-bot-alpha0_2_4.zip
```

2. Modify your .env.example file (see [.env page](.env-file-greater-than-v0.2.4-alpha.md)) with nano or whatever text editor you use: \
   `nano .env.example`\
   \
   \- Rename it to .env with this command: \
   `mv .env.example .env`
3. Modify your [baseConfig.json](baseconfig.json.md)
4. Give it permission to execute and then run the executable provided:\
   `chmod +x rude-bot-alpha0_2_4`\
   \
   `./rude-bot-alpha0_2_4`&#x20;
5. Run in background with screen command:\
   `screen -S session1`\
   \
   Execute the bot `./rude-bot-alpha0_2_4`\
   \
   Leave the session with CTRL + D and then tap the letter A.\
   \
   Log back in to the session with `screen -r session1`
