# SPI-MATLAB-thermocouple
Simulink Model for reading temperature from k-Type thermocouple using SPI device (MAX6675)

## Description
This simulink model reads temperature from k-Type thermocouple using SPI device (MAX6675).
CS pin is set low to start the conversion process in MAX6675. SPI block initiate the clock cycle. Upon falling pulse data is read as MSB and LSB. Pulse generator is used for continuous conversion and ultimately reading temperature.
The bits are then merge together and shift right 3 bits to read only temperature signal D14 to D03. Multiplied by offset to get temperature in centigrade.

## Requirements
1. MATLAB & Simulink Hardware Support Packages for Arduino
2. Arduino UNO
3. MAX6675
4. k-Type thermocouple

## Thank Note
Really appreciate the MATLAB's answers which supported a lot in getting this done.
