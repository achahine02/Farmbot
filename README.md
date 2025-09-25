# Farmbot
Farmbot project as part of my internship at FH Joanneum

This project documents the design and integration of a 24 V water pump system into the FarmBot Genesis v1.6
 platform, carried out in collaboration with FH Joanneum.

The goal was to reliably control a diaphragm water pump using the Farmduino’s peripheral outputs while protecting the board from overcurrent and inductive loads. To achieve this, we developed a dedicated relay + power supply system housed in a custom-designed enclosure.

🔧 System Overview

The Farmduino peripheral pin is used only as a low-current signal to switch a 24 V relay module.

The relay module controls the connection between a separate 24 V power supply and the water pump.

A custom enclosure was designed and fabricated to house the relay module and PSU, ensuring safe wiring and maintainability.

This approach keeps the pump current (2.5–6 A) fully isolated from the Farmduino, while still allowing control via the FarmBot web interface.

🛠 Hardware Used

FarmBot Genesis 1.6 (Farmduino board + Raspberry Pi 4)

24 V diaphragm pump (nominal 2.5 A)

24 V relay module (4-channel, optocoupler-based)

24 V power supply for pump (independent from Farmduino PSU)

Custom relay + PSU enclosure 

🚀 Outcomes

Safe, reliable pump control integrated into the FarmBot platform.

Modular design: the pump system can be swapped or upgraded without modifying the Farmduino board.

Documentation and open-source sharing to support other FarmBot users with similar needs.
