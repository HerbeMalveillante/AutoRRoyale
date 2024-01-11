# AutoRRoyale

A smart, free and open source Python-based bot for the Rush Royale mobile game

## What is this project ?

AutoRRoyale is a bot for the Rush Royale mobile game.
This game is a tower defense game where you play with or against other players to defeat waves of monsters. It's very entertaining, but it can be time consuming and repetitive to farm gold to upgrade your deck.

I want to make it clear that this bot is not meant to be used to cheat in the game. I am not responsible for any ban that could be caused by the use of this bot. I created this project as a challenge and to learn more about AI, game theory and image processing. It is an experiment and I do not recommend using it.

Now that MyGames lawyers are happy, let's talk about the project itself.

## Features

This section is a TODO list and a feature list at the same time. I will update it as I add new features. I plan to add features from the most basic to the most advanced, allowing the bot to automate more and more of the game, adding QoL features and improving the winrate as I go.

### Basic features

- [ ] Try to know what screen / state the game is in (fight, menus, etc.)
- [ ] Launch a coop game on any map from any screen.
- [ ] Extract all the information from the game screen : tower types, tower merge ranks, active spells, tower levels, incoming boss, wave number, mana count, hero charge, etc.
- [ ] Merge two towers
- [ ] Upgrade a tower
- [ ] Use the hero ability
- [ ] Create a tower
- [ ] Extremely basic AI

### Advanced features

- [ ] Play on repeat
- [ ] Report the results of the games, the rewards and the statistics of the game and send them to a Discord channel
- [ ] Detect when something is going wrong (bot is stuck, game crashed, etc.) and send a notification to a Discord channel
- [ ] Try to fix itself when something is going wrong
- [ ] Improve the AI : create an algorithm to determine the best move to make, based on the current game state and statistics

### "This is never going to happen" features

- [ ] Automatically watch ads whenever available to earn extra rewards
- [ ] Automatically collect the additional rewards (quests rewards, battle pass rewards, Ad Chest rewards, etc.)
- [ ] Automatically use maps when available
- [ ] Automatically buy everything in the shop when available
- [ ] Automatically upgrade cards when available
- [ ] Play PvP
- [ ] Create AIs for different decks, and log statistics about the winrate of each AI to determine the optimal deck

### Note

More features could be added after that, to make the bot absolutely 100% automatic from a fresh save to a really solid account and winrate. It would be exponentially more difficult to implement though, and I don't think I will ever get to that point. Furthermore, this would involve complex game theory that I'm not sure I'm ready to tackle yet.

## Technical details

The bot is written in Python. The game is played on an Android Emulator for several reasons :

- Cross platform support on Windows, Linux and MacOS
- Easy to automate
- The bot can run indefinitely without having to worry about being unable to use your phone
- Multiple instances of the game can be run at the same time, allowing the bot to play on multiple accounts simultaneously

The emulator I'm using to develop the bot is Android Studio's emulator. It is free, open source and easy to use. It is also the official emulator for Android development, so it is well maintained and updated. In the future, I might implement a calibration system to allow the bot to work on any emulator.

A detailed guide on how to set up the emulator and the bot will be available later on.

## The deck used by the bot

For now, the bot will play on coop mode only, so it would be logical to use a support deck, which involves less strategy than a DPS deck. However, I happen to play a DPS deck which is upgraded enough to be able to carry a game even if the other players are underlevelled.

Furthermore, I know this deck pretty well, so it will be easier for me to create an AI for it.

The deck is the following :

- Demon Hunter
- Mime
- Clown
- Portal Mage
- Dryad
