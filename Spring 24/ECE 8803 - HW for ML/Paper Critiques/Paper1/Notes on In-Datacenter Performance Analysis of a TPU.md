# Summary
## Abstract
Evaluation of a custom ASIC called a TPU on datacenter applications. Comparison is made to Intel Haswell CPU and Nvidia K80 GPU deployed across similar datacenters. Workloads wrtitten in TensorFlow framework involves production NN applications(MLPs, CNNs, LSTMs). The paper is able to show that the TPU is 15X to 30X faster than its contemporaries, with TOPS/Watt about 30x - 80X higher, ==even with low utilisation for some applications.== Recommends using GPU memory(GDDR5) to triple the achieved TOPS
## Introduction to NNs
- phases of an NN - training and inference
- quantization and energy/area gains
- batching
- focus of the paper (backbone of the paper)
	- Inference emphasizes response-time over throughput
	- GPU only marginally faster due to latency limits, even though more competent hardware
	- CNNs are just 5% of the workload
	- TPU 15x to 30x  faster than K80 GPU and CPU
	- Improving TPU memory will multiply the performance gains 
	- Can do more MACs than GPU
	- performance/watt of TPU is 30X to 80X
## TPU Origin, Architecture, Implementation and Software
Development focused on DNNs
Designed to be a coprocessor on the PCIe I/O bus, similar to an FPU
- Contains 256x256 MACs that can perform 8-bit multiply and add
Mix of 8-bit weights and 16-bit activations causes it to compute at half speed, while both becoming 16-bits causes the compute to be quarter speed
Weigths re staged through an op-chip Weight-FIFO that reads from an off-chip 8GiB DRAM(weight memory)

==Sparse architectural support is omitted==


## CPU, GPU and TPU Platforms
## Performance: Rooflines, Response-Time and Throughput
It is assumed that the models do not fit in the on-chip caches, leading them to be either computation limited or memory bandwidth limited. It is shown that there is a large margin for optimization through performance tuning without modifying operational intensity. 

## Energy Proportionality
## Evaluation of Alternative TPU designs
## Discussion

# Strengths
# Weaknesses
# Possible Improvements