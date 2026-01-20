## Firmware Overview

The firmware is written using STM32 libraries.

### Modules
- adc.c – Reads temperature and current sensors
- spi_adxl345.c – Vibration sensor interface
- i2c_fram.c – FRAM read/write routines
- modbus_rtu.c – RS-485 Modbus communication
- fault_detection.c – Motor fault logic

