🚪 Automatic Garage Door Control – PLC Project
📘 Overview

This project demonstrates an Automatic Garage Door Control System implemented using a Fatek PLC and programmed with WinProLadder software.
The system provides both manual and automatic control modes, ensuring safe and efficient door operation with visual indicators and timed automation.

🧩 Hardware Components

Fatek PLC (FBs Series)

Start, Stop, Open, Close Push Buttons

Auto Mode Switch (Slide Switch)

Open Limit Switch

Close Limit Switch

Indicator Lamps (Red & Green)

Garage Door Motor (Forward/Reverse control)

Power Supply Unit

🧠 Software & Programming

PLC Software: WinProLadder

Language: Ladder Logic

Programming Platform: Fatek PLC Communication via RS232/USB

🪜 Ladder Logic Description

The program logic is divided into several sections:

Initialization & Power Control – System activates via Start button.

Manual Operation – Door opens/closes through push buttons; stops at limit switches.

Indicator Control – Lights indicate door position (fully open → Green, fully closed → Red).

Automatic Mode – Using a timer (T1), if the door remains open for 30 seconds, it automatically starts closing.

Emergency Stop – Stop button interrupts all active coils and timers immediately.

⏱️ Timing Logic

T1 (Auto Close Delay Timer): 30 seconds ON-delay timer activated when the door is fully open and Auto mode is ON.

🖥️ Simulation / Implementation

The ladder logic was simulated using WinProLadder.

Tested on a Fatek PLC with actual hardware connections for validation.

The door control sequence works reliably in both manual and automatic modes.
