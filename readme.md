# Discord Price Bot Installation

## Pre-requisites
- A Github account
- A Heroku account
- A Discord account
- [Heroku CLI](https://devcenter.heroku.com/articles/heroku-cli) installed

## Code Setup

1. Fork the [discord-price-bot](https://github.com/beethovenxfi/discord-price-bot) repo from BeethovenX
2. Edit line 18 of src/bot.js to use a relevant message for your project, this will display in Discord
3. Create a new file in your repo's root directory called 'Procfile' - note capital P and no extension
4. Edit your Procfile to contain 'worker: node src/bot.js'
5. Commit your changes

## Heroku Setup

