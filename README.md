# baremetal-on-stm32
This repository will focus on programming STM32 devices by bare metal programming

I am using the Nucleo Board STM32L467RG, it is based on Coretx M4 and is very versetile. 
It is also used on STM32 SensorTile.

This bare metal programming guide is made in a way to explain developers who want to learn how to program a board purely through low level hardware access using a high level programming language, C. This guide is focued on STM32L476RG but can be used to learn and program any board. Once we have understanding of the MCU, it's datasheet, user and reference manual. 

First, we will start off by learning the layout of MCU and the memeory address map and then we will start with the classic blinky project, and then move on further from there. Initially, we won't use the HAL (Hardware Absraction Library) but then we will realise that how it is useful after learning some bare-metal without HAL. 
