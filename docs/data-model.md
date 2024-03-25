[data-model.md](data-model.md)---
title: Data Model
description: "UML class diagram, entity-relationship diagram and DDL."
menu: Data Model
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
- [`edu.cnm.deepdive.jata.entity.Game`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/entity/Game.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.entity.User`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/entity/User.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.entity.UserGame`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/entity/UserGame.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.entity.Fleet`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/entity/Fleet.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.entity.Ship`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/entity/Ship.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.entity.Shot`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/entity/Shot.java){:target="_blank"}

## Repositories
- [`edu.cnm.deepdive.jata.repository.GameRepository`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/dao/GameRepository.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.repository.UserRepository`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/dao/UserRepository.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.repository.UserGameRepository`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/dao/UserGameRepository.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.repository.FleetRepository`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/dao/FleetRepository.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.repository.ShipRepository`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/dao/ShipRepository.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.repository.ShotRepository`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/dao/ShotRepository.java){:target="_blank"}

