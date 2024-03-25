---
title: Overview
description: "Project proposal or summary of in-progress/completed project."
menu: Overview
order: 0
---

{% include ddc-abbreviations.md %}

## Summary

Have you ever thought Battleship was too friendly of a game?  Do you think the pig-pile is a great war-time tactic?  Json + the Arg(nauts) has both!  Json + the Arg(nauts) is a multi-player game app taking Battleship! to another level. In a game designed for 2-6 players, you may fight up to five other players!  
Turn-based game-play allows each player to see the effect of the other players shots.  Each player in an n-player game gets n shots to fire at whomever they choose. At the end of each players turn, the results of their shots are displayed on EVERYBODY'S screen. Just watch what happens when the first ship is located - ON ANY SCREEN!
## Intended users & user stories
{: menu="Users" }

Jata appeals to two types of players; the player who enjoys the challenges of multi-player gaming, and the player who enjoys piling on to someone who is already being shot at.

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

* Google sign-in service (Mandatory)
	> This service will be used to sign-in/out of your account on our app.

	> If the service is interrupted, players will not be able to access there accounts.
	
* Internet access (Mandatory)
	> This service will connect our app to the internet, allowing you to find other players for a game.

	> If this service is interrupted, the user will not be able to get into a game.
	
* Location services (Optional) (stretch goal)
	> Location  |  Android Developers

	> This service will allow users to find other users near by and join/invite them to a game.

	> If this service is interrupted or not allowed, users will not be able to find other near by users for a game.
	
* Messaging services (optional) (stretch goal)
	> Send simple data to other apps  |  Android Developers

	> This service will allow users to send friends/family texts messages inviting them to a game they have created.

	> If this service is interrupted or not allowed, users won’t be able to use texts as a means of inviting other users to a game.
	
* Jata API
	> Not created yet

	> API will take user requests to enter a game defined by certain number of players; take in a salvo from players and return if shots were hits, misses, or kills; track which players have been eliminated.

	> If interrupted, there would be no game/ game would crash.
	
* Vibrator
	> Vibrator  |  Android Developers

	> Will vibrate the phone when your ships have been hit, when your ships have been sunk, and when it’s the start of your turn.

	> If service is interrupted, phone won’t vibrate when the above actions occur.
	
* Media Player
	> MediaPlayer  |  Android Developers

	> Will allow the app to play sound effects according to what happens in the game.

	> If interrupted, the sound effects will not be played.

  
## Stretch goals and possible enhancements 
{: menu="Stretch goals" }

If you can identify functional elements of the software that you think might not be achievable in the scope of the project, but which would nonetheless add significant value if you were able to include them, list them here. For now, we recommend listing them in order of complexity/amount of work, from the least to the most.




