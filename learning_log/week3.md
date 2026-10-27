analogWrite() - PWM
- Pulse-Width Modulation, is a digital method of controlling analog power by rapidly switching a signal on and off.
- 0–255 : 0v - 5v (8 bits)
--> widely used technique in dimming LEDs, controlling motor speed, etc

Duty cycle: the propor tion of "on-time" in each cycle 

Oscilloscope (measures  voltage and displays it graphically) 

How to fade in or fade out the light? 
Arduino Code: 

void setup() {
  // put your setup code here, to run once:
  pinMode(3, OUTPUT);
}

// for loop
void loop() {
  // put your main code here, to run repeatedly:
  // fade in 
  for (int i = 0; i <= 225; i +=5){
    analogWrite(3, i); 
    delay(20);
  }
  

  // fade out
  // alles einmal umdrehen (Vorzeichen, etc.) 
  for (int i = 255; i >= 0; i -=5){
    analogWrite(3, i); 
    delay(20);
  }


<img width="1003" height="597" alt="analog_digital" src="https://github.com/user-attachments/assets/b5159fe8-df83-4fa6-81c8-691ac11f8899" />

Tilt Switch --> can detect tilting of an object! (has a little ball inside that closes the circle) 

Serial Baud Rate --> number of signal changes per second in a serial communication channel

- did some experimentation with the Tilt Switch (0,1,0,0,0,0,0,1..)
--> signal was disturbed when we move the Tilt Switsch (flackern, schwachses Signal)
--> pin is disconnected
- digital read between 0 and 1
- analog read (only on analog pins!) between 0 and 1023


Potentiometer (adjustable resistor, common use case: volume adjustment, has 3 pins, a wiper and a resistive strip) 
How it should look like on the board: 

![IMG_0244](https://github.com/user-attachments/assets/e345f37f-6d3f-4122-a8e1-2000d2b4d7b9)

- We learned how to dim a light and turn it on and off (basically built a lightswitch)
Arduino Code:

![IMG_0245](https://github.com/user-attachments/assets/23c805a4-a990-48f7-83d5-044c56f6ec74)

