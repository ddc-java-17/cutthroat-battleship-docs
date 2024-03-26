---
title: REST API Endpoints
description: "HTTP methods, parameters, payloads."
menu: Endpoints
order: 25

---

{% include ddc-abbreviations.md %}


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




