Unfortunately I was sick last session and couldn't attend class. But - I picked up my Adruino Kit from the post office (there was has been some trouble with shipping & delivery, so it took a few more days till it arrived and I could pick it up). 

I unpacked everything and also looked into the slides from week2, looked at the different wires (--> use red for + and black for -), trying to follow the new insights. 

Revised the things from week 1, e.g. how to attach the lamp, how (and how NOT) to place a component on a breadboard...
![IMG_0234](https://github.com/user-attachments/assets/418d4ea5-43e5-467f-8ee5-ea6ebd779265)

LED (Light Emitting Diode)
- Long leg = + (Anode), Short leg = - (Kathode)
- Always needs a resistor to limit current (otherwise it burns out!)
- Safe current for common LEDs: max 15mA
- use a 220Ω resistor for this
- Different colors have different forward voltages:
  - Red / Yellow: 1.8–2.3V
  - Green / Blue / White: 2.8–3.6V
  - (This is why green LEDs can look dimmer with the same resistor!)

RGB LED
- One LED that contains Red, Green, Blue inside — 4 legs total
- Two types:
  - Common Anode (+): shared + leg → connect to 5V
  - Common Cathode (-): shared - leg → connect to GND
  - In class we use Common Cathode
- Needs 3 resistors (one per color)
- To make yellow: turn on Red + Green (no Blue)

Resistors
- Limits current so components don't break
- Two physical types:
  - THT (Through Hole) — the ones with legs we use on breadboards
  - SMD (Surface Mount) — tiny flat ones for circuit boards
- Value is read from the color bands on the body


Ohm's Law: 
V = I × R → voltage = current × resistance
I = V / R → current = voltage / resistance
R = V / I → resistance = voltage / current

Power Law: 
P = I × V → power = current × voltage (in Watts)
I = P / V
V = P / I

Why do we use a 220 Ω resistor for an LED? (copied from the slides, so I remember) 
For current limiting (otherwise)
<15mA: safe current for common LEDs
a 330 Ω would also work, the light will be dimmer

When looking at the two different types of circuts, some vague memories from my physics class in grade 8 or 9 came back to my mind ("Reihenschaltung", "Parallelschaltung"), but I think I need to relearn these :) 
I hope that I can follow along the next class (week3) well with my own Kit now! 
