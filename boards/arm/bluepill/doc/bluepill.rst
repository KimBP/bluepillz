.. _bluepill_stm32f103_board:

ST BLUEPILL BOARD
#################

Overview
********
See `bluepill wiki`_ for information


Hardware
********

Supported Features
==================

The Zephyr bluepill board configuration supports the following hardware features:

+-----------+------------+-------------------------------------+
| Interface | Controller | Driver/Component                    |
+===========+============+=====================================+
| NVIC      | on-chip    | nested vector interrupt controller  |
+-----------+------------+-------------------------------------+
| UART      | on-chip    | serial port-polling;                |
|           |            | serial port-interrupt               |
+-----------+------------+-------------------------------------+
| PINMUX    | on-chip    | pinmux                              |
+-----------+------------+-------------------------------------+
| GPIO      | on-chip    | gpio                                |
+-----------+------------+-------------------------------------+
| CLOCK     | on-chip    | reset and clock control             |
+-----------+------------+-------------------------------------+
| FLASH     | on-chip    | flash memory                        |
+-----------+------------+-------------------------------------+
| IWDG      | on-chip    | independent watchdog                |
+-----------+------------+-------------------------------------+

Other hardware features are not yet supported in this Zephyr port.

The default configuration can be found in the defconfig file:
``boards/arm/bluepill/bluepill_defconfig``

Connections and IOs
===================

Each of the GPIO pins can be configured by software as output (push-pull or open-drain), as
input (with or without pull-up or pull-down), or as peripheral alternate function. Most of the
GPIO pins are shared with digital or analog alternate functions. All GPIOs are high current
capable except for analog inputs.

Board connectors:
-----------------
XXX TO come

Default Zephyr Peripheral Mapping:
----------------------------------

XXXXX To be changed


- UART_1_TX : PA9
- UART_1_RX : PA10
- UART_2_TX : PA2
- UART_2_RX : PA3

For mode details please refer to `STM32 Nucleo-64 board User Manual`_.



References
**********

.. target-notes::

.. _bluepill wiki:
   https://wiki.stm32duino.com/index.php?title=Blue_Pill

.. _STM32F103 reference manual:
   http://www.st.com/resource/en/reference_manual/cd00171190.pdf

.. _STM32F103 data sheet:
   http://www.st.com/resource/en/datasheet/stm32f103rb.pdf

