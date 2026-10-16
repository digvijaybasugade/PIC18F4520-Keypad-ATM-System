# PIC18F4520-Based ATM System

## Project Overview
This project implements a basic ATM system using the PIC18F4520 microcontroller and Embedded C. It provides keypad-based PIN verification and menu-driven ATM operations with a 16×2 LCD display.

## Features
- Keypad-based PIN authentication
- Balance inquiry
- Cash withdrawal with balance validation
- Deposit with balance limit checking
- Token number generation
- LCD-based user messages
- UART serial communication
- Menu-driven user interface

## Hardware Requirements
- PIC18F4520 Microcontroller
- 4×4 Matrix Keypad
- 16×2 LCD Display
- UART serial communication interface
- Power supply and required interfacing components

## Software Requirements
- MPLAB IDE 8
- PIC18-compatible C compiler
- Proteus Design Suite (for simulation)

## Technologies Used
- Embedded C
- PIC18F4520
- UART Communication
- Keypad Interfacing
- LCD Interfacing
- Proteus Simulation

## Working Principle
The system receives a 12-character identification code through UART and compares it with predefined IDs in the firmware. If an ID matches, the user enters a four-digit PIN using the keypad.

After successful PIN verification, the ATM menu allows the user to check the balance, withdraw money, deposit money, or generate a token number. The LCD displays the corresponding messages and transaction results.

## Default Configuration
- Initial balance: 50000
- Initial token number: 1001
- PIN for ID 1: 5693
- PIN for ID 2: 2723

**Note:** These are demonstration values defined in the source code and should be changed before any real-world use.

## Project Structure
- `main.c` — Main program, UART functions, authentication, and ATM operations
- `lcd.h` — LCD function declarations and interface definitions
- `README.md` — Project documentation

## Future Improvements
- Improve keypad scanning and debouncing
- Add transaction history
- Improve authentication and error handling
- Integrate a suitable hardware interface for cash dispensing

## Author
Digvijay Dilip Basugade

## Disclaimer
This project is intended for educational purposes and microcontroller simulation. It is not a production-ready banking system.
