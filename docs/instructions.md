---
title: Instructions
description: "Project build instructions and user instructions for the app."
menu: Instructions
order: 30
---

{% include ddc-abbreviations.md %}

## Build instructions
{: menu="Build" }

 The user would first need to go to 'https://github.com/ddc-java-17/jata-android', and click the green 
 code button on the upper right hand side of the screen, then from that drop down copy the SSH key. 
 They should then open up Intellij IDEA (or whichever service they prefer to use), and select clone from CVS,
 where they can then paste in the SSH key and clone the repository as a gradle project. Next the user would 
 need to open up the local.properties file from the project view, in the app directory, and obtain and 
 insert the correct baseurl and client ID to connect to the server. From there the user can execute the run app task.


## User instructions
{: menu="User" }

 Once the user has opened the app and signed in through Google, they should first use the two drop-down 
 options on the home screen to select the board size and amount of players for the game they would like to play.
 Once their preferences are set, the user will hit start game. This will take them to a screen with their board 
 and ships. From here, the user can long press on any of their boats and use the move or rotate option to 
 set up their ships however they would like. Note that when moving a boat, the square on the grid that is
 selected is where the front of the boat will go, and it won't fit horizontally from that point, the boat
 will rotate down 90 degrees. If the boat wouldn't fit that way either, then the boat will stay in its 
 original position. When rotating a boat, it will rotate 90 degrees down from the first square on the 
 grid (left-most point of the boat) that that boat is located in. Once the user is satisfied with their ship placement,
they need to hit the "Armada ready, prepare for battle!" button at the bottom of the screen. The user must then
wait until they find a game. Once in a game, the user can swipe right or left on the screen to see other user's boards, 
or tap the display names shown at the top of the screen to navigate to those user's boards. When it is the 
user's turn to fire, a shots remaining counter and fire button will appear. The user can then navigate to 
whichever board they would like to fire on, and tap any square on the grid to place a shot, (a red circle will 
 appear confirming to the user that is where they would like to shoot, they can tap that same square again to remove
 that shot and place it somewhere else). Once the user has placed all their shots, they will press the fire button 
to send those shots. The squares on the grid that were fired at will then be filled with a white circle if the 
shot was a miss, or a red circle if the shot was a hit (these will also appear on the user's board when other 
 players fire at them). This process is repeated until only one player has ships remaining, making that user 
the winner. A simple text dialog will then appear on each user's screen with a "you win" or "you lose" 
message, along with a home button. The user can then press the home button to navigate back to the home screen 
and change the board size or player count if desired, or just start up a new game. 
