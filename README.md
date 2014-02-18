zc706-ddr3-sodimm-dma
=====================

Example project that uses the AXI DMA peripheral to connect a custom
AXI-Stream peripheral to the DDR3 SODIMM memory on the ZC706 board

### Description

This XPS project provides the processor and peripherals access to the 1GB
DDR3 SODIMM memory via the Xilinx "AXI 7 Series Memory Controller" IP core.
The SDK project included is a simple application that writes to the memory
and commands a DMA transfer of that data to a custom AXI-Streaming core that
contains a simple loopback FIFO. The application commands a DMA transfer
from the custom peripheral back to the memory, and then verifies the data.

A key feature of this design is the use of an interconnect to drive a slave
(the DDR3 SODIMM memory) using two masters (the processor and the DMA engine).

### Requirements

* ISE Design Suite 14.7
* ZC706 Evaluation Board

### License

Feel free to modify the project or use it as a base for your application.

### Fork and share

If you port this project to another hardware platform, please send me the
code or push it onto GitHub and send me the link so I can post it on my
website. The more people that benefit, the better.

### About the author

I'm an FPGA consultant and I provide FPGA design services and training to
innovative companies around the world. I believe in sharing knowledge and
I regularly contribute to the open source community.

Jeff Johnson

http://www.fpgadeveloper.com