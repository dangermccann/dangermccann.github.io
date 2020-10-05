---
layout: default
title: Lord Mayor Game
permalink: /lordmayor
---

# Lord Mayor Game
![Lord Mayor Gameplay](./assets/images/gameplay1.png "Lord Mayor Gameplay")

Lord Mayor is a real-time strategy game with a vintage aesthetic that plays like a cross between a puzzler and a city builder. You play a newly minted Gentleman who is challenged to build cities that meet the demands of His Majesty the King. You are given a limited amount of time and resources, and must place buildings carefully to optimize their yield and promote various qualities on which the city is judged.

Each level is a new city that must be built from scratch, and each presents varying terrain and victory conditions. As you conquer each level you are promoted through the ranks toward the ultimate title of Lord Mayor.

I developed the game in Unity using C#.  All code was written by me from scratch, and visual assets were designed in Photoshop with the help of the [Vectorian](https://www.vectorian.net/) graphics pack.

- [Lord Mayor website](https://lordmayorgame.com/)
- [Source code](https://github.com/dangermccann/Lords)
- [Purchase game on Steam](https://store.steampowered.com/app/499330/Lord_Mayor/)

### Project Status
The game was released for Windows, Mac and Linux on Steam in 2016 and is still available for purchase for $1.99.  Since the release I have opened sourced the project under the Creative Commons Attribution 4.0 International License.  

### Highlights
* The game map is a 2D [hexagonal grid](https://github.com/dangermccann/Lords/blob/master/Assets/Models/Hex.cs) of tiles that can be occupied by buildings placed by the player.  
* I'm generating the maps for each city in the game programmatically using a modified perlin noise [algorithm](https://github.com/dangermccann/Lords/blob/master/Assets/Maps/MapGenerator.cs).
*  [Buildings](https://github.com/dangermccann/Lords/blob/master/Assets/Models/Building.cs) provide resources to the city that can be used to improve the city's aggregate attributes or traded for other goods.   
* A player completes a [level](https://github.com/dangermccann/Lords/blob/master/Assets/Levels/Level.cs) by reaching the target aggregate scores for the city.  

### Screen shots
![Building selection dialog](./assets/images/gameplay6.png "Building selection dialog")
Building selection dialog

---

![Help dialog](./assets/images/help1.png "Help dialog")
Help dialog

---

![Trade user interface](./assets/images/trade.png "Trade user interface")
Trade user interface

---

![Interstitial with level victory conditions](./assets/images/interstitial.png "Interstitial with level victory conditions")
Interstitial with level victory conditions

---
