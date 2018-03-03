# PolarFire Evaluation Kit RISC-V Designs
Sample Mi-V Libero project(s) for the PolarFire (MPF300T) Evaluation Kit.

This project contains a Libero project containing an FPGA design including a Mi-V soft processor. 

### Design Features
The FPGA designs include the following features:
* Uses MIV_RV32IMA_L1_AHB processor
* RISC-V debug block allowing on-target debug using openocd/GDB
* LSRAM for code/data
* User peripherals such as GPIO, Timers, UART

The memory map for each design is available within each Libero project.

### Libero Projects
* PF_MIV_RV32IMA_L1_AHB_BaseDesign:
      Uses MIV_RV32IMA_L1_AHB soft processor. Allows software debugging using FlashPro5. The same JTAG port is used for programming the FPGA and debugging RISC-V software.
* PF_CoreRISCV_AXI4_BaseDesign:
      Uses legacy CoreRISCV_AXI4 soft processor. Allows software debugging using FlashPro5. The same JTAG port is used for programming the FPGA and debugging RISC-V software.
* PF_CoreRISCV_AXI4_CoreBootStrap:
      Uses legacy CoreRISCV_AXI4 soft processor. Allows software debugging using FlashPro5. This also allows for booting from SPI Flash.The same JTAG port is used for programming the FPGA and debugging RISC-V software.

### Target Mi-V CPU
Details of the features of Mi-V CPUs are available [here](https://github.com/Mi-V-Ecosystem/Mi-V-CPUs).

### Target Hardware
Details of the features of PolarFire Evaluation kit are available [here](https://www.microsemi.com/products/fpga-soc/design-resources/dev-kits/polarfire/polarfire-eval-kit).

