# Bot Setup Instructions

1. [Download zip file](https://github.com/AlexRubik/rude-bot-solana/releases) (on Linux, use the wget command) onto the machine you will run the bot on, unzip the zip file, and keep all files in the same folder.\
   e.g.,&#x20;

```
wget https://github.com/AlexRubik/rude-bot-solana/releases/download/v1.1.0-alpha/rude-bot-alpha1_1_0.zip
```

```
unzip rude-bot-alpha1_1_0.zip
```

```
cd rude-bot-alpha1_1_0
```

2. Modify your .env.example file (see [.env page](.env.md)) with nano or whatever text editor you use:&#x20;

```
nano .env.example
```

\
\- Rename it to .env with this command:&#x20;

```
mv .env.example .env
```

3. Modify your [baseConfig.json](baseconfig.json.md) with nano
4. Give it permission to execute and then run the executable provided:

```
chmod +x rude-bot-alpha1_1_0
```

```
./rude-bot-alpha1_1_0
```

Use CTRL + C to stop the bot.

5. We can run in background with screen command.

This creates a new terminal session:

```
screen -S session1
```

You may need to install `screen` with this command: `apt install screen`

\
After you have created your screen session, you can execute the bot

```
./rude-bot-alpha1_1_0
```

\
Leave the session with CTRL + D and then tap the letter A.\
\
Log back in to the session with `screen -r session1`
