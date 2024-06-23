
# Goals - Compiler
- Compiling GEMM Instructions
	- Making the GEMM MacroNode
	- Padding
	- compiling
		- Tiling
		- Convert to instructions
- Compiling SPMM Instructions

# Tasks
- Compiling GEMM Instructions ![[Pasted image 20240405183519.png]]
	- Formalizing instructions to run GEMM
		- in VEGETA ISA
		- LD STR
		- ALU OP
		- pooling, activation
	- MacroNode Creation
	- Code up translator for VEGETA
		- Tiled MacroNode -> VEGETA ISA
	- Tiling for GEMM operations