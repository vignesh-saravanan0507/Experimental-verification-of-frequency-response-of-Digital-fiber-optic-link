# Experimental-verification-of-frequency-response-of-Digital-fiber-optic-link

# Fiber Optic Digital Link Experiment (660nm & 950nm)

## AIM
To study a **660nm & 950nm Fiber Optic Digital Link**.  
This experiment demonstrates how a digital signal can be transmitted over a fiber cable and reproduced at the receiver end.

---

## EQUIPMENTS REQUIRED
- Link-B Kit with power supply  
- Patch chords  
- 20 MHz Dual Channel Oscilloscope  
- 1 MHz Function Generator  
- 1 Meter Fiber Cable  

---

## THEORY
Fiber optic links can be used for transmission of both digital and analog signals. A typical fiber optic link consists of three main elements:

1. **Transmitter** – Converts electrical signals into optical signals.  
2. **Optical Fiber** – Serves as the transmission medium.  
3. **Receiver** – Converts optical signals back into electrical signals.

### Transmitter
- LED-based digital DC coupled transmitters are widely used due to ease of fabrication.  
- A TTL gate drives an NPN transistor, which modulates the LED (SFH450V or SFH756V).  
- The LED is turned ON and OFF to represent digital signals.

### Receiver
- The **SFH-551V** digital optodetector delivers a digital output with minimal external circuitry.  
- It integrates:
  - Photodiode  
  - Transimpedance amplifier  
  - Comparator  
  - Level shifter  

**Working principle:**
- The photodiode converts light into photocurrent.  
- The transimpedance amplifier converts photocurrent into voltage.  
- The comparator compares this voltage with a reference derived from a “blind” photodiode for synchronization.  
- The level shifter provides an open collector output stage with a catch diode to prevent transistor saturation.

---

## PROCEDURE
1. Refer to the block diagram and make the required connections.  
2. Connect the power supply to the Link-B kit with proper polarity and switch ON.  
3. Set switches and jumpers as follows:  
   - All fault switches **OFF**  
   - SW8 → TX position  
   - SW9 → TX1 position  
   - SW10 → TTL position  
   - JP5 → +5V position  
   - JP6 → shorted  
   - JP8 → Pulse position  
4. Feed a **TTL square wave (1 kHz)** from the function generator to the **IN post of Digital Buffer**.  
5. Connect **OUT of Digital Buffer → TX IN of Transmitter**.  
6. Loosen the cap of **SFH756V (660nm)**, insert the fiber, and tighten the cap.  
7. Connect the other end of the fiber to **SFH551V detector** carefully.  
8. Observe the detected signal at **TTL OUT** on the oscilloscope.  
9. Vary input frequency to measure digital bandwidth.  
   - Determine the frequency at which the detector fails to recover the signal (max bit rate).  
10. Switch SW9 → TX2 position.  
11. JP7 → +5V position.  
12. Remove fiber from SFH756V (660nm), loosen cap of **SFH450V (950nm)**, insert fiber, and tighten.  
13. Observe detected signal at **TTL OUT** on oscilloscope.  

---

## TABULATION

<img width="1244" height="1096" alt="image" src="https://github.com/user-attachments/assets/c01deb13-0838-4fdd-ab73-0305d72b624c" />

---

## MODEL GRAPH

---

## RESULT
The digital signal was successfully transmitted through **660nm and 950nm fiber optic links** and reproduced at the receiver end.  
The maximum bit rate of the digital link was determined experimentally.


