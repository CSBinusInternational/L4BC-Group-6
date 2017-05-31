Tower of Beginning

 


Revision: 0.0.0

Final Project Report
Game Design Development



COMP6205 – Computer Graphics
Computer Science Program
Bina Nusantara University International
2016/2017 


License 
If you use this in any of your games. Give credit in the GDD (this document) to Alec Markarian and Benjamin Stanley. We did work so you don’t have to.   

Feel free to Modify, redistribute but not sell this document.


TL;DR - Keep the credits section of this document intact and we are good and do not sell it.






# Table of Content
1. Overview
2. Theme / Setting / Genre
3. Project Description
4. Core Gameplay Mechanics Brie
5. Targeted platforms
6. Project Scope
7. Project Limitations
8. How to operate the gam
9. Story and Gameplay
  * Story
  * Gameplay
10. Assets Needed
  * 2D
  * 3D
  * Animation
11. Schedule
   * Week #1 
   * Week #2
   * Week #3
   * Week #4
   * Week #5
12. Full Coding
   * https://github.com/CSBinusInternational/L4BC-Group-6
13. Screenshot of the Game





# Overview
 
## Theme / Setting / Genre

* Dungeon Crawling
* Survival
* Third-person

## Project Description 
	
&ensp;&ensp;Our group consist of two members, Luffandri (in charge of Back End) and Thedy Dinata (in charge of Planning, GUI, and Models). This is a game we created for our final project of Computer Graphics course at Binus International. We came with the idea because we love playing RPG games but at the same time have a survival mechanic into it. Our game is based on the Japanese anime series, Sword Art Online (SAO).
&ensp;&ensp;In this game, the player will be Kirito, the main protagonist in the series of Sword Art Online. The objective of the game is to survive and kill the boss inside the dungeon. The player wins when the enemy is dead. In the original series, when the level boss is cleared, they will move to the next level. However our game only simulate one of the level, so the game will end when the player win.



These are several steps how to play this game: 
1.	Click on the screen when the game starts.
2.	You will spawn on the middle of the arena, and you will see a menu.
3.	Go to the menu to choose the difficulty of that level.
4.	You can walk with WASD.
5.	You can rotate your camera with holding left or right mouse button and turn it around the player.
6.	You can attack with spacebar.
7.	You only can attack the same direction to your camera.
8.	When you choose the difficulty level, a monster will spawn on the other side of the arena.
9.	Your need to walk to the monster to aggro/provoke the enemy to start chasing you.
10.	You and your enemy will have a health bar which indicate your health status.
11.	You will die when your health bar reach 0.
12.	You will win the game when enemy’s health bar reach 0.

&ensp;&ensp;We used 2 character model, the first one is for the player model which is Kirito’s model and the second one is for the enemy model which is the wolf’s model. We planned to use more model for our game, however there are some errors and bugs when we tried to export the other model from blender to babylon. So we decided to use only one model for the enemy.
	
## Core Gameplay Mechanics Brief

* Survive: The player must survive the level.
* Movement: The player can move forward, backward, rotate to the left and right.
* Attack: The player can only attack enemy in front of them.
* Life: The player and monster have each own life and the system will always checks whether the player is alive or not. In addition, player can also die if it goes out of the arena.
* Algorithms and Maths: It used for the camera, the rotations of the player, check the range of the player and enemy, and check the position of the player.

## Targeted platforms

* Web-based platform, however limited to several browsers such as google chrome and mozilla firefox.

## Project Scope 
* Game Time Scale
  * Around 5 weeks

* 2 Men Team
  * Core Team
    * Luffandri (1901498321) + luffandrifandri@gmail.com
      * Back End and debugging.
    * Thedy Dinata (1901531054) + thedy_dinata@yahoo.co.id
      * Gui, Models, and Planning.

* Licenses / Hardware
  * Story : Sword Art Online (Reki Kawahara)
    * Enemy : Wolf (3DHaupt)
      * Link : https://www.blendswap.com/blends/view/24800
     * Character : Kirito (chelyzmarx)
      * Link : https://www.blendswap.com/blends/view/78512

     * Sound :
        * Link :
          * https://mp3tunes.ws/we-have-to-defeat-it-sword-art-online-extended-a5f4889
          * http://soundbible.com/130-Werewolf-Howl.html
          * http://soundbible.com/950-Bite.html
          * http://soundbible.com/1176-Sword-Swing.html
          * http://www.zedge.net/ringtone/1578930/

  * List of Tech/Library Being Used
    * Babylon.js
    * BabylonObjLoader.js
    * hand-1.3.7.js
    * canvas2d.js
    
* Project Limitations
  
  * Collision
    * The player and enemy cannot collide each other because we failed to use physics in this project. We tried to use it once and it makes the character rotation to spin around. So the player still can go through the other model such as the wolf.
  
  * Enemy Model
    * We decided to only use the wolf model because we could not found other models which can be export to babylon. Most of the models have textures which is cause problems when exporting from blender to babylon.
  
  * Wolf Animation
    * On the last minutes, we failed to make the wolf animation to stop when it is not chasing the player. We tried different ways to make it stop and all failed so we decided to keep the wolf animation to move all the time.

  * Story of the Game
    * At first we want to create the game which have some other floors and models like in the series, however because of time and due to many projects we decided to keep it simple. 

  * How to operate the game
    1.	Clone or pull from this repository.
    2.	Open index.html using your web browser (recommended to use mozilla firefox).
    3.	If the textures not load in the web, try using other web browsers or open it through web storm or using xampp.
    4.	All the other files such as textures, character’s model, sounds, images are inside the assets folder.
    5.	Good luck and have fun!




## Story and Gameplay

### Story 
&ensp;&ensp;The story begins when all people around the world start playing Virtual Reality Massively Multiplayer Role-Playing Game (VRMMORPG). A young boy that is a big fan of the game decides to start playing the game and little does he know that he will be trapped inside. Kirito will have to complete all the levels inside the tower to challenge the last boss and to escape from the game world. However if you die inside the game, you will also die in reality. Will he able to survives and saves everyone who are trapped inside the game?

### Gameplay 
&ensp;&ensp;Player will have to walk into a platform to summon an enemy. The goal condition of the game is that player will have to beat the enemy, and the losing condition is that the player dies. There are 2 possible ways of dying/losing, one is falling of the arena, and second is by getting killed by the enemy.


















## Assets Needed

* 2D
	* Textures
		* Environment Textures
			* Sky box textures
			* Ground textures
* 3D
	* Characters List
		* Kirito (player)
		* Wolf (enemy)
	* Environmental Art Lists
		* Arena
* Animation
	* Character Animations 
		* Player
* Kirito
	* Walk
	* Attack
* Wolf
	* Walk
	* Attack












## Schedule
* Week #1
	* Finalize our game
	* Search for the model which will be use for the characters

* Week #2
	* Search for the textures and fogs to make the game more realistics

* Week #3
	* Create the major part of the game
	* Health bars, UI, and many more

* Week #4
	* Create the arena
	* Create the movements of the characters

* Week #5
	* Create rpg style camera
	* Create falling from the arena
	* Create the combat system
	* Create the difficulties level
	* Put everythings into one
	* debug and finalize the game

	















## Full Coding
	- https://github.com/CSBinusInternational/L4BC-Group-6
## Screenshot of the Game

  * Start Screen	 
  
  * Summon Platform
	 
  * Enemy
	 
  * Gameplay
	 
  * Lose
	 
  * Win
	 
