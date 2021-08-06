# Basic Discord.js Bot

__Installation__

Use `npm init` and it will create a package.json file

```sh
npm init
```

Now Make a File called `index.js` and type `npm i discord.js` in the terminal.

```sh
npm i discord.js
```

Get your bot token from **[Discord Developer Portal](https://discord.com/developers/docs)**

```javascript
const Discord = require("discord.js"); //discord.js lib
const client = new Discord.Client(); 
 

let prefix = "!";// or use the prefix that you want 

client.on("message", (message) => {

  if (!message.content.startsWith(prefix) || message.author.bot) return;
 
  if (message.content.startsWith(prefix + "ping")) { // ping command
    message.channel.send("pong."); // responds by sending pong 
 
  }
});
 
client.login("your bot token");//your discord bot token from Developer Portal

//end of the code 
```
To Start the Bot Use `node index.js` in the terminal.

```sh
node index.js
```

If you ned any help join the Support server.

### **[Discord Support Server](https://discord.gg/zRqEsZjFj8)**

