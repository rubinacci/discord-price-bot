# Discord Price Bot Installation

## Pre-requisites
- A Github account
- A Heroku account
- A Discord account
- [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli) installed

## Repo Setup

1. Fork the [discord-price-bot](https://github.com/beethovenxfi/discord-price-bot) repo from BeethovenX
2. Edit line 18 of `src/bot.js` to use a relevant message for your project, this will display in Discord
3. Create a new file in your repo's root directory called `Procfile` - note capital P and no extension
4. Edit your Procfile to contain `worker: node src/bot.js`
5. Commit your changes

## Discord Setup

1. Go to [Discord Applications](https://discord.com/developers/applications) and create a New Application - give it a snappy name such as `STA Price (FTM)`
2. Click into the Bot tab, and create a bot
3. Generate a Token for the bot, copy and paste this somewhere safe
4. INCOMPLETE

## Heroku Setup

1. Create a new app with an appropriate name and region
2. For `Deployment Method`, select Github, connect to your account, and select your Pricebot repo
3. Click into the `Settings` tab, and click `Reveal Config Vars`
4. Create 7 sets of Config Vars:
```
DISCORD_TOKEN / token_from_discord_step_3_above
NAME / token_name_e.g._STA
ORACLE ADDRESS / 0x33365E1B22BbeF5766419e19f77c15fD3E0a8Ae5
PRICE_PRECISION / 2
RPC / https://rpc.ftm.tools
TOKEN_ADDRESS / token_contract_address_e.g._0x89D5e71E275B4bE094Df9551627BCF4E3b24cE22
TOKEN_DECIMALS / 18
```
5. Return to the Deploy tab, and under Manual Deploy click `Deploy Branch`, this will install and deploy your application
6. INCOMPLETE
