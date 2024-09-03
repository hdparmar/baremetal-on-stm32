# baremetal-on-stm32
This repository will focus on programming STM32 devices by bare metal programming

I am using the Nucleo Board STM32L467RG, it is based on Coretx M4 and is very versetile. 
It is also used on STM32 SensorTile.

This bare metal programming guide is made in a way to explain developers who want to learn how to program a board purely through low level hardware access using a high level programming language, C. This guide is focued on STM32L476RG but can be used to learn and program any board. Once we have understanding of the MCU, it's datasheet, user and reference manual. 

First, we will start off by learning the layout of MCU and the memeory address map and then we will start with the classic blinky project, and then move on further from there. Initially, we won't use the HAL (Hardware Absraction Library) but then we will realise that how it is useful after learning some bare-metal without HAL. 

LED Toggle - Address of the User LED which is LED2 at Port A Pin 5: Giving us PA5

The peripherals starts at 0x40000000

And the Port A is clocked by AHB2 Bus with boundary address of 0x4800 0000 (Starting address) - 0x4800 03FF (Ending Address)
With 1 KB Size (bytes) termed as GPIOA

Difference between AHP & APB

APB: Advanced Peripheral Bus 

AHP: Advanced High Performance Bus

AHB is faster than APB, with AHB bus you can access a particular peripheral with less clock cycle. For our example GPIOA is connected to AHB2 Bus at 80 Hz
