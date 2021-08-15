# Temperature-Controlled-Fan

- In this project, I have implemented a Temperature Regulation system using 8051 Microcontroller in Assembly Language. 
- This project aims to regulate the speed or switch off the fan based on the surrounding temperature which is measured using a temperature sensor. 
- The analog values obtained are then passed through an ADC converting it to digital, which then parses it to the Microcontroller for calculations. Based on the temperature, it decides the speed of the fan and displays the necessary information. 
- We regulate the voltage the fan receives based on the temperature of the surroundings, if it is greater than 35°C, the fan runs at max speed, when it is between 25°C and 35°C at medium speed and turns off when the temperature is below 25°C.

NOTE: I couldn't obtain a plastic fan for the basic hardware demo, so instead I used a wheel as a substitute for a fan.

NOTE: The rotation of the wheels cannot be visualized in the Output Images.


The repository consists of:
- The proteus simulation file 
- The assembly language code on Keil uVision (C51) IDE.

Hardware Requirements:
1.	AT89S52 Microcontroller Development Board
2.	LM-35 Temperature Sensor
3.	ADC0804 IC
4.	LCD – 16x2
5.	5V DC Motor
6.	5V Relay
7.	Resistors - 10kΩ 
8.	Resistors - 1kΩ
9.	Capacitors – 150pF
10.	10kΩ Potentiometer
11.	IN4007 Diode
12.	2N222 NPN Transistor
13.	Connecting Wires

Software Requirements:
1.	Keil uVision IDE – For assembly language coding
2.	ProgISP – For uploading the code to the microcontroller
3.	Proteus – For Software design and simulation of the circuit

Block Diagram:

![image](https://user-images.githubusercontent.com/69978515/129463718-9e21a0e1-d6b8-47df-b986-6f18f00766a8.png)

Circuit Diagram: (Refer Proteus)

![image](https://user-images.githubusercontent.com/69978515/129463736-326fb703-acbe-4c9c-b559-a6314fee432e.png)

Prog ISP:
Directly uploading your Assembly language code to the 8051 board might not work. The development board used here does not support USB Protocol. Instead we use the USB ISP Programmer that comes along with the kit, to upload our code.
- Debug and Run your assembly language code, and generate a hex file.
- Now, open the Prog ISP Software and upload the hex file there. Follow the intructions and initialize the software for your board.
- Now, you can upload the hex file for your code on to the 8051 board.
