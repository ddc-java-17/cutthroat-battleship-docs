---
title: Overview
description: "Project proposal or summary of in-progress/completed project."
menu: Overview
order: 0
---

{% include ddc-abbreviations.md %}

## Summary

Have you ever thought Battleship was too friendly of a game?  Do you think the pig-pile is a great war-time tactic?  Cutthroat Battleship has both!  Cutthroat Battleship is a multi-player game app taking Battleship! to another level. In a game designed for 2-6 players, you may fight up to five other players!  
Turn-based game-play allows each player to see the effect of the other players shots.  Each player in an n-player game gets n shots to fire at whomever they choose. At the end of each players turn, the results of their shots are displayed on EVERYBODY'S screen. Just watch what happens when the first ship is located - ON ANY SCREEN!
## Intended users & user stories
{: menu="Users" }

Cutthroat Battleship appeals to two types of players; the player who enjoys the challenges of multi-player gaming, and the player who enjoys piling on to someone who is already being shot at.

* Players who enjoy challenges.

  > As someone who enjoys challenging multi-player games, I play this game because winning takes a keen understanding of game theory and not just a little luck.

* Players who enjoy pig-piling.

  > As someone who enjoys creating misery, I play this game because I can use all my shots to sink an entire ship in one turn!


## Functionality

The player will be able to see all play screen with the results of everybody's shots.
  * Swipe left/right to see any play screen
  * Select location of shot placement
  * See placement of their own ships
  * See game statistics including current rank and number of games played

## Persistent data
{: menu="Persistence" }

The app will store the following peristent data
* User
  * Display name
  * OAuth2.0 identifier
  * Timestamp of first login to the app
* Game
  * Number of games played
  * Game difficulty (# of players)
  * Current rank
  

    
## Device/external services
{: menu="Services" }

If the client component will need to access special services of the device (e.g., sensors, contacts, messaging), list them here using a bullet list. Also, if the client component will need to access already-existing external services (e.g., real-time weather data, Open Movie Database, Open Trivia Database), those should also be listed here; any such references to external services should include links to the main page or API description page for the service.

## Stretch goals and possible enhancements 
{: menu="Stretch goals" }

If you can identify functional elements of the software that you think might not be achievable in the scope of the project, but which would nonetheless add significant value if you were able to include them, list them here. For now, we recommend listing them in order of complexity/amount of work, from the least to the most.
