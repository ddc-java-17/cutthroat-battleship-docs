---
title: Current State
description: "Current state of completion, known deficiencies, and test environments used."
menu: State
order: 40
---

{% include ddc-abbreviations.md %}

## Completion state
{: menu="Completion" }
Basic server-side functionality has been completed.  Users may start a game, add ships and place shots.  Fired shots are compared against ships and return a hit value.
Ships and shots are validated against the edge of the board.  ShipLocations are further validated against other ships in a particular user's fleet.  Users are prohibited from placing additional ships once the first set is placed.


## Known deficiencies
{: menu="Deficiencies" }
This implementation is missing the following:
 - ship is sunk
 - fleet is sunk/player dead
 - turn counter
 - status
 - legal ship instantiation testing
 - join game/add another player
 - end game indication
 - control of returned information (Json View)
 - n-1 shot counter and reduction as players die
 - no statistics or reporting services


## Test environments used
{: menu="Environments" }
Database was tested with simple text commands through an HTTP interface.
Ships were placed using the ships endpoint.  Additional users were added by placing a fake oauthKey into the database and restarting the server.


