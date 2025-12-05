# Voice-Controlled-Smart-Home-Model
A voice-activated home automation prototype that uses Python for speech recognition and an Arduino Mega 2560 to control physical lighting circuits. This project demonstrates how to bridge high-level software (AI/Speech) with low-level hardware (LEDs/Relays).
 Jarvis-Lite: Voice Controlled Smart Home Model

# Demo
https://youtu.be/slHfhOEyEwg




Arduino Mega 2560 (1): The microcontroller brain.

LEDs (3): Red (Kitchen), Green (Bedroom), Blue (Living Room).

Resistors (3): 220Ω (to protect LEDs).

Breadboard (1): For prototyping connections.

Jumper Wires (7+): Male-to-Male type.

# Wiring Guide

Red LED (Kitchen): Connect Breadboard Row 10 to Arduino Pin 22.

Green LED (Bedroom): Connect Breadboard Row 15 to Arduino Pin 23.

Blue LED (Living Room): Connect Breadboard Row 20 to Arduino Pin 24.

> Note: Ensure all LEDs share a common Ground (GND) connection via the breadboard's negative rail.


# Software Installation

1. Arduino Setup

Download and install the Arduino IDE.

Open smart_home.ino.

Connect your Arduino Mega via USB.

Select Tools > Board > Arduino Mega 2560.

Select your Port (e.g., COM3) and click Upload.



2. Python Setup

Install Python 3.x on your computer.

Install the required libraries:


> pip install pyserial SpeechRecognition pyaudio


Open smart_home_voice.py and update the SERIAL_PORT variable to match your Arduino's port.



# Voice Commands

Once the Python script is running, try saying these commands:

"Turn on Kitchen" - Turns on the Red LED.

"Bedroom off" - Turns off the Green LED.

"Living room on" - Turns on the Blue LED.

"Party mode" - Turns ON all LEDs.

"System Deactivate" - Turns OFF all LEDs.



# Future Improvements

 Add an LCD screen to display the current status text.

Replace LEDs with 5V Relays to control actual desk lamps.

Add a specialized "wakeup word" like "Hey Jarvis".

