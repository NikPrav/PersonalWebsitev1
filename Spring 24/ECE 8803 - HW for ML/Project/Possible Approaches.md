https://arxiv.org/pdf/1810.09773.pdf
https://educationecosystem.com/blog/fpga-programming-with-opencl/

# Points to Focus on
- Custom Accelerator Design - ISA design
- Accelerator Deployment - Custom RTL on FPGA
- Communication with the above accelerator - Send and Recieve Data b/w Host CPU and FPGA

# OpenCL
## Overview
- OpenCL is a device-agnostic alternative to the NVIDIA CUDA programming Language
- has a threading and a memory model
- reads like something akin to HLS, need to figure out how to use custom hardware with the same
- ==OpenCL is compiled offline into an FPGA bitstream, and then loaded at run-time by the host to reprogram the FPGA==![[Pasted image 20240326163737.png]]
	- each thread is a work-item, and multiple work-items are grouped to form a work-group
	- memory is classified into 4 types
		- Global - off-chip
		- Local - on-chip
		- Constant - off-chip read-only
		- Private - thread-specific memory on-chip
- Intel FPGA SDK exists, with all the necessary APIs and run-time programs and uses PCIe- attached, similar to a GPU

## Communication with OpenCL
- https://www.intel.com/content/www/us/en/docs/programmable/683846/22-4/implementing-the-channels-extension.html
- https://www.intel.com/content/www/us/en/support/programmable/support-resources/design-guidance/opencl-software-support.html

## Implementation - A simple Vector Add via OpenCL and Intel FPGA
https://educationecosystem.com/blog/fpga-programming-with-opencl/#:~:text=is%20also%20supported.-,Trying%20FPGA%20Programming,-Let%E2%80%99s%20explore%20the
- Intel FPGA SDK for OpenCL is used to emulate the code and verify functionality
- it is then built for the FPGA and the Host
- the program is then run


# VTA
## Overview
![[Pasted image 20240328114044.png]]
- Is it possible to replace the ISA and MicroArchitecture with our own custom accelerator - say, VEGETA?
- How is the reconfigurablity of an FPGA used? What if I just wanted to do this for a specific novel hw architecture?

## Architectural Implementation
https://tvm.apache.org/docs/topic/vta/dev/index.html
- ==VTA is written in HLS==
- ISA comprises of 4 CISC instructions
	- `LOAD` loads a 2D tensor from DRAM
	- `GEMM` performs a micro-op sequence of matrix-matrix multiplications
	- `ALU` performs a sequence of matrix-matrix ALU operations
	- `STORE` Stores a 2D tensor from the output buffer to DRAM
- Programmed via a linear instruction stream
	- r/w `control` register, w-only `insn_count` register, w-only `insns` register
	- CPU preps the instruction stream in DRAM into a buffer prepared by VTA runtime, and asserts the `control` register, ==which is then read from the DRAM via DMA==
- fetch module partially decodes the instrcutions, and pushes the instructions into command queues to feed into load, compute and store modules
- It is then pipelined according to `load-compute-store`

- VEGETA also has an instruction FIFO queue
- A possibility can be to use what VTA does, ==utilise DMA to read instructions and data==
	- How does DMA work

# Notes to self
- play around with fpgas more
- fpga linux environment - RTL connection
- what does the bitstream program - instructions for the hardware

