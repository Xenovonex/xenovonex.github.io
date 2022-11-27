---
layout: default
title: Arduino Miss Teaque
---

[Back to Miscellaneous projects](./miscellaneous.md)
# Arduino LED mystery
### Date of Project: 12 October 2021
<img src="/assets/img/missteaque_arduino.PNG" alt="missteaque" width="300"/>

## Goal
Design and build a 8x8 LED configuration that can show different symbols and a sequence of arrows that lead to the solution of a mystery. 

## Process
* The LEDs are controlled by an Arduino.
* The LEDs are covered by a 3D-printed screen to make the colors visually more appealing.
* The LEDs show different symbols.
  - The symbols can be created in Paint. Python code is written to convert an 8x8 pixel image to C code that lights up the LEDs to show the corresponding image.
  - One can 'scroll' through a menu of symbols using 'left' and 'right' buttons. 
  - One can 'select' a symbol with a button after which a sequence of arrow symbols show.

## Result
Below is Github code for the image-to-LED conversion and the Arduino code. Also, a video of the working product is shown. 

### [Github code](https://github.com/Xenovonex/Miss_Teaque_Escape)

### Video of the Arduino LED mystery LED configurations and sequences
<video width="640" height="480" controls>
  <source src="./assets/img/missteaque_vid_r.mp4" type="video/mp4">
  Your browser does not support the video tag.
</video>

## Skills
* Arduino
* Mechatronics
* C programming
* Python
