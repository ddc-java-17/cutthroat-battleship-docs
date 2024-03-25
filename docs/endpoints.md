[data-model.md](data-model.md)---
title: REST API Endpoints
description: "HTTP methods, parameters, payloads."
menu: Endpoints
order: 25

---

{% include ddc-abbreviations.md %}


## Start a game

### request

`POST /jata-world/games`

Starts a new game, populates player pool.


### Body

| Type 	| Description                       	|
|------	|-----------------------------------	|
| game 	| board size/ player count settings 	|


### Responses

| status          	| body  	| description                             	|
|-----------------	|-------	|-----------------------------------------	|
| 201 created     	| game  	| game started and player pool populated. 	|
| 404 bad request 	| error 	| server unable to be reached.            	|



