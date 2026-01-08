# STM32 Timer Triggered ADC with DMA and UART

## Description

This project demonstrates ADC data acquisition on STM32 using
hardware timer trigger, DMA for efficient data transfer, and
UART output for monitoring.

## Hardware

- STM32 Nucleo board (STM32F401)
- ADC Channel 1 (PA1)
- USART2 (Virtual COM Port)

## Software

- STM32CubeIDE
- HAL drivers
- Windows PowerShell for serial monitoring

## Working

- TIM2 generates periodic trigger (TRGO)
- ADC conversion starts on timer trigger
- DMA transfers ADC data to memory
- ADC conversion complete callback sends data via UART

## Output

ADC values are displayed on a serial terminal at 115200 baud.

## Result

Verified ADC output using PowerShell serial terminal.
