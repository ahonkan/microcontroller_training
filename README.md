# microcontroller training
Objective of this training is to exercise the commonly used interfaces on a standard microcontroller such as STM32F Family.

## Parts
[NUCLEO-F446ZE](https://estore.st.com/en/nucleo-f446ze-cpn.html)  Currently Out Of Stock

## Setup IDE
- Download the IDE tool
- Get familiar with the project environment, settings, file and directory structure
- Compile, Build & Debug simple Hello Application.
- Know how to use JTAG debugger, set/clear breakpoints, view memory, attach to a running system for the simple hello application

## Configure Pin Mux Settings
Use configuration tool to configure GPIO pins to access LED & Buttons, then other facilities.

## LED Push Button- Main Loop
Use push button to control LED in Main Loop
Basic ARM CPU execution.

## LED Push Button- ARM Timer Control
Use push button to control LED via interrupt.
ARM Internal Timer Interrupt Operation.
Push Button Gates the LED which is triggered by Timer ISR.

## LED Push Button- GPIO Interrupt
Use push button to control LED via interrupt.
Specific SOC interrupt (STMicro) configuration.  Configure push button to toggle LED.
ARM extended interrupt table.
Play with WAI and low power operation

## UART Operation- Character Echo
Set up UART and echo character.

## UART Operation- Line Echo
Echo character and when the enter key is pressed, it prints out the full line, and starts over.

## UART Operation- Command Line processing
Echo characters, and when enter key is pressed, the string entered will be broken into words separated by spaces.
The first word is the command and the remaining are arguments.
Implement command:  "led on" and "led off"

## DAC DMA & Timer
https://www.adafruit.com/product/2130  

Configure DAC with DMA to convert data out at a fixed rate.  
Create a DTMF Tone Generator.

## ADC & DMA
https://www.adafruit.com/product/1063  

Configure ADC to capture analog signals, link with DMA to capture and store data.  
Capture from external signal generator if available.
Create a DTMF Tone Detector

## ADC & DAC- Audio Delay, Audio Speed up 
Connect ADC, DAC and record & play back sound at normal or at another rate based on push button 
Use DMA transfers to make this not take up cpu cycles and use timer to pace the DAC

## Timer - STM32F Timer Block
Use STM Timer interrupt to toggle LED 
Configure PWM to fixed duty cycle
Connect DMA to PWM reload and generate a ramp pwm signal

## I2C
I2C Temp: https://www.adafruit.com/product/1782  
Set up I2C temperature sensor.  Capture data based on periodic interrupt.

## SPI
Set up two SPI interfaces on board, one master one slave, and perform transactions.


Hardware faults
Memory page segmentation
Profiling
FreeRTOS

## USB (optional)

## Capstone Project: Temperature Controller
Physically attach temperature sensor to a power resistor.   
Use the temperature reading to control PWM on a FET driver that drives current through the power resistor.  Maintain fixed temperature on resistor.

## Capstone Project: N-Phase Switching Power Supply
PWM& ADC voltage feedback

## Capstone Project: N Baud Modem
Timers, ADC, DAC

## Capstone Project: Self Leveler
Accelerometer & Servo motor to keep a platform Level
I2C/SPI, PWM

## Capstone Project (Advance): USB Gadget Device
Configure USB as Audio input/output device- ADC/DAC
USB Annoy-a-tron:  USB configured as mouse (HID)  device and using screen feedback, make mouse move in patterns on the screen.
https://sourceforge.net/projects/mpos/



