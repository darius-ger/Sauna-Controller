# ESP32 DevKit-C Pinout and Recommended Usage

| Pin  | GPIO | Recommended Usage                 | Notes                                                                |
|------|------|-----------------------------------|----------------------------------------------------------------------|
| VIN  | -    | Power Input (5V)                  | Connect to 5V power source                                           |
| GND  | -    | Ground                            | Common ground                                                        |
| 3V3  | -    | 3.3V Power Output                 | Provides 3.3V output from onboard regulator                          |
| EN   | -    | Enable Pin                        | Pull high to enable the chip                                         |
| IO0  | GPIO0| Boot Mode / General Purpose I/O   | Must be pulled low to enter boot mode                                |
| IO1  | GPIO1| UART TX                           | Used for serial communication                                        |
| IO2  | GPIO2| General Purpose I/O               | Can be used for output or input                                      |
| IO3  | GPIO3| UART RX                           | Used for serial communication                                        |
| IO4  | GPIO4| General Purpose I/O               | Suitable for PWM, I2C, or other digital functions                    |
| IO5  | GPIO5| General Purpose I/O               | Often used for SPI or digital output                                 |
| IO12 | GPIO12| General Purpose I/O              | Must float during boot; avoid using for pull-up/down configurations  |
| IO13 | GPIO13| General Purpose I/O              | Suitable for PWM or digital input/output                             |
| IO14 | GPIO14| General Purpose I/O              | Often used for SPI or digital output                                 |
| IO15 | GPIO15| General Purpose I/O              | Must float during boot; avoid using for pull-up/down configurations  |
| IO16 | GPIO16| General Purpose I/O              | Can be used for digital input/output                                 |
| IO17 | GPIO17| General Purpose I/O              | Can be used for digital input/output                                 |
| IO18 | GPIO18| SPI CLK                          | Default SPI clock pin                                                |
| IO19 | GPIO19| SPI MISO                         | Default SPI MISO pin                                                 |
| IO21 | GPIO21| I2C SDA                          | Default I2C data pin                                                 |
| IO22 | GPIO22| I2C SCL                          | Default I2C clock pin                                                |
| IO23 | GPIO23| SPI MOSI                         | Default SPI MOSI pin                                                 |
| IO25 | GPIO25| ADC / DAC                        | Can be used as analog input or DAC output                            |
| IO26 | GPIO26| ADC / DAC                        | Can be used as analog input or DAC output                            |
| IO27 | GPIO27| ADC                              | Can be used as analog input                                          |
| IO32 | GPIO32| ADC                              | Can be used as analog input                                          |
| IO33 | GPIO33| ADC                              | Can be used as analog input                                          |
| IO34 | GPIO34| ADC (Input Only)                 | Analog input only                                                    |
| IO35 | GPIO35| ADC (Input Only)                 | Analog input only                                                    |
| IO36 | GPIO36| ADC (Input Only)                 | Analog input only                                                    |
| IO39 | GPIO39| ADC (Input Only)                 | Analog input only                                                    |

# Notes on Pin Usage

- **Power Pins**: Use `VIN` for 5V input and `3V3` for 3.3V output.
- **Boot Mode**: GPIO0 must be pulled low to enter boot mode.
- **Analog Pins**: GPIOs 32-39 are ADC pins, with GPIOs 34-39 being input-only.
- **SPI Pins**: GPIOs 18, 19, and 23 are default SPI pins.
- **I2C Pins**: GPIOs 21 and 22 are default I2C pins.
- **UART Pins**: GPIOs 1 (TX) and 3 (RX) are default UART pins.
- **GPIO12 and GPIO15**: Avoid using these pins for pull-up or pull-down configurations as they affect the boot process.

This table provides a clear overview of the ESP32 DevKit-C pins and their recommended usage. Adjust the pin assignments based on your specific project requirements.
