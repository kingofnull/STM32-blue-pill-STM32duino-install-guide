# STM32 Blue Pill Stm32duino install guide
A guide to install Stm32duino bootloader and getting started with Arduino 

1) Add board manager url to Arduino : 
```
http://dan.drown.org/stm32duino/package_STM32duino_index.json
```

  Backup: [tools_win-2022.9.26.zip](tools_win-2022.9.26.zip) , [STM32F1-2022.9.26.zip](STM32F1-2022.9.26.zip)

2) Install STM32F1xx from Board Manager.

2) Download STLink Utilty:
[Download STM32 ST-LINK Utility v4.6.0.7z](STM32 ST-LINK Utility v4.6.0.7z)

3) Download bootloader: 
[Download generic_boot20_pc13.bin](generic_boot20_pc13.bin)

4) Flash bootloader using ST-LINK Utility. Open `generic_boot20_pc13.bin` and click `Erase` then `Program Verify`.

4) Connect board.

5) Download and install Maple windows drivers (serial and dfu) by running `install_drivers.bat`.(I dont know about linux drivers!)

[Download maple-drivers-win.7z](maple-drivers-win.7z)

6) In Arduino IDE set:
Board :     STM32F108C6/fake STM32F108C8
CPU Speed:  72Mhz
Port:       COM1 (maple)                --> Deffers by your pc setup


