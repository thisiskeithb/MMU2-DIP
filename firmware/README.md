# MMU2-DIP
Ported from [Prusa3D](https://github.com/prusa3d/MM-control-01)

MCU: STM32F0C8

Supports:
- TMC2208, TMC2209, TMC2130, and TMC5160 drivers from BigTreeTech,
- TMC stall protection (TMC2209, TMC2130, and TMC5160 only),
- Manual loading of filaments

# Modify configuration
Set the drive type, motor current, etc. in [`/MMU2/src/config.h`](MMU2/src/config.h)

# Building
To build this firmware, use [VSCode](https://code.visualstudio.com/download) with [PlatformIO](https://platformio.org/platformio-ide).

# Upgrade firmware in Windows
1. Install `firmware/Tool/cd340driver/CH341SER.EXE`.
2. Connect a usb cable
3. Open `firmware/Tool/flymcu/FlyMcu.exe`.

   ①. Refresh the port.

   ②. Select the corresponding port.

   ③. Set the baud rate.

   ④. Select the `firmware.hex` file.

   ⑤. Set download parameters.

   ⑥. Click "Start ISP(p)" to start downloading.

   ![image](https://github.com/bigtreetech/MMU2-DIP/blob/master/firmware/Tool/UpgrateFirmware.png)
