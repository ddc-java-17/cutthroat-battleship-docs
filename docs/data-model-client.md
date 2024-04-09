---
title: Data Model - Client
description: "UML class diagram, entity-relationship diagram and DDL."
menu: Client Data Model
order: 20
uml:
  image: img/uml-client-side.svg
  pdf: pdf/uml-client-side.pdf
---

{% include ddc-abbreviations.md %}

{% include uml.md %}

## Entity Classes
- [`edu.cnm.deepdive.jata.model.entity.User`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/model/entity/User.java){:target="_blank"}

## Repositories
- [`edu.cnm.deepdive.jata.service.UserRepository`](https://github.com/ddc-java-17/jata-service/blob/main/src/main/java/edu/cnm/deepdive/jata/service/UserRepository.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.service.JataRepository`](https://github.com/ddc-java-17/jata-android/blob/main/app/src/main/java/edu/cnm/deepdive/jata/service/JataRepository.java){:target="_blank"}

## Service
- [`edu.cnm.deepdive.jata.service.JataServiceProxy`](https://github.com/ddc-java-17/jata-android/blob/main/app/src/main/java/edu/cnm/deepdive/jata/service/JataServiceProxy.java){:target="_blank"}
- [`edu.cnm.deepdive.jata.service.JataLongPollServiceProxy`](https://github.com/ddc-java-17/jata-android/blob/main/app/src/main/java/edu/cnm/deepdive/jata/service/JataLongPollServiceProxy.java){:target="_blank"}
