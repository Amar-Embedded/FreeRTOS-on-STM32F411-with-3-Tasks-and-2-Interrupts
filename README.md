# FreeRTOS-on-STM32F411-with-3-Tasks-and-2-Interrupts

In this project, FreeRTOS I implemented on an STM32F411 microcontroller using a toolchain on Ubuntu. The system runs 3 concurrent tasks and handles 2 interrupts: one for an external pushbutton and another for an ADC (Analog-to-Digital Converter) potentiometer interrupt.

Components Used:
STM32F411 Microcontroller: Running FreeRTOS.
Pushbutton: External interrupt source.
Potentiometer: Analog input, with an ADC interrupt to monitor voltage levels.
FreeRTOS: Real-Time Operating System to handle task scheduling.

Functionality:
Task 1:
Printing Task1 on Minicom.
Task 2:
Printing Task2 on Minicom.
Task 3:
ADC Value Processing: Reads and displays the analog value from the potentiometer (12 bit resolution).

Interrupts:
External Pushbutton Interrupt:
This interrupt triggers when the user presses the external button. It toggls the LED.
ADC Interrupt:
When the potentiometer’s value changes crosses 2000 then LED will toggle again.
