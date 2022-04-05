# Introduction

This repository contains firmware for a pickup winder based on a Ramps 1.4 board, RepRadDiscount Full Graphics Smart Controller, a stepper motor, a servo and an Arduino Mega 2560 microcontroller board.

# Installation

- Assemble the pickup winder as can be seen in the picture below
- Use e.g. the Arduino IDE to flash the sketch in the src/ directory to the Mega 2560

# Usage

- Press the encoder button on the display to enter/leave a setting
- Rotate the encoder to change a setting. Since the display is so godawfully slow the code waits for a timeout until updating the display.
- Press the STOP button on the display to start the winding process
- Press the STOP button to stop the winding process, too ;)
- Press the STOP button twice (doubleclick) to reset the "Current Winds" counter to 0

# CAVEATS

- Do not use the encoder during the winding process. The stepper control should be robust, but the servo control is not. Everytime you move the encoder you will experience the servo jerking. This will take a little effort to do correcty.
- The "Current Winds" counter is only updated when the winding is stopped. Otherwise the display updates would interfere with the servo controll as well.

# LICENSE

- To be figured out

# Author

- Florian Paul Schmidt
- Florian Hofmann  

