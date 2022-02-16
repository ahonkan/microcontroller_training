# microcontroller training
Objective of this training is to exercise the commonly used interfaces on a standard microcontroller such as STM32F Family.

## Parts
https://estore.st.com/en/nucleo-g071rb-cpn.html  

Microphone input: https://www.adafruit.com/product/1063  

Speaker driver: https://www.adafruit.com/product/2130  

I2C Temp: https://www.adafruit.com/product/1782  

FET Board:
https://www.amazon.com/Onyehn-Mosfet-Button-Arduino-Raspberry/dp/B07GLNCRR4/ref=pd_sbs_3/138-9532009-5015836?pd_rd_w=KG1oY&pf_rd_p=dfec2022-428d-4b18-a6d4-8f791333a139&pf_rd_r=3WP3FZHXNH9TTEDXBPCQ&pd_rd_r=ebb85f0e-da1c-434d-90f7-e5a66eb27be7&pd_rd_wg=5Jt2b&pd_rd_i=B07GLNCRR4&psc=1  

Optional:
https://www.totalphase.com/products/aardvark-i2cspi/  

## Setup IDE
Compile, Build & Debug simple application.
Know how to use JTAG debugger, set/clear breakpoints, view memory, attach to a running system.

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
Configure DAC with DMA to convert data out at a fixed rate.  
Create a DTMF Tone Generator.

## ADC & DMA
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



