# Blinky example (for nrf5340DK) with a defined nrf GPIO Pre-processor

I tried to change main.c by adding preprocessor #include <hal/nrf_gpio.h>. So that the functionality of GPIOS can be tested and they can easily configured manually.

## Definition for Pins

#define Gpio_pin  NRF_GPIO_PIN_MAP(0,31) with this command the pins are to be defined.

## main (void)

In the main Program the output configuration for that pin must be present there otherwise the code is not going to work properly.

## whileloop of main (void)
After defining the parameters, the whileloop must be configured, because we want to see the blinking led on the development kit (nrf5340). The code can be seen in repo.


