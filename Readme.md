# Zulip bot to help in rescue operations

This zulip bot is part of a project built for Hackverse hackathon.
 The main objective of this bot is to help people in rescue operations. Zulip is a great place to discuss and hence, this platform can be used by rescue operators to discuss strategy to excute tailored rescue operations for different distress locations. Anyone can join the zulip chat, interact with the bot and help to strategise a rescue plan.

## Why zulip?
Zulip provides a great platform where people can interact and plan in an effective way. The zulip bot acts as a ready interface so that people can discuss and analyse the information from the comfort of zulip, all from one single app, no need to switch between apps. Also, the bot's reply provides context for others.

## Usage
On a zulip chat thread, these commands are useful:

- `@distresssos report` : displays locations where distress was registered.
- `@distresssos rescue <int>` : rescue a person from distress location

## How to run this bot
This bot is currently deployed on Heroku and works with [hackverse-gods.zulipchat.com](hackverse-gods.zulipchat.com). Please make an id if you want to use this bot.

Or if you want to deploy your own clone this repo, obtain a zuliprc from zulipchat.com and put it into the root directory of the master branch. Now, type in these commands to deploy to heroku:

- `heroku create` - creates an app instance on heroku
- commit the zuliprc file, `git add .; git commit -m 'zuliprc added'`
-  `git push heroku master`
- `heroku dyno:scale worker=1` assign a worker dyno so that the app is online 24/7
### Thats it!!
