---

layout: default
---

This portfolio contains a variety of projects that I've put together in my spare time over the years.  

# [Optix Ray Tracer & Path Tracer](./pathtracer)
[![Ray Traced Spheres](./assets/images/three-spheres.png "Ray Traced Spheres")](./pathtracer)

For this project I wrote a general purpose path tracer in C++ using the [NVIDA OptiX 7.1](https://developer.nvidia.com/optix) ray tracing engine.  The program demonstrates a variety of different rendering techniques from simple Lambertian shading to complex physically based rendering with multiple importance sampling.  

The application parses a scene file to build a graph containing vertices, triangles, spheres, material data and lighting data; it then builds the Optix pipeline containing the ray tracing programs, global acceleration structure containing the scene graph and shader binding table containing the material and lighting data.  The pipeline and data is then sent to the GPU and the ray generation program is launched.  

- Source code can be shared upon request.  [Contact me](./contact/)

[Read more...](./pathtracer)


---

# [Lord Mayor](./lordmayor)
[![Lord Mayor Gameplay](./assets/images/gameplay1.png "Lord Mayor Gameplay")](./lordmayor)

Lord Mayor is a real-time strategy game with a vintage aesthetic that plays like a cross between a puzzler and a city builder. You play a newly minted Gentleman who is challenged to build cities that meet the demands of His Majesty the King. You are given a limited amount of time and resources, and must place buildings carefully to optimize their yield and promote various qualities on which the city is judged.

Each level is a new city that must be built from scratch, and each presents varying terrain and victory conditions. As you conquer each level you are promoted through the ranks toward the ultimate title of Lord Mayor.

I developed the game in Unity using C#.  All code was written by me from scratch, and visual assets were designed in Photoshop with the help of the [Vectorian](https://www.vectorian.net/) graphics pack.

- [Lord Mayor website](https://lordmayorgame.com/)
- [Source code](https://github.com/dangermccann/Lords)
- [Purchase game on Steam](https://store.steampowered.com/app/499330/Lord_Mayor/)


[Read more...](./lordmayor)

---

# DCPU-IDE
[![DCPU-IDE Screenshot](./assets/images/dcpu-ide.png "DCPU-IDE Screenshot")](./dcpuide)
DCPU-IDE a set of visual tools for developing software for the fictitious [DCPU-16 processor](https://github.com/dangermccann/dcpu16-ide/blob/master/specification.txt), a processor architecture developed for the defunct video game [0x10c](https://en.wikipedia.org/wiki/0x10c).  The suite of tools includes an assembler, emulator, editor and visual debugger that supports breakpoints, variable watches and memory contents.  

The tools and site are written in JavaScript, and custom user programs are stored in AWS DynamoDB.  

- [DCPU-IDE website](https://www.dcpu-ide.com) 
- [Source code and documentation](https://github.com/dangermccann/dcpu16-ide) 

---

# Untitled Base Defence Game
![Defense Game Screenshot](./assets/images/defense-game.png "Defense Game Screenshot")
This project is an unfinished, untitled base defense game where the player must protect their base for an onslaught of enemy ships.  The player can place turrets to fend off the attack and reactors that generate positive energy over time.  Dispensers can be used to launch a drone to attack an enemy spawner.  The player completes the level by accumulating enough energy from their reactors to reach the level target.  If enough enemy ships make it through the player's defences, the player's energy level reaches zero, and the player is defeated.  

I developed the game from scratch in Unity using C#.  I modeled all 3D assets from scratch in Blender and used Substance Painter and Photoshop to create the textures.  

- [Source code and game assets](https://github.com/dangermccann/Untitled)

---

# Arduino Controlled FPS
![Picture of Arduino and hardware](./assets/images/arduino-project.jpg "Picture of Arduino and hardware")
This project demonstrates the ability for an Arduino-powered game controller to be used as an input source for a FPS game developed in Unity.  The game controller consists of a ATmega328P microcontroller, one or more MCP23017 I/O expansion ICs, a joystick, a 7-segment display and an arbitrary number of LEDs and buttons.

The Arduino program supports low-latency bidirectional communication with the Unity game runtime over a USB connection using the [WRMHL](https://github.com/relativty/wrmhl) library.  

- [Source code](https://github.com/dangermccann/MoonBase)


---



