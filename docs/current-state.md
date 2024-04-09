---
title: Current State
description: "Current state of completion, known deficiencies, and test environments used."
menu: State
order: 40
---

{% include ddc-abbreviations.md %}

## Completion state
{: menu="Completion" }
Basic server-side functionality has been completed.  Users may start a game, set preferences for board size and player count, add and move ships and place shots. Server side defines board size, as well as number of ships and size of those ships for certain board sizes.  Fired shots are compared against ships and return a hit value, also return a drawable so players can tell if it was a hit or miss. Players can toggle shots
before firing, a red circle will be placed in the square on the grid the user taps, marking where their shot will be fired. That same square can be tapped again to remove that shot and allow it to be placed somewhere else.
Ships and shots are validated against the edge of the board.  ShipLocations are further validated against other ships in a particular user's fleet.  Users are prohibited from placing additional ships once the first set is placed. Shots are limited based on players in game/ still alive, user's may not place more shots than allowed.
swiping between boards has been implemented, along with tab navigation where you can just click a user's display name to get to their board. Turn counter implemented, moves on to next user after last user's shots were placed. Fire shots button only appears when it is your turn, so you can't fire out of turn. You win/ you lose pop-ups appear when game ends, along with a home button that navigates you back to the home screen.
Basic play through of a game works, with possible update bugs on the first round. Registers when a user's fleet is sunk, removing them from the turn counter, so they can no longer fire and lowers the shot count for user's still alive by one.


## Known deficiencies
{: menu="Deficiencies" }
This implementation is missing the following:
 - fleet is sunk/player dead - works, pop-up message only displays at end of game, not right when sunk.
 - no statistics or reporting services
 - drawables don't rotate properly 
 - intermediate update bugs
 - no extensive tests performed on other android devices 
 - no tests done is landscape mode
 - game not fully operational in landscape mode 
 - start game button gone in landscape mode, can't scroll to get it


### Fixed deficiencies 
- turn counter - implemented
- status - implemented
- legal ship instantiation testing - implemented
- join game/add another player - implemented
- end game indication - implemented
- control of returned information (Json View) - implemented
- n-1 shot counter and reduction as players die - implemented 
 - ship is sunk - decided against providing this information


## Test environments used
{: menu="Environments" }
Database was tested with simple text commands through an HTTP interface.
Ships were placed using the ships endpoint.  Additional users were added by placing a fake oauthKey into the database and restarting the server.
Samsung s 23 - physical device
Samsung galaxy note 20 - physical device 
Samsung galaxy s 24 - physical device


