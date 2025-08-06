.. _waveshare_nrf51_unknown:

Waveshare Unknown nRF51 Board
############################

Overview
********

The Waveshare Unknown nRF51 Board is a development board based on the Nordic nRF51822
microcontroller. This board is designed for Bluetooth Low Energy (BLE) development
and general embedded applications.

Hardware
********

Features
========

- **SoC**: nRF51822 (QFAC package)
- **CPU**: ARM Cortex-M0 32-bit processor
- **Flash**: 256 KB
- **RAM**: 32 KB
- **GPIO**: 31 pins
- **UART**: 1 (UART0)
- **SPI**: 1 (SPI1)
- **I2C**: 1 (I2C0)
- **LEDs**: 5 (GPIO 18-22)
- **Buttons**: 2 (GPIO 16-17)

Supported Features
=================

- Bluetooth Low Energy (BLE)
- GPIO control
- I2C communication
- SPI communication
- UART communication

Pin Mapping
===========

LEDs
----

- LED0: GPIO 18
- LED1: GPIO 19
- LED2: GPIO 20
- LED3: GPIO 21
- LED4: GPIO 22

Buttons
-------

- Button0: GPIO 16 (with pull-up, active low)
- Button1: GPIO 17 (with pull-up, active low)

UART
----

- TX: GPIO 9
- RX: GPIO 11
- RTS: GPIO 8
- CTS: GPIO 10

I2C
---

- SDA: GPIO 0
- SCL: GPIO 1

SPI
---

- SCK: GPIO 25
- MOSI: GPIO 24
- MISO: GPIO 23
- CS: GPIO 30

Programming and Debugging
*************************

The board supports programming and debugging through:

- J-Link
- nRF5x Command Line Tools
- nRF Util

Default Configuration
********************

The board comes with the following default configuration:

- UART console enabled
- GPIO enabled
- Serial driver enabled
- Console enabled

Getting Started
**************

1. Connect the board to your development machine
2. Build and flash your application using Zephyr RTOS
3. Use the UART console for debugging and interaction

Example Build Command
====================

.. code-block:: console

   west build -b nrf51_unknown samples/basic/blinky

Example Flash Command
====================

.. code-block:: console

   west flash

References
**********

- `nRF51822 Product Specification <https://www.nordicsemi.com/Products/nRF51822>`_
- `Zephyr RTOS Documentation <https://docs.zephyrproject.org/>`_ 