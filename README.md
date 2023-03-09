#      DiscordJS V14 Handler

![Discord Shield](https://discordapp.com/api/guilds/1076890610855837746/widget.png?style=shield)
![Version](https://img.shields.io/static/v1?label=Version&message=1.0.0&color=blue)
![DJS](https://img.shields.io/badge/Discord.js-14.7.1-green)
![Status](https://img.shields.io/badge/Status-Ready%20to%20work!-green)
![Replit](https://img.shields.io/badge/Replit-000000?link=http://left&link=https://replit.com/@yuvrajrastogi7/DiscordJS-v14-Handler?style=for-the-badge&logo=replit&logoColor=white)

Create a powerful Discord bot with ease using our Discord.js handler. Our handler is designed for both beginner and advanced developers with its simple interface and advanced features. With built-in autocomplete and modal functionality, you can quickly and easily create and manage commands for your bot. Get started today and take your Discord bot to the next level! [Want help? feel free to ask](https://discord.gg/Fy5mqEBjkS)

**For Replit:** [Click here](https://replit.com/@yuvrajrastogi7/DiscordJS-v14-Handler)

- Simple interface for both beginner and advanced developers

- Autocomplete functionality

- Modal functionality

- Highly customizable to suit your specific needs

- Built using Discord.js library version 14

# Setting up

- First, download the Discord.js handler as a ZIP file and extract it

- Open the extracted folder in VS Code

-  Create a `.env` file and add the following code: 

```js

TOKEN=YOUR_TOKEN

GuildID=YOUR_TESTING_SERVER_ID

```

Note: If you don't want to use a `.env` file, you can modify the `Config/bot.js` file like this: 

```js

require("dotenv").config();
module.exports = {
  TOKEN:
    process.env.TOKEN || "Token_Here", // Replace (Token_Here) to your bot token 
  PREFIX: process.env.PREFIX || ",",
  Slash: {
    Global: true, // set false for loading slash command in your testing guild make sure you add your server id
    GuildID: process.env.GuildID || "ID", // Your testing Server ID
  },

};

```

- After that install these packages by using `npm int`, `npm install` command:

    - discord.js

    - dotenv

    - pretty-ms@^7.0.1

    - mongoose@^6.7.5

- Finally, use the command `node .` to run your bot and start using the Discord.js handler.

# Guide
If you want to our handler in replit then [click here](https://replit.com/@yuvrajrastogi7/DiscordJS-v14-Handler).

After setup is complete, you can start adding commands and events to your bot. Here's where to put them:

- `Commands/Slash/`: for adding slash commands

- `Commands/Message/`: for message commands

- `Events/`: for events

- `Function/`: for adding some utility functions

- `Config/bot.js`: for adding some configuration

To get started, simply create a new file in the appropriate folder and start writing your code. Here's an example of what the basic structure of a command file might look like:

```js

module.exports = {
    name: " ",
    description: " ",
    // ...
   run: async (args, client , interaction) => {
   interaction.reply({
          content: "Thanks for using our handler!",
          ephemeral: true // Can be false
  })
}
};

```

# Need Help? Contact us!

Join our community and create ticket or create post in forums. [Join now](https://discord.gg/ezdeDThy)

![My Discord](https://discord-readme-badge.vercel.app/api?id=760002115049095238)

