https://arxiv.org/pdf/2006.13829.pdf - https://github.com/ICIdsl/caffe_fpga
[[caffe_barista.pdf]]
- OpenCL can be used for the communication layer - ![[Pasted image 20240325142156.png]]
- A performance model is used to maximise exec time in hardware

# Things to look for
- Does it work with any caffe model?
	- has multiple caffe models
- Can the FPGA parameters be customised?
- What is the ISA of the design on the FPGA?
	- Custom ISA?
	- Function of OpenCL
	- 
- Can it be extended to other accelerators such as SIGMA?
- How does OCL work in communication?

# Caffe-Barista Paper
- Focuses on Training Cycle
- Integrates FPGAs into the training of CNNs
- Consists of three components
	- Software-integration layer that enables seamless integration of FPGA accelerator with caffe
	- FPGA-based h/w accelerator
	- OpenCL runtime that orchestrates the CNN execution b/w host CPU and FPGA
- ==FPGA device runs a kernel that is responsible for executing matrix multiplication==
- CPU executes all other operations, and ==coordinates offloading of computations to the FPGA==
## Execution Flow
- Caffe Flow for CONV Layers
	- Caffe selects platform to execute on
	- for each batch in each layer, caffe calls batch-level GEMM function
		- for forward pass, im2col is called, and converts them into matrices
		- for backward pass, the gradietns w.r.t weights are calculated by multiplying the inputs with the gradients w.r.t the output. THe gradents w.r.t input for each element in the batch is calculated through multiplying the weights with the gradient w.r.t output.
		- ==All these matrices are tiled, and fed into FPGA-GEMM Kernel==
		- im2col is not required for backprop
- Acclerator Architecture
	- Comprises of a ==parameterised== systolic array
	- overall dimensions of PE in the systolic array is configurable
- 
