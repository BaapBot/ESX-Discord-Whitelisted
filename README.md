# ESX-Discord-Whitelisted
ESX Discord Whitelisted


O que voce vai precisa.
Criar um arquivo com nome bot.js

E add

```js
const Discord = require("discord.js");
const bot = new Discord.Client({disableEveryone: true});
bot.commands = new Discord.Collection();

// Displays the message in console
bot.on("ready", async () => {
    console.log('\x1b[32m%s\x1b[0m', `${bot.user.username} is online and ready to do something! I'm live on ${bot.guilds.size} servers.`);
    bot.user.setActivity("Online Now", {type: "PLAYING"});

    bot.user.setStatus('Online') // Online, idle, invisible & dnd
});

// Bot Start
bot.on("message", async message => {
    if(cmd === `.hello`){
        return message.channel.send("Hello Mate!");
    }
});

bot.login("");
```

Tem que isntalar o node.js na maquina e o code vb tbm.
fuiii!!!
