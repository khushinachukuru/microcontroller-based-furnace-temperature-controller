# microcontroller-based-furnace-temperature-controller
Project Overview
A furnace temperature controller is an essential device for industrial applications where precise temperature control is required. This project involves designing a microcontroller-based furnace temperature controller using an Arduino board, a temperature sensor (such as a thermocouple or a thermistor), a relay module, and a heater. The system continuously monitors the furnace temperature and adjusts the heating element accordingly to maintain a predefined temperature range.

Project Components
1. Hardware Requirements
Arduino Uno / Mega / Nano – Acts as the microcontroller to process data and control the heater.
Temperature Sensor (e.g., K-Type Thermocouple with MAX6675 module, DS18B20, or NTC Thermistor) – Measures furnace temperature.
Relay Module (5V or 12V, depending on heater power rating) – Switches the heater ON/OFF based on temperature readings.
Heater Element – Provides heat to the furnace.
Cooling Fan (optional) – Helps in cooling when temperature overshoots.
LCD Display (16x2 or OLED Display) – Shows real-time temperature readings and control status.
Push Buttons / Keypad – Used for setting the desired temperature.
Buzzer (optional) – Alerts when the temperature exceeds safe limits.
Power Supply (5V for Arduino, 12V or 230V for heater and relay module as needed).
2. Working Principle
The temperature sensor continuously reads the furnace temperature and sends data to the Arduino microcontroller.
The Arduino compares the measured temperature with the user-defined setpoint.
If the temperature is below the setpoint, the relay turns ON the heater.
If the temperature exceeds the setpoint, the relay turns OFF the heater.
An LCD/OLED display shows real-time temperature readings and system status.
A buzzer can be added to alert the user if the temperature exceeds a critical limit.
Circuit Diagram
The circuit consists of:

The temperature sensor connected to the Arduino via the appropriate interface (Analog/Digital/SPI).
The relay module connected to an Arduino digital output pin for heater control.
The LCD display connected via I2C or parallel interface to display temperature readings.
Push buttons to set the desired temperature.
