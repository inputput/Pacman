# Pacman project!![Pac_Droite](https://user-images.githubusercontent.com/78816569/107407429-effac980-6b09-11eb-94ef-28b02d05eb48.png)~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Developed by Léo Meyne and Emilien Tellier from C2 group as part of the first semester of the "DUT Informatique" of Vélizy.
### Description :

* Developement of a program based on the example of the 80' game PACMAN.
* Language : C. 
* using "Libragphique" and "Makefile" that the school provides.
* The project unfold in five folders, one file "makefile" and this file.
 - data : this folder contains ".txt" files which are used to operate the program (4 game levels and "records.txt" that contains the highests scores).
 - imgae : this folder contains all the game's images (ghosts' sprites, paccman's, etc).
 - lib : "libgraphique"'s folder, contains "libgraphique{.c;.h}", the ".ttf" file that contains font and the patch note.
 - obj : this folder is empty before you build the program, then it contains ".o" objects files.
 - src : contains two ".c" files ("partie.c" and "main.c") and their matching ".h" files.
 - makefile : building tool.
 - readme.txt (this file).

### Installation :
Because it is in C language coded, you just have to build the program before running it.
To do this, make the game's folder your current directory, then execute "make" command that will build the program.
The compiled code is created, you now just have to run the command "./resultat".

### Usage :
* The launched program boot on the very first menu. To play, you just have to click on one of the three pictures which are matching a level of the game.
![56](https://user-images.githubusercontent.com/78816569/107412838-5682e600-6b10-11eb-8909-32370f5bf6ae.PNG)
* The game is now ready to begin whenever you'll have pressed a key.

* The graphic part of the game is split as following :
  * The top left part displays informations :
		- The remaining lifes (showed as visible pacman images (one equal one life))(first line).
		- The player's score (showed just down the remaining lifes and preceded by "Score :") .
		- Pacman's power disponibility ("disponible" or "indisponible" (Up or recharging)).
  
   *    The central part with the game's display.

*   We move pacman with keyboard's directional arrows.
*   Each time Pacman eats a "Pacboule" (small squares) it wins one point.
*	Ghosts are basicly following pacman, to eat him.
*	Whenever Pacman is going on a bonus (big circles), ghosts are changing their color and going backward, fearing pacman.
*	The fear is growing : Once the middle of the duration of the bonus is complete, ghosts are paralyzed and they stop moving.
*	In this time period, if pacman goes on a ghost, it eats it, and wins ten points.
*	The ghost's dying, it respawns on his original spawnpoint and then,the ghosts fear is reinitialised for ten game turns.
*	Pacman has a powerup, this power is acting as a bonus.
*	To use this powerup, the player has to press the space bar.(WARNING : powerups' using is stopping pacman's run until the player press a new key).
*	Once this powerup comes to it is the end, Pacman has to score 75 points to get it back.
*	The game is ending up to two conditions :
		- The easy one : Pacman has no more lifes, he dies and the player's lives is saved.
		- The hardest one : Pacman ate all the "Pacboules", ghosts have nothing more to protect, the game comes to it's end. and the player's score is saved.
		

### Support :

Are you experiencing an issue ?
You can contact us on our emails : telliemilien@gmail.com leo.meyne@gmail.com.
Or via the DUT's discord as "Leo Meyne" or "Emilien Tellier".

### Roadmap :

In the future it might be great to improve the graphism quality or the software global accessibility.

### Contributing :

The project is currently paused, that's why we aren't really interested in contribution. You can refer to the support section if you want to talk about potential ideas you have or amelioration axes you think that can be great. Your interest will always be useful to us, we do not leave this project as dead, just paused for the moment.

### Authors and acknowledgment

We are thanking our teachers for their contribution to our success in this project.
We also thank them for their time, out of office hours, and all their helpful advice.

### License :

This project is totally open source. You can take it for your own, and make it yours, at the exception of "partie.c","partie.h" and "makefile", that aren't even ours.
### Project Status :
As we said before, the project isn't currently living, it's paused, but :
* Segmentation bugs : it still exists segmentation bugs ( the crash indicate : segmentation error ).
* For the ghosts moving we use the pythagore theorem ( we use the hypotenuse to calculate the shortest way ) not a shortest way algorithm, so sometime the ghosts can be blocked and they can’t pass through another ghost.
* It exists also many “little bugs” because we didn’t have time to test a lot of time the last version before the deadline.
* A bug that given sometime an infinity live to pacman “auto-corrected” during the developpement, but I can maybe come back.
* Areas for improvement :
  -- Board Game’s display optimization ( just load the part of board game where ghosts and Pacman moving)
-- Add different difficulty level
--Better manage ghost AI.

