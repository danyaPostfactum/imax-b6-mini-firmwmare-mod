# Imax B6 Mini charger firmware modification project

The main goal is to improve the charger accuracy (voltage and current measuring) and to extend some voltage ranges (DC-IN thresholds, LiIo cut-off voltages).

# Some hardware information
The MCU is 8051-Based MegaWin MA84G564 (another name is MG84FG516).
In `hardware` dir you can find the MG84FG516 datasheet, the circuid diagram and the pcb photo (bottom).
The `dfu.jpg` explains how to force the MCU to DFU mode (this mode is used to flash via USB) if firwmare was damaged.

# Disassembling stock firmware (v1.19)
The stock firwmware bin file (named as `133`) is extracted from B6mini_Firmware_Update_V1.19 exe file (using 7zip).
The MCU description (ports, interrupts, memory areas) for IDA pro is located in `i51.cfg` file (you should add the file contents to your default `i51.cfg` file).
I have located some interesting parts of firmware (ADC related).

# Some useful links
- https://www.skyrc.com/iMAX_B6mini_Charger
- https://rcsearch.ru/wiki/IMAX_B6_Mini
- https://mysku.club/blog/aliexpress/32004.html
- https://radiokot.ru/forum/viewtopic.php?f=11&t=113631
- https://rcopen.com/forum/f88/topic409450