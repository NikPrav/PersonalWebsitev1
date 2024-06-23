DNNWeaver is a framework written to optimise hardware to run a given DNN model, and has optimisations for convolutions
- The framework first optimizer the hardware according to the specs of the FPGA
- It then converts the given compute graph through methods such as tiling to instructions
- The instructions are then written onto the FPGA via DMA, and a register is written onto which signifies that the FPGA should start executing
- Once the FPGA finishes execution, the data is then read back from the FPGA

# Questions
- What are the FPGA-specific optimizations carried out by DNNWeaver?
- What is the target ISA?

# Program Flow
- Compiler object is created
- compile is called
	- passes an acc_obj that has details about the fpga
		- M, N, freq, mem_if_width, prec
	- macro node array is created after combining graph ops
	- Distinguishes between systolic array operations and PU operations
		- How does VEGETA deal with PU operations?
			- Has activation functions
	- Pads the arrays appropriately
	- Optimises tiling for conv layer
		- creates a varialbe optimal iling, which has a lot of parameters(B/b, )
	- 
- 