Learning Log - Week 5 

Movement! 
- introduced Servo Motor

1. Exercise:
- makes it move 180 degrees, interruptetd --> add a delay

Code e.g. (just makes it move in one half) 
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

