# Accelerometer Bubble Level
## Note
Unfortunately, the code for this old project has been lost in time. Hence this repository does not contain any code and is only an overview of the project.

## Description
This project is used to determine the flatness of the surface using a virtual bubble on a LCD screen which is interfaced to STM32F4 Discovery microcontoller. The virtual bubble displaces in the opposite direction of the tilt of the surface on which the microcontroller is placed on. The surface is said to be completely flat when the bubble is inside the box on the LCD screen.

## Components
* LCD screen : Nokia 5110 LCD (84 x 48). It uses the PCD8544 driver which is a low power CMOS LCD controller/driver, designed to drive a graphic display of 48 rows and 84 columns. The LCD is interfaced to the microcontroller using SPI.
* Microcontroller : STM32F4-discovery development board. It features 32-bit ARM Cortex-M4 processor, 1-MB Flash memory and 192-KB RAM. The discovery board also has a 3-axis accelerometer which is used for this project.

## Concept
The roll and pitch are calculated from accelerometer readings and then mapped onto X and Y coordinates of the LCD display. The accelerometer's pitch and roll vary from -90deg to +90deg. For the Nokia 5110 LCD (84 x 48), there are 84 pixels on the X axis and 48 pixels on Y axis. So on the X axis each pixel represents 180/84= 2.14deg and on the Y axis each pixel represents 180/48=3.75deg.

