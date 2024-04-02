---
title: REST API Endpoints
description: "HTTP methods, parameters, payloads."
menu: Endpoints
order: 25

---

{% include ddc-abbreviations.md %}

## Get the current user

### Request

`GET /jata-world/users/me`

Gets the current user object and their information.

### Path Parameters

| Parameter | Description                                   |
|-----------|-----------------------------------------------|
| key       | UUID (unique identifier for the current user) |


### Responses

| Status | Body | Description           |
|--------|------|-----------------------|
| 200    | User | Current user returned |

## Update a user

### Request

`PUT /jata-world/users/me`

### Body

| Type   | Description                                          |
|--------|------------------------------------------------------|
| String | A new display name to be updated to the current user |

### Response

| Status | Type | Description                                    |
|--------|------|------------------------------------------------|
| 200    | User | The current user with the updated display name |

## Find a user by key

### Request

`GET /jata-world/users/{key}`

Finds a user by their key and returns their information.

### Path Parameters

| Parameter | Description                         |
|-----------|-------------------------------------|
| key       | UUID (unique identifier for a user) |


### Responses

| Status | Body | Description   |
|--------|------|---------------|
| 200    | User | User returned |



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


## Place a fleet of ships

### put

`PUT /jata-world/games/{gameKey}/ships`

Places all of the ships for the current user


### Path Parameters

| Type 	    | Description                       	     |
|-----------|-----------------------------------------|
| gameKey 	 | Unique identifier of the game resource	 |


### Body

| Type 	         | Description                       	        |
|----------------|--------------------------------------------|
| ShipLocation 	 | Array describing every location of a ship	 |


### Responses

| status          	 | body  	| description                             	                                                |
|-------------------|-------	|------------------------------------------------------------------------------------------|
| 201 created     	 | game  	| Ships placed and placement verified 	                                                    |
| 404 bad request 	 | error 	| Invalid ship placement, either off of the board or intersecting another ship           	 |
| 409 conflict 	    | error 	| attempted to place more ships after ships have already been placed           	           |


