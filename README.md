# Discord Server Nickname Enforcer

 A simple script that monitors and resets your chosen nickname on a Discord server, ensuring it remains unchanged even if altered by random server staff or bots.

## Using

To use this script, follow these steps:

1. Place the script (name-enforcer.js) and the config file (name-enforcer.json) in the same directory
2. Populate the config with the details for one or more servers -- the config is a JSON array of server objects (user ID, guild ID, intended nickname, token)
3. Run with [Deno](https://deno.land)

```deno run --allow-net --allow-read name-enforcer.js```

## Example Configuration

Here's an example config with two different servers

```[
    {
        "userId": "4000000000000000000",
        "intendedName": "Name111",
        "auth": "YOUR_DISCORD_TOKEN_HERE",
        "guild": "1111111111111111111"
    },
    {
        "userId": "6000000000000000000",
        "intendedName": "Name222",
        "auth": "YOUR_DISCORD_TOKEN_HERE",
        "guild": "22222222222222222222"
    }
]```
