<div align="center">
	<br>
	<p>
		<a href="https://discord.gg/ejEkDvZCzu"><img src="https://media.discordapp.net/attachments/1031166956541333675/1109981153282244730/BeFunky-design__1___2_-removebg-preview_1.png?width=497&height=156" width="780" alt="SLashy" /></a>
	</p>
	</br>
	<a href="https://discord.gg/vpHKcMZrrt"><img src="https://img.shields.io/badge/Support_Server-000?style=for-the-badge&logo=&color=informational" alt="Discord server" /></a>
	<a href="/"><img src="https://img.shields.io/badge/Version-2.0-000?style=for-the-badge&logo=&color=informational" alt="Version" /></a>
	<a href="https://github.com/TahaGorme/Slashy/stargazers"><img src="https://img.shields.io/github/stars/TahaGorme/Slashy?style=for-the-badge&logo=&color=blue" alt="Stars" /></a>
	<a href="https://github.com/TahaGorme/Slashy/network/members"><img src="https://img.shields.io/github/forks/TahaGorme/Slashy?style=for-the-badge&logo=&color=blue" alt="Forks" /></a>
	<a href="https://github.com/TahaGorme/Slashy/issues"><img src="https://img.shields.io/github/issues/TahaGorme/Slashy?style=for-the-badge&logo=&color=informational" alt="Issues" /></a>
	<a href="https://github.com/TahaGorme/Slashy/pulls"><img src="https://img.shields.io/github/issues-pr/TahaGorme/Slashy?style=for-the-badge&logo=&color=informational" alt="Pull Requests" /></a>
<br>
	<a href="https://replit.com/tahagorme/slashy"><img src="https://binbashbanana.github.io/deploy-buttons/buttons/remade/replit.svg" alt="Deploy on replit" /></a>

</br>
</div>

 ## About
Slashy is an advanced Dank Memer Grinder/Farmer Selfbot. It supports all the best Dank Memer commands for getting rich and bypasses anti-selfbot measures with intelligent solvers. 

## Features
- [x] User-friendly GUI for easy configuration, live stats & extensive logs
- [x] Supports running unlimited accounts
- [x] Completely undetectable
- [x] Supports a broad list of commands;
     `daily`,
     `beg`,
     `fish`,
     `hunt`,
     `dig`,
     `search`,
     `crime`,
     `postmemes`,
     `stream`,
     `adventure` &
     `trivia`
- [x] Automatically solves Dank Memer captcha's
- [x] Takes random breaks to avoid suspicion
- [x] Allows you to transfer items through serverpools automatically 
- [x] Automatically buys tools & reads alerts
- [x] Automatically plays minigames
- [x] Ability to auto-use customizable items

### In Development
- [x] Auto Pet Care
- [ ] Auto Work
- [ ] Auto Farm

## Installation
- Download [NodeJS](https://nodejs.org/en/download)
- Run the following commands in your shell/console:

```javascript
git clone https://github.com/TahaGorme/slashy.git
```

```javascript
cd slashy
```

```bash
npm i
```
- Now enter the correct values in [config.json](./config.json).

To start the selfbot, run the following command in your shell/console:
```javascript
node .
```

### Replit Deploy
- Go to: https://replit.com/tahagorme/slashy
- Create a so-called "secret", and name it "config", now, put your filled in [config.json](./config.json) in it.

### Tokens.txt Format
Whether you want to run Slashy in a specific channel or in DMs, you're going to need to use [tokens.txt](./tokens.txt) for your tokens.

- The format for this is either:
```js
channelId1 token1 // Use a single space to seperate the two values
channelId2 token2
```
or:
```js
token1
token2
```

## Config
```json
{
  "playInDms": false, // Whether to grind in Dank Memer's DMs or not.
  "password": "password", // The password needed to access your GUI
  "loginDelay": 100, // The delay in between logging into accounts
  "commands": [
    {
      "command": "beg", // The command
      "cooldown": 45000 // The cooldown for this command
    },
    {
      "command": "fish",
      "cooldown": 35000
    },
    {
      "command": "hunt",
      "cooldown": 35000
    },
    {
      "command": "search",
      "cooldown": 25000
    },
    {
      "command": "dig",
      "cooldown": 35000
    },
    {
      "command": "crime",
      "cooldown": 45000
    },
    {
      "command": "highlow",
      "cooldown": 25000
    },
    {
      "command": "trivia",
      "cooldown": 45000
    },
    {
      "command": "postmemes",
      "cooldown": 25000
    },
    { 
      "command": "stream",
      "cooldown": 300000
    }
  ],
  "autoAdventure": true, // Whether to play adventures
  "autoApple": true, // Whether to use or not to use apples automatically
  "autoDaily": true, // Whether to automatically claim your daily rewards
  "autoHorseShoe": true, // Whether to use or not to use horseshoes automatically
  "postMemesPlatforms": ["tiktok", "facebook"], // Preferred postmemes platforms
  "devMode": true, // Whether to use or not to use developer mode
  "webhookLogging": true, // Whether to log through webhooks or not
  "webhook": "https://discord.com/api/webhooks/1105165234848682097/8amxrSfjYiVPC4YdajckRqSBmPulfqkZqCrtqRPEEmNAASHHksrSZjBIy_83QifYTW-W", // Webhook link
  "triviaOdds": 0.95, // Odds for trivia to be successful
  "autoDeposit": true, // Whether to automatically deposit to your bank or not
  "searchLocations": [], // Locations to search in
  "autoBuy": true, // Whether to autobuy tools or not
  "serverEventsDonate": {
    "enabled": false, // Whether to donate or not
    "blacklist": [ // Items you want to blacklist from being donated
      "Apple",
      "Lucky Horseshoe",
      "Hunting Rifle",
      "Fishing Pole",
      "Shovel",
      "Trivia Trophy",
      "Adventure Ticket"
    ],
    "mainUserId": "userid" // The user to pay the items/coins to
  },
  "cooldowns": {
    "buttonClickDelay": {
      "minDelay": 350, // Minimum delay
      "maxDelay": 400 // Maximum delay
    },
    "triviaCooldown": {
      "minDelay": 350,
      "maxDelay": 400
    },
    "shortBreak": {
      "minDelay": 5000,
      "maxDelay": 40000,
      "frequency": 0.0005 // Frequency of going on break
    },
    "longBreak": {
      "minDelay": 300000,
      "maxDelay": 3000000,
      "frequency": 0.0005 // Frequency of going on break
    },
    "commandInterval": {
      "minDelay": 350,
      "maxDelay": 400
    }
  }
}
```

## Contributing
Pull requests & suggestions are always welcome! For major changes, please open an issue/DM us on Discord first to discuss what you would like to change and to what extend.

## License
[MIT](https://choosealicense.com/licenses/mit/)