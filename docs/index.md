---
title: Overview
description: "Project proposal or summary of in-progress/completed project."
menu: Overview
order: 0
---

{% include ddc-abbreviations.md %}

## Summary

Replace this paragraph with one or more paragraphs summarizing the purpose and operation of software you are planning to develop for this project.

{: menu="Users" }
## Intended users & user stories

Write a bullet list here, including at least 2 different types of intended users. Make it reasonably specific; simply saying "Anyone who likes games" (for example) is not sufficiently specific.

For each type of intended user, include at least 1 _user story_. A user story is usually just 1 simple sentence (no more than 2 sentences), in the voice of the intended user, stating a specific task that the user performs using the app, and the benefit that will be obtained. The simplest user stories take the form 

> As a <type of intended user (_who_)> I want to <use of specific feature or functionality (_what_)> so that <benefit (_why_).

Please avoid writing too much for the user story. In particular, if the way the user story is written makes it difficult to see the _who_, _what_, and _why_, then you probably need to re-write it more directly. (On the other hand, a user story should not simply be a re-statement of the intended user description.)

Here is one (silly) example of an intended user, along with a user story. Please note not only the conceptual structure, but the Markdown syntax used.

* People who like to use randomness in their decision-making.

    > As someone who enjoys randomness in my life, I use this app to flip a virtual coin or roll one or more virtual dice, so that I can base my decisions on randomness without having to carry coins or dice in my pockets.

## Functionality

List (using a bullet list---or ordered list, if order is relevant) the key functional aspects that will be provided by the app---i.e., tell us what the user will be able to do using the app. This should not simply be a re-statement of the [summary](#summary), but should instead provide a more specific articulation of the functionality and user experience. 

{: menu="Persistence" }
## Persistent data

Using a bullet list, list what content will be maintained in non-volatile storage---including filesystems, relational or non-relational databases, a thord-party cloud-based storage service, etc.

{: menu="Services" }
## Device/external services

If any component of the system will utilize (or even require) an external service, or a host service separate from the components of this project, beyond the components for the persistence summarized above, list them here.

{: menu="Stretch goals" }
## Stretch goals and possible enhancements 

If you can identify functional elements of the software that you think might not be achievable in the scope of the project, but which would nonetheless add significant value if you were able to include them, list them here. For now, we recommend listing them in order of complexity/amount of work, from the least to the most.
