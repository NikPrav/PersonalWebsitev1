# Tentative Plan
Run Python Code for a DNN on an FPGA

# Goals 
- Convert DNN to intermediate representation:[[Python to Intermediate Representation]]
- Communicate with the FPGA using ISA: [[Communication Protocol with the FPGA]]
	- Dataflow - Can the data be transferred from the Machine to the FPGA? Or does the data have to be on the FPGA locally
	- FPGA should act as an accelerator, akin to GPU
- Make the physical connection to the FPGA for communication
or
- Make specialized accelerator for DNN
	- Use templates for synthesis?

# Steps
Using DNNWeaver as the backbone
- Compile graph model into ISA using a Compiler
- Write instructions and data to FPGA memory via DMA
- Execute on FPGA
- Read back data from FPGA


[[DNNWeaver - Overview]]
[[Project Plan]]