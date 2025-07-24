
# Tokenless Block Instrument Explanation
#
## This repository presents a complete information about token block instrument, especially in railways how it works its features and all the required things.
---
A tokenless block instrument is a railway signaling device used primarily on single line sections to control train movements without the need for physical tokens, which were traditionally used as the authority for a train to proceed into a block section. Instead, tokenless block systems rely on electrical interlocking and coded signals to ensure safe and exclusive occupancy of a block section by only one train at a time.
## Working Principle
**Purpose:** The instrument ensures that only one train is allowed in a single line block section at any time to prevent collisions. It confirms the section is clear before allowing the next train to enter.

**Tokenless Operation:** Unlike the traditional token system where a physical token was handed to the driver, the tokenless block instrument transmits coded electrical signals or pulses between two stations controlling the block section, thus providing authority electronically rather than physically

**Role of Block Handle and Indications:** The instrument typically has a handle with positions such as Normal (Line Closed), Train Going To, and Train Coming From. The handle's position helps set the status of the block section and grants authority for train movement. When set to "Train Going To" or "Train Coming From," the block handle allows the signals to be cleared for train passage. The handle movement is electrically locked and controlled to enforce safety interlocks

**Interlocking Mechanism:** Before a train is allowed to enter the block, both station masters must cooperate to set the block handle appropriately. The system electrically interlocks the two ends to prevent conflicting movements and controls the last stop signals accordingly

**Typical Applications**: Commonly used in Indian Railways for single line operations, this instrument supports both Radio-Equipped (RE) and Non-RE areas, working on standard DC power supplies and often integrated with signal interlocks to last stop signals
#
## Type of Tokenless Block Instrument Used in Railways
Indian Railways primarily uses the Handle Type Tokenless Block Instrument, often referred to as the “Daido Type” or the Handle Type FM Tokenless Block Instrument for single line sections.This system replaces traditional token exchange methods with electrically coded signals and robust interlocking to regulate train movements safely.The image shows the tokenless block instrument used in railways.

  <img width="400" height="300" alt="image" align="center" src="https://github.com/user-attachments/assets/74b44e1f-3e9e-48ab-8043-bc27b7a1c78f" />
  <img width="300" height="300" alt="image" src="https://github.com/user-attachments/assets/fa3c3b4a-f00c-4a28-aabd-264c6b5007c8" />
  
  
  
  
## Key Components
#

**Block Handle:** Operated between three positions—Normal (Line Closed), Train Going To (TGT), and Train Coming From (TCF).

**Galvanoscope:** Shows the presence and direction of line currents.

**Time Release Indicator:** Indicates the status of time-release mechanisms, ensuring the block is safely released only after the required delay.

**TOL Indicator:** “Train On Line” indicator glows red when a train occupies the block section.

**Counters:** Track line clear cancellations and pushback operations.

**Push Buttons (PB1 & PB2):** Used for sending and receiving coded signals between stations.
#
## How It Works
**Request for Line Clear:**

The sending station (A) initiates a request using the bell code, and the receiving station (B) acknowledges.

**Operation of Block Handles:**

After coordination, handles at both stations are turned—B to “Train Coming From” (to accept), A to “Train Going To” (to send).

This action closes interlocks and sets signals for train movement.

**Electronic Coded Signalling:**

The instrument sends modulated frequency tones (e.g., 1800Hz or 2700Hz, modulated by 65Hz or 85Hz) as coded authority to proceed.

**Train Movements:**

When the train enters the block, the TOL (Train on Line) indicator lights up at both stations and buzzers sound.

Track circuits at signals further confirm movement and release signals as the train clears sections.

**Block Release:**

Once the train leaves the section and is detected at the reception station, staff reset the handles. The “Train on Line” indicator switches off, unlocking the block for the next movement.

This system is the modern standard for single-line absolute block working in Indian Railways and many other networks, offering safety with increased operational efficiency.
#
Now we will simplify the above things with the help of diagrams


<img width="900" height="800" src="https://github.com/souravlouha/Electronics_Industrial_Training/blob/main/tokenless%20block%20instrument/images/1.png" />

In this circuit we have two inputs(Red wires) and the black wires are grounded. The output is a buzzer, when the train passed from one station towards another station the buzzer beeps indicating that the train successfully passed the station. Here also we have a dual timer ic(NE 556) The NE556 is a dual timer integrated circuit that contains two independent 555 timer circuits packed in a single 14-pin IC. It is designed to provide precise timing and oscillation functions such as time delay generation, pulse width modulation (PWM), pulse generation, sequential timing, and oscillators.

<img width="900" height="800" src="https://github.com/souravlouha/Electronics_Industrial_Training/blob/main/tokenless%20block%20instrument/images/2.png" />

The circuit requires 25 Volt. Since we have only one input so we connected only one input and other is not connected. And the output is connected to the buzzer as shown in the above image.  

<img width="900" height="800" src="https://github.com/souravlouha/Electronics_Industrial_Training/blob/main/tokenless%20block%20instrument/images/3.png" />

<img width="900" height="800" src="https://github.com/souravlouha/Electronics_Industrial_Training/blob/main/tokenless%20block%20instrument/images/4.png" />

<img width="900" height="800" src="https://github.com/souravlouha/Electronics_Industrial_Training/blob/main/tokenless%20block%20instrument/images/5.png" />

<img width="900" height="800" src="https://github.com/souravlouha/Electronics_Industrial_Training/blob/main/tokenless%20block%20instrument/images/6.png" />

Now in type 1, it work indivisually in every station. When the train enters the station it sends a signal that train has enter the station. and when it leaves it sends another signal that the train has left the station. We have explained this with the helps of mobile and the red and the green lines as shown in the images.



<img width="900" height="800" src="https://github.com/souravlouha/Electronics_Industrial_Training/blob/main/tokenless%20block%20instrument/images/7.png" />

<img width="900" height="800" src="https://github.com/souravlouha/Electronics_Industrial_Training/blob/main/tokenless%20block%20instrument/images/8.png" />

Now in type 2, it works in between the two stations. When the train leaves one station it produces a beep sounds and sends it to another station to indicate that the train has successfully left the station and proceeds towards another station.






