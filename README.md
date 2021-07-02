# LogicCircuit-to-HDL-or-VHDL
A version of Eugene Lepekhin's LogicCircuit that translates LC projects to Nand2Tetris HDL or to structural VHDL

This repository contains a modified version of Eugene Lepekhin’s LogicCircuit program that generates the “.hdl” files expected by the Hardware Simulator that is part of the Nand2Tetris tool suite created and distributed by Noam Nisan, Shimon Schocken, Mark Armbrust, and their colleagues. For better compatibility with the Nand2Tetris software, you will need to install the additional builtInChips by copying the contents of the provided builtInChips directory to
 	<N2T_install_directory>\tools\builtInChips.

The HDL suite is also capable of generating structural VHDL suitable for use with FPGA design software such as the Xilinx Vivado Design Suite

I have successfully used the modified version of LogicCircuit to produce hdl design files for all hardware projects enumerated in the Chapters 1, 2, 3, and 5 of “The Elements of Computing Systems.” Using the modified LogicCircuit to complete the hardware assignments in the Nand2Tetris book, I have found the design methodology that uses LogicCircuit to complete the design, and the N2T Hardware Simulator and test scripts to validate that design, to be a powerful and intuitive combination. I hope and anticipate that this combination will help students learn the course underlying principles more readily than if they just used HDL to develop their circuit designs.

To install the modified version of LogicCircuit, first uninstall any existing versions, then double click on the installer. Then copy the added builtInChips as described above.
  
The “SaveAsHDL” feature has been tested reasonably thoroughly in the course of implementing all of the N2T book’s hardware projects. Others will no doubt encounter problems not yet identified.  If you do find a bug, please send the circuitproject file that demonstrates the problem, together with a short explanation of the problem, to jkb@colorado.edu. I will endeavor to address repeatable problems as they are identified.

The structural VHDL generated by this code is targeted to the Xilinx Vivado Synthesis Suite. I have used this code to successfully implement a VHDL version of the N2T CPU using this tool suite (implementing the full N2T Computer requires additional platform-specific code not included here). There are many issues related to the correct use of these tools with actual hardware that cannot be easily addressed within LogicCircuit.

