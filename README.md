# FireAlarmDetectionSTM32

The purpose of this project is to design and develop a smart fire alarm system that practices the Digital Signal Processing technology. This repository records the step by step to create the project using the STM32Cube IDE. The overall code of the project will be compile and build into STM32 microcontroller. 

# Software
The software used in this project listed as below: 

1)	[STM32CubeIDE](https://www.st.com/en/development-tools/stm32cubeide.html#get-software)
2)	[STM32CubeMX](https://www.st.com/en/development-tools/stm32cubemx.html#get-software)

# Hardware
The hardware used in this project listed as below: 

1)	STM32F44RE MCU
2)	DHT11 Temperature Sensor
3)	Active Buzzer Module
4)	LCD1602 Serial IIC I2C
5)	LED

# Setup Project

The new project is created by using STM32Cube IDE. At the early setup page, STM32F446RE board is chosen for this project.

![step1](https://github.com/amiruliman/FireAlarmDetectionSTM32/blob/main/Images/step1.png)

Another pop-up configuration will appear to setup the option for this project. C language will be selected as the targeted language and let the other option set as default settings. 

![step2](https://github.com/amiruliman/FireAlarmDetectionSTM32/blob/main/Images/step2.png)

1) Set GPIO pin for LED, temperature sensor and buzzer

![step3](https://github.com/amiruliman/FireAlarmDetectionSTM32/blob/main/Images/step3.png)

2) Enable external crystal for the clock 

![step4](https://github.com/amiruliman/FireAlarmDetectionSTM32/blob/main/Images/step4.png)

3) Enable timer for setting the delay for microsecond

![step5](https://github.com/amiruliman/FireAlarmDetectionSTM32/blob/main/Images/step5.png)

4) Enable I2C1 for LCD 1602 I2C Module 

![step6](https://github.com/amiruliman/FireAlarmDetectionSTM32/blob/main/Images/step6.png)

5) To trigger the buzzer, need to produce PWM to create a square wave of low frequency by enabling the PWM generation in the timer mode.

![step7](https://github.com/amiruliman/FireAlarmDetectionSTM32/blob/main/Images/step6.png)

# Circuit Connection (Schematic)

Below is the connection for all the component needed.

![schematic](https://github.com/amiruliman/FireAlarmDetectionSTM32/blob/main/Images/schematic.png)

# Rerun this project on your side

To run this project, install the necessary software as mentioned above and follow the following steps:

1. Download the repository and unzip it in your workarea. 
2. Open **STM32CubeIDE** software
3. Select **File > Import** .
4. Under **General**, select **Existing Project into Workspace** and click **Next**. 
5. Browse the **FireAlarm_CMSIS** folder.
6. Enable **Copy projects to Workspace**.
