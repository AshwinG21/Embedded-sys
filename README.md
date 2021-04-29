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

#### OFF
![OFF](https://github.com/259881/Embedded-sys/blob/63daabfd34aad10d20fc0353ba36f3eed21d5bf3/Simulation/Simulation_OFF.png)

#### Outputs

|Circuit|RAM Table|
|:--:|:--:|
|![CIRCUIT](https://github.com/hemanthasapu/embedded_systems_project_256889/blob/main/simulation/Circuit.gif)|![RAM_TABLE](https://github.com/hemanthasapu/embedded_systems_project_256889/blob/main/simulation/RAM_table.gif)|
|CRO|Serial Monitor|
|![CRO](https://github.com/hemanthasapu/embedded_systems_project_256889/blob/main/simulation/Oscilloscope.gif)|![ON](https://github.com/hemanthasapu/embedded_systems_project_256889/blob/main/simulation/Serial_Monitor.gif)|

### Functionality 

* When the two switches are closed, the first LED glows indicating the actuation of the system and the heater.
* Next the analog input from the temperature sensor is received and digitized using ADC.
* The digitized temperature input is visualized using Pulse Width Modulation.
* The corresponding temperature values based on the digitized temperature input is transmitted by the UART protocol. Here the data is displayed on the serial monitor.

### CI and Code Quality

|Build|Cppcheck|Codacy|
|:--:|:--:|:--:|
|[![Compile-Linux](https://github.com/hemanthasapu/embedded_systems_project_256889/actions/workflows/Compile.yml/badge.svg)](https://github.com/hemanthasapu/embedded_systems_project_256889/actions/workflows/Compile.yml)|[![Cppcheck](https://github.com/hemanthasapu/embedded_systems_project_256889/actions/workflows/CodeQuality.yml/badge.svg)](https://github.com/hemanthasapu/embedded_systems_project_256889/actions/workflows/CodeQuality.yml)|[![Codacy Badge](https://app.codacy.com/project/badge/Grade/bf425986b42541fd92f2459de6359d9b)](https://www.codacy.com/gh/hemanthasapu/embedded_systems_project_256889/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=hemanthasapu/embedded_systems_project_256889&amp;utm_campaign=Badge_Grade)|

# LED Blinking 

## In Action

|ON|OFF|
|:--:|:--:|
|![ON](https://github.com/259881/Embedded-sys/blob/72dab35fbaa4344b5949eac735ad7130e6bf8596/Simulation/simulationON.png)|![OFF](https://github.com/259881/Embedded-sys/blob/a4fb835a0c452559859f0a83f764e4b510c4afe2/Simulation/simulationOFF.png)|

#### CI and Code Quality

|Build|Cppcheck|Codacy|
|:--:|:--:|:--:|
|[![Compile-Linux](https://github.com/Bharathgopal/Emb-C/actions/workflows/Compile.yml/badge.svg)](https://github.com/Bharathgopal/Emb-C/actions/workflows/Compile.yml)|[![Cppcheck](https://github.com/Bharathgopal/Emb-C/actions/workflows/CodeQulaity.yml/badge.svg)](https://github.com/Bharathgopal/Emb-C/actions/workflows/CodeQulaity.yml)|[![Codacy Badge](https://app.codacy.com/project/badge/Grade/643b7ca2b2dc4daba1e700c216bb87d9)](https://www.codacy.com/gh/Bharathgopal/Emb-C/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Bharathgopal/Emb-C&amp;utm_campaign=Badge_Grade)|
