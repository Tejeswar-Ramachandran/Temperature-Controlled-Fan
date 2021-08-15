# Temperature-Controlled-Fan

- In this project, I have implemented a Temperature Regulation system using 8051 Microcontroller in Assembly Language. 
- This project aims to regulate the speed or switch off the fan based on the surrounding temperature which is measured using a temperature sensor. 
- The analog values obtained are then passed through an ADC converting it to digital, which then parses it to the Microcontroller for calculations. Based on the temperature, it decides the speed of the fan and displays the necessary information. 
- We regulate the voltage the fan receives based on the temperature of the surroundings, if it is greater than 35°C, the fan runs at max speed, when it is between 25°C and 35°C at medium speed and turns off when the temperature is below 25°C.

NOTE: I couldn't obtain a plastic fan for the basic hardware demo, so instead I used a wheel as a substitute for a fan

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

Outputs:

NOTE: I couldn't obtain a plastic fan for the basic hardware demo, so instead I used a wheel as a substitute for a fan

- Temperature > 35C (Rotation of wheel not visible in images)

![image](https://user-images.githubusercontent.com/69978515/129463782-37a54dc1-d5b9-4f23-a26f-e547b8a4cae7.png)

- 25C < Temperature < 35C (Rotation of wheel not visible in images)

![image](https://user-images.githubusercontent.com/69978515/129463783-fc407931-8da2-4a5b-9e4c-083029ca50c9.png)

- Temperature < 25C (Rotation of wheel not visible in images)

![image](https://user-images.githubusercontent.com/69978515/129463785-546878df-3d8d-4ff5-a817-fc842727dfeb.png)

