---
title: Data Model - Server
description: "UML class diagram, entity-relationship diagram and DDL."
menu: Server Data Model
order: 20
ddl: sql/ddl.sql
erd:
  image: img/erd.svg
  pdf: pdf/erd.pdf
uml:
  image: img/uml-server-side.svg
  pdf: pdf/uml-server-side.pdf
---

{% include ddc-abbreviations.md %}

{% include uml.md %}

{% include erd.md %}

{% include ddl.md %}

## Entity Classes
- [`edu.cnm.deepdive.jata.model.entity.Game`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/entity/Game.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.model.entity.User`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/entity/User.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.model.entity.UserGame`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/entity/UserGame.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.model.entity.ShipLocation`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/entity/ShipLocation.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.model.entity.Shot`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/entity/Shot.java){:target="_blank"}

## Repositories
- [`edu.cnm.deepdive.jata.model.dao.GameRepository`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/dao/GameRepository.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.model.dao.UserRepository`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/dao/UserRepository.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.model.dao.UserGameRepository`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/dao/UserGameRepository.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.model.dao.ShipLocationRepository`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/dao/ShipLocationRepository.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.model.dao.ShotRepository`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/dao/ShotRepository.java){:target="_blank"}


## REST Controllers
- [`edu.cnm.deepdive.jata.controller.GameController`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/controller/GameController.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.controller.UserController`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/controller/UserController.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.controller.ShipLocationController`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/controller/ShipLocationController.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.controller.ShotController`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/controller/ShotController.java){:target="_blank"}

## Service
- [`edu.cnm.deepdive.jata.service.GameService`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/service/GameService.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.service.AbstractGameService`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/service/AbstractGameService.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.service.UserService`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/service/UserService.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.service.AbstractUserService`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/service/AbstractUserService.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.service.ShipLocationService`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/service/ShipLocationService.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.service.AbstractShipLocationService`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/service/AbstractShipLocationService.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.service.ShotService`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/service/ShotService.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.service.AbstractShotService`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/service/AbstractShotService.java){:target="_blank"}
