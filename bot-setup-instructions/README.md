# Bot Setup Instructions

1. [Download zip file](https://github.com/AlexRubik/rude-bot-solana/releases) (on Linux, use the wget command) onto the machine you will run the bot on, unzip the zip file, and keep all files in the same folder.\
   e.g.,&#x20;

```
wget https://github.com/AlexRubik/rude-bot-solana/releases/download/v1.0.0-alpha/rude-bot-alpha1_0_0.zip
```

```
unzip rude-bot-alpha1_0_0.zip
```

```
cd rude-bot-alpha1_0_0
```

2. Modify your .env.example file (see [.env page](.env.md)) with nano or whatever text editor you use: \
   `nano .env.example`\
   \
   \- Rename it to .env with this command: \
   `mv .env.example .env`
3. Modify your [baseConfig.json](baseconfig.json.md)
4. Give it permission to execute and then run the executable provided:\
   `chmod +x rude-bot-alpha1_0_0`\
   \
   `./rude-bot-alpha1_0_0`&#x20;
5. Run in background with screen command:\
   `screen -S session1`\
   \
   Execute the bot `./rude-bot-alpha1_0_0`\
   \
   Leave the session with CTRL + D and then tap the letter A.\
   \
   Log back in to the session with `screen -r session1`
