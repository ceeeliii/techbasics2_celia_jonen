This week was all about sound!

- introduced the buzzer
- Difference between passive and active buzzers:
  Passive --> it requires a signal in order to make sound
  Active --> it can produce sound directly when connected to power (longer leg is +)
- With `tone(pin, frequency, duration)` I can play different notes on a passive buzzer
- A melody is just two arrays: one for the notes and one for how long each note lasts
- There are several pre-inszalled libraries in Arduino that contain code for differnt sounds, melodies etc.

- introduced the Ultrasonic Distance Sensor (looks like a music blaster)
- ground = -
- Ucc = power supply
- Trippger pin and Echo Pin
- sends out a sound and measures how long the echo takes to come back --> from that time the Arduino calculates the distance

![IMG_0446](https://github.com/user-attachments/assets/bf187d15-b907-420e-ae7e-b9af3c4c79ae)
![IMG_0445](https://github.com/user-attachments/assets/a1e726a4-e724-44a4-b0d4-6d784ffc08fc)
![IMG_0443](https://github.com/user-attachments/assets/e9f14e49-4fae-4839-ba81-8da1d6c38bde)
![IMG_0442](https://github.com/user-attachments/assets/edfb6578-8c67-4255-ab3f-6d278c65d822)
![IMG_0440](https://github.com/user-attachments/assets/f60f8f4f-a6d1-466d-b1a1-0d80c417b177)


Buttons:
- Push buttons need a **pull-up or pull-down resistor**, otherwise the pin reads random values
- A multimeter is a useful debugging tool for checking connections, voltage and resistance

Things I need to remember: 
- definen PinMode
- always add ; in the end of a line!
- when do I need to use print, read,etc..?c


What I want to try next:
- Make a small instrument with several buttons, where each button plays a different note --> also in connection to my final project which I want to start thinking about 
- Try the pull-up version of the button circuit (couldn't figure it out this week)
