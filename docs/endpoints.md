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


## Submit a shot 

### request 

`POST /jata-world/games/{gameId}/shots`

submits a shot in the game specified by gameId.


### Path parameters

| Parameter 	| Description                         	|
|-----------	|-------------------------------------	|
| gameId    	| Unique identifier of game resource. 	|


### Body

| Type 	| Description         	|
|------	|---------------------	|
| Shot 	| Coordinates of shot 	|


### Responses 

| Status          	| Body  	| Description                  	|
|-----------------	|-------	|------------------------------	|
| 201 ok          	| shot  	| Shot submitted successfully. 	|
| 400 bad request 	| Error 	| Invalid shot placement.      	|

