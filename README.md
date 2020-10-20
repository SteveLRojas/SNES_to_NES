# SNES_to_NES
This project is an adapter board designed to be installed inside a SNES gamepad.  
The source is written in assembly for the AT90S1200 MCU. All code is in the main ASM file.  
All the project details can be inferred from the source file, which is short, simple, and well commented.  
A single layer PCB design is included.  

Bug fix: added temporary nes variable in main. This is need so that the NES variable is always valid, as the NES console can trigger an interrupt and read it at any time.  
	In previous versions the A and B buttons had a small chance of getting pressed at random, which made games such as B-Wings effectively unplayable.  

News update: The AT90S1200 microcontroller used in this project has been obsolete for a very long time (~2004), so I will no longer maintain this project.
A new project has been created using an ATtiny24.
