---
layout: page
title: Lord Mayor
permalink: /lord-mayor
hero_image: LordMayor-Icon-Wide.png
description: Lord Mayor is a real-time strategy game with a vintage aesthetic that plays like a cross between a puzzler and a city builder.   
lead: <a href="https://lordmayorgame.com/">Lord Mayor</a> is a real-time strategy game with a vintage aesthetic that plays like a cross between a puzzler and a city builder.   

sublead: |
  
  <p>
  You play a newly minted Gentleman who is challenged to build cities that meet the demands of His Majesty the King. You are given a limited amount of time and resources, and must place buildings carefully to optimize their yield and promote various qualities on which the city is judged.
  </p>
  <p>
    <a href="https://github.com/dangermccann/Lords" class="btn btn-secondary px-4 py-2 btn-sm">Source Code</a>
    <a href="https://lordmayorgame.com/" class="btn btn-secondary px-4 py-2 btn-sm">Website</a>
  </p>
  <p>
    <a href="https://store.steampowered.com/app/499330/Lord_Mayor/" class="btn btn-primary px-4 py-2 btn-sm"><span class="icon-steam"></span> Buy on Steam</a>
  </p>

screenshots:
  - image_url: gameplay1.png
    caption: Game map
  - image_url: gameplay6.png
    caption: Building selection dialog
  - image_url: help1.png
    caption: Help dialog
  - image_url: trade.png
    caption: Trade user interface
  - image_url: interstitial.png
    caption: Interstitial with level victory conditions

---

Each level is a new city that must be built from scratch, and each presents varying terrain and victory conditions. As you conquer each level you are promoted through the ranks toward the ultimate title of Lord Mayor.

I developed the game in Unity using C#.  All code was written by me from scratch, and visual assets were designed in Photoshop with the help of the [Vectorian](https://www.vectorian.net/) graphics pack.

### Project Status
The game was released for Windows, Mac and Linux on Steam in 2016 and is still available for purchase for $1.99.  Since the release I have opened sourced the project under the Creative Commons Attribution 4.0 International License.  

### Highlights
* The game map is a 2D [hexagonal grid](https://github.com/dangermccann/Lords/blob/master/Assets/Models/Hex.cs) of tiles that can be occupied by buildings placed by the player.  
* I'm generating the maps for each city in the game programmatically using a modified perlin noise [algorithm](https://github.com/dangermccann/Lords/blob/master/Assets/Maps/MapGenerator.cs).
*  [Buildings](https://github.com/dangermccann/Lords/blob/master/Assets/Models/Building.cs) provide resources to the city that can be used to improve the city's aggregate attributes or traded for other goods.   
* A player completes a [level](https://github.com/dangermccann/Lords/blob/master/Assets/Levels/Level.cs) by reaching the target aggregate scores for the city.  


### Technologies Used
- Unity
- C#
- Adobe Photoshop
