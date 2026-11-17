# Today was about Movement again! 
*Notes from class:* 

- introduced Stepper Motor 
- I was very happy that my code & setup from exercise 1 worked rigth away :)
- But my battery was probably low, so I powered the stepper directly from Arduino
- managed to change the rotation

Exercise 2: 
- defining the destination, not the movement!

- Pattern: "moveCW = !moveCW;" --> changes back and forth (boolean, not operator)

I struggled with Exercise 3: setting the pins up correctly by myself and also adjusting the code so that thes stepper stops, when I touch the sensor, but managed to fix it in the end (with some help) :) 

*What I learned:* 
- stepper motor moves in small, exact steps instead of just to an angle like a servo --> good for very precise positioning and for strong torque at low speed
- downside: it's trickier to use. It needs a matching driver board, and every stepper model has different specs, so the code can differ
- this week we used the 28BYJ-48 stepper with a ULN2003 driver board. The four driver inputs (IN1–IN4) go to four pins on the Arduino, and the driver and Arduino must share the same GND!!
- a stepper can be powered from a power module or directly from the Arduino's 5V
- Steps per revolution tells how many steps the motor needs for one full turn --> `moveDegrees()` converts between degrees and steps so I don't have to calculate it myself
- RPM (revolutions per minute) sets the speed, and I can use it to work out how long a movement takes
- a stepper doesn't know its current position - that's the difference between `move()` (relative movement) and `moveTo()` (absolute position)
- Blocking vs. non-blocking functions: `moveDegrees()`, `move()` and `moveTo()` pause the whole sketch until the movement is done. `newMoveDegrees()`, `newMove()` and `newMoveTo()` together with `stepper.run()` in `loop()` let the Arduino do other things while the motor moves
- i connected a touch sensor (0 = no touch, 1 = touched) to pin 2 and used it to stop the motor while it's touched (struggled here to set it up correctly)

else: 
- bigger stepper types exist too: NEMA motors with drivers like the A4988, DRV8825 or TMC2208. Steppers can drive a threaded rod or a pulley with belt
- to "home" a stepper (find its starting position), you can use a limit switch or a magnet with a Hall effect sensor



Photos: 1. Exercise Set up and 2. Exercise Set up 
[week6_photos.pdf](https://github.com/user-attachments/files/34967853/week6_photos.pdf)

Last Exercise: 
[week6_photos.2.pdf](https://github.com/user-attachments/files/34968535/week6_photos.2.pdf)
