# Embedded C Programming Examples with Continuous Integration and Code Quality

# embedded_systems_project

## Heat Control System 

### Theory

The heat control system is basically used to control the temperature inside a car. Whenever the user or driver gets seated inside the car, the button sensor gets activated. After that, the user gets access to turn on the heater. The temperature sensor monitors the temperature and sends the analog value to the microcontroller. The microcontroller processes the analog input of the temperature sensor and outputs a temperature value through serial communication. All the activities of the control system are performed on the microcontroller, ***Atmega328***.

### Simulation

The operation of the heat control system is coded in embedded c and the working is demonstrated using a simuation software called ***SimulIDE***.
Below shown two images where in the 1st image shows the status of the simulation when the system is OFF and the second image shows the status of the system when it is ON. 

#### ON
![ON](https://github.com/259881/Embedded-sys/blob/dd9619d0bf5ec8510b388c13f65093cd88ac2d20/Simulation/Simulation_fnal.gif)
-----------------------------------------------------------------------------------------------------------------------------------
#### OFF
![OFF](https://github.com/259881/Embedded-sys/blob/63daabfd34aad10d20fc0353ba36f3eed21d5bf3/Simulation/Simulation_OFF.png)

#### Outputs

|Circuit|RAM Table|
|:--:|:--:|
|![circuit](https://github.com/259881/Embedded-sys/blob/883bd20604d7552dbffed5447cfd061bc1803b4e/Simulation/Circuit.gif)|![Ram Table](https://github.com/259881/Embedded-sys/blob/233f462244119af26820fa5c5072e353ab16a4ae/Simulation/RAM_table.gif)|
|CRO|Serial Monitor|
|![CRO](https://github.com/259881/Embedded-sys/blob/b0dabf3e9307da78662215f941f1645bfdfb131b/Simulation/Oscilloscope.gif)|![Monitor](https://github.com/259881/Embedded-sys/blob/b0dabf3e9307da78662215f941f1645bfdfb131b/Simulation/Serial_Monitor.gif)|

### Function

* When the two switches are closed, the first LED glows indicating the actuation of the system and the heater.
* Next the analog input from the temperature sensor is received and digitized using ADC.
* The digitized temperature input is visualized using Pulse Width Modulation.
* The corresponding temperature values based on the digitized temperature input is transmitted by the UART protocol. Here the data is displayed on the serial monitor.

# LED Blinking 

## In Action

|ON|OFF|
|:--:|:--:|
|![ON](https://github.com/259881/Embedded-sys/blob/72dab35fbaa4344b5949eac735ad7130e6bf8596/Simulation/simulationON.png)|![OFF](https://github.com/259881/Embedded-sys/blob/a4fb835a0c452559859f0a83f764e4b510c4afe2/Simulation/simulationOFF.png)|

--------------------------------------------------------------------------------------------------------------------------------------------
## Activity_1
![Act1](https://github.com/259881/Embedded-sys/blob/84b68e77defa034239c5a0d180628e742bfaf1cc/Simulation/Activity_1.png)
---------------------------------------------------------------------------------------------------------------------------------------------
## Activity_2
--------------------------------------------------------------------------------------------------------------------------------------------
## Activity_3
----------------------------------------------------------------------------------------------------------------------------------------------
## Activity_4
---------------------------------------------------------------------------------------------------------------------------------------------

#### CI and Code Quality

|Build|Cppcheck|Codacy|
|:--:|:--:|:--:|
|[![Compile-Linux](https://github.com/Bharathgopal/Emb-C/actions/workflows/Compile.yml/badge.svg)](https://github.com/Bharathgopal/Emb-C/actions/workflows/Compile.yml)|[![Cppcheck](https://github.com/Bharathgopal/Emb-C/actions/workflows/CodeQulaity.yml/badge.svg)](https://github.com/Bharathgopal/Emb-C/actions/workflows/CodeQulaity.yml)|[![Codacy Badge](https://app.codacy.com/project/badge/Grade/643b7ca2b2dc4daba1e700c216bb87d9)](https://www.codacy.com/gh/Bharathgopal/Emb-C/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Bharathgopal/Emb-C&amp;utm_campaign=Badge_Grade)|
