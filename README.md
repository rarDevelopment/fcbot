# fcbot

Hello and welcome to fcbot!

I didn't know if this would work out or not so there's not much documentation.

## Table of contents
- Using fcbot
  - [Setup without league updates](#setup-without-league-updates)
  - [Setup with a public league](#setup-with-a-public-league)
  - [Setup with a private league](#setup-with-a-public-league)
- Commands
  - [For everyone](#for-everyone)
  - [Admin-only](#admin-only)
- [FAQ](#faq)

## Using fcbot

You can add fcbot to your Discord, if you're an admin, by going to

https://discord.com/api/oauth2/authorize?client_id=671814513967890459&permissions=2048&scope=bot


Then, you'll have to set it up.

### Setup without league updates

In ANY channel in your server that Fantasy Critic Bot is in:
```
    !fcadd <name of a channel you want updates to go to>
    !fcstart
```
Example:
```
    !fcadd fantasy-critic
    !fcstart
```

That's it!

You can !fcadd multiple channels if you want.

### Setup with a public league

***Note: this currently only works with 2020 public leagues. To fix very soon.***

In ANY channel in your server that Fantasy Critic Bot is in:
```
    !fcadd <name of a channel you want updates to go to>
    !fcleague <league ID>
    !fcstart
```

Example:
```
    !fcadd fantasy-critic
    !fcleague abb1234f-44c0-2c7d-9901-80aa314d26f6
    !fcstart
```

You can find your league ID in the URL of your league's page. 
https://www.fantasycritic.games/league/YOUR-LEAGUE-ID-HERE/2020

### Setup with a private league

In ANY channel in your server that Fantasy Critic Bot is in:
```
    !fcadd <name of a channel you want updates to go to>
    !fclogin <login email> <password> <league ID> <league year>
    !fcstart
```

Example:
```
    !fcadd fantasy-critic
    !fclogin supergreg@gmail.com s3cr3tpa55w0rd abb1234f-44c0-2c7d-9901-80aa314d26f6 2020
    !fcstart
```

Yes, typing your password into discord is a bad, stupid idea. 
You can do it in a private channel, you can delete the message after you 
send it. Sorry. This bot was just for me at first. Hopefully this will improve
soon. It should be in a PM or something.

You can find your league ID in the URL of your league's page. 
https://www.fantasycritic.games/league/YOUR-LEAGUE-ID-HERE/2020

## Command list

### For everyone

 * `!fcscore`: Show a leaderboard for your league.
 * `!fccheck <search string>`: searches for a game and tells you about it. (Score, classification, release date, etc.)
 * `!fchelp`: Show available commands.

### Admin-only

 * `!fcadd <channel name>`: Add a channel that should receive updates from fcbot.
 * `!fcremove <channel name>`: Remove a channel from receiving updates.
 * `!fcleague <league ID>`: Set this fcbot to monitor the given public league.
 * `!fclogin <email> <password> <league ID> <league year>`: Set this fcbot to monitor the given private league.
 * `!fcstart`: Begin posting updates to added channels.
 * `!fcstop`: Stop posting any updates.
 * `!fcstatus`: List added channels, whether updates are active, etc.
 * `!fcadminhelp`: Show admin commands.

## FAQ

### What happens with 2021 public leagues, once they exist??

Unsupported for now, but it will be a small change once 2021 leagues are here. I will get to it then.

### It's broken aahhh

I'm on discord as DrCat#2160, send me a PM and I will try to help.
