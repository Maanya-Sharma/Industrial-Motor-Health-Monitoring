# Industrial Motor Health Monitoring System

An embedded system designed to monitor industrial motor health by measuring
vibration, temperature, and current, with fault detection and RS-485 (Modbus RTU)
communication.

## Features
- Vibration monitoring using ADXL345
- Temperature and current sensing
- Fault detection (overcurrent, overheating, abnormal vibration)
- RS-485 communication using Modbus RTU
- Local non-volatile data logging using FRAM
- Designed for industrial 24V environments

## Hardware
- MCU: STM32F103C8
- Vibration Sensor: ADXL345 (SPI)
- Current Sensor: MCS1823
- Communication: MAX485 (RS-485)
- Memory: FM24C64 (FRAM)
- Power: 24V → 5V Buck → 3.3V LDO

## Communication
- Protocol: Modbus RTU
- Interface: RS-485
- Baudrate: 9600 / 19200

## Modbus Register Map 
Register	Description
40001	Temperature (°C ×10)
40002	RMS Vibration
40003	Motor Current (A ×100)
40010	Fault Status
40020	System Health

## Applications
- Predictive maintenance
- Industrial motor monitoring
- Condition-based monitoring systems

## Author
Developed as an industrial embedded systems project.
