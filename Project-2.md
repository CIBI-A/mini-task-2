### [Pix-a-Sketch](https://www.hackster.io/gatoninja236/pix-a-sketch-a-virtual-etch-a-sketch-on-an-led-matrix-dd3bae)

### Problem statement:
Use two rotary encoders to draw whatever picture in 64 x 64 RGB LED Matrix Panel

### Ideation:

Rotary encoder >> Arduino nano >>  RPi >> RGB Matrix HAT >> 64 x 64 RGB LED Matrix Panel

DOF sensor is used to erase random 5 pixels and a push button is used to erase totally.

##### My idea:

Rotary encoder >> Arduino Mega >> 64 x 64 RGB LED Matrix Panel 

Instead of using DOF sensor, push button to erase the last pixel(storing the positions in an array) and a toggle switch to erase totally


Advantages of my idea:
  * Arduino Mega has 54 digital IO pins which is lot to connect LED matrix, rotary encoder and push buttons.
  * LED matrix library is already present.
  * Cost is less.
  * Easy to implement
  
Disadvantages of actual project:
  * Requires Arduino Nano to connect rotary encoder since RPi has less GPIO pins which will be occupied by LED matrix.
  * Both RPi and Nano needed to be programmed.
  * It cannot erase last pixel.
  * Reqire LED matrix HAT
  * Hard to implement
  
  
  
[Interfacing LED matrix with Mega](https://wiki.dfrobot.com/64x64_RGB_LED_Matrix_-_3mm_pitch_SKU_DFR0499)  
