## Learning Log - Week 5 

*Movement*

1. Exercise:
- makes it move 180 degrees, interruptetd --> add a delay

Code example from Arduino (just makes it move in one half) 

#include <Servo.h>
Servo myservo;

void setup() {
  // attach pin 9 to the servo object
  // it can be any digital pin
  myservo.attach(9);
}

void loop() {
  // write to a position from 0 to 180

  for (int i=0; i <= 180; i +- 5) {
    myservo.write(i);
    delay(10);
  }

}


## What I learned (summary) 
- there are different motor types: servo motors, stepper motors** and DC motors
- a positional servo (like the SG90) moves to a specific angle between 0° and 180°. A continuous servo doesn't hold an angle but spins, and the signal controls its speed instead
- a servo has 3 wires: power (5V), GND and a signal wire that goes to a digital pin on the Arduino
- to control it I use the `Servo.h` library. `myservo.attach(9)` connects the servo to a pin and `myservo.write(angle)` moves it to a position
- `delay()` gives the servo time to reach its position before the next command (don't forghet to add that!)
- to make a servo move slowly, I move it in small steps (e.g. 1° at a time in a `for` loop with a short delay) instead of jumping straight to the end position
- a potentiometer gives an analog value from 0 to 1023 with `analogRead()`
- with `map()` I can turn that into an angle from 0 to 180 and control the servo by turning the knob
- a joystick has two analog axes (X and Y, read on A0 and A1) and a push button
- at rest the analog values are around the middle (about 512)
- the joystick button needs `INPUT_PULLUP`, so it reads 1 when not pressed and 0 when pressed

Examples for ussage (projects):
- servos are used in robotic arms, animatronic eyes, moving tails and even wearable jewelry. That showed me how much can be done with such a small motor

## What I struggled with
- figuring out the correct code by myself, putting all different commands together in the right order/ combining them
- code still feels kinda weird or hard to grasp for me, but I feel like I'm becomming more familiar with how Arduino in general works
- following class - sometimes all codings or items on the board sound the same to me hah
