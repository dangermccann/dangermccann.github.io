---
layout: page
title: Arduino Controlled FPS
permalink: /arduino-fps
hero_image: arduino-project.jpg
lead: This project demonstrates the ability for an Arduino-powered game controller to be used as an input source for a FPS game developed in Unity.  

sublead: |

  <p>
    <a href="https://github.com/dangermccann/MoonBase" class="btn btn-secondary px-4 py-2 btn-sm">Source Code</a>
  </p>

screenshots:
  - image_url: arduino-project.jpg
    caption: Prototype Controller 

---
### Hardware Components
- ATmega328P microcontroller
- MCP23017 I/O expansion ICs
- Joystick
- 7-segment display 
- Any number of number of LEDs and buttons

### Highlights

The Arduino program supports low-latency bidirectional communication with the Unity game runtime over a USB connection using the [WRMHL](https://github.com/relativty/wrmhl) library.  

