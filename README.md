# Quiz Buzzer System

A digital logic-based quiz buzzer system designed to identify the first participant
to press their button, lock out subsequent inputs, and indicate the registered
participant using LEDs and a buzzer.

## Project Overview

This project implements a quiz buzzer system using digital logic ICs instead of
a microcontroller. Four participant buttons are provided, and the system
registers the first button press.

Once a participant is registered, subsequent button presses are ignored until
the administrator presses the reset button.

## How It Works

1. The system is powered on and initialized.
2. The administrator presses the reset button to prepare the system for a new round.
3. When a participant presses their button, the corresponding input is processed
   by the logic gates.
4. The CD4013 D flip-flops store the registered state.
5. The SN74HC08N AND gates control the logic required to prevent subsequent
   participants from being registered.
6. The corresponding LED and buzzer indicate the registered participant.
7. The registered state remains stored even after the button is released.
8. The administrator presses reset to clear the stored state and start the next round.

## Main Components

- CD4013BD D Flip-Flops x2 (IC)
- SN74HC08N AND Gates x2 (IC)
- Push Buttons
- LEDs
- Buzzer
- 220Ω and 1kΩ Resistors
- 1N4007 Diodes
- 5V DC Supply

## Features

- First-press detection
- Subsequent-input lockout
- LED indication
- Buzzer feedback
- Reset functionality
- Microcontroller-free digital logic implementation
- 
## Team

- Pruthviraj Kute
- Adarsh Maurya
- Mubasshir Memon
- Shlok Mishra
