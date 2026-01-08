# STM32 Timer Triggered ADC with DMA and UART

## Description

This project demonstrates ADC data acquisition on an STM32 microcontroller
using a hardware timer trigger, DMA for efficient data transfer, and UART
for serial monitoring.

## Hardware Used

- STM32 Nucleo board (STM32F401)
- ADC Channel 1 (PA1)
- USART2 (Virtual COM Port via ST-Link)

## Software Used

- STM32CubeIDE
- HAL drivers
- Windows PowerShell for serial monitoring

## Working Principle

- TIM2 generates a periodic trigger (TRGO).
- ADC conversion starts on the timer trigger.
- DMA transfers the ADC data to memory automatically.
- ADC conversion complete callback sends the ADC value via UART.

## Output

ADC values are transmitted over UART at a baud rate of 115200 and can be
viewed on a PC serial terminal.

## Output Screenshot

![ADC UART Output](images/output.png)

## Result

The ADC values were successfully observed on the PC, confirming proper
operation of timer-triggered ADC with DMA and UART.
