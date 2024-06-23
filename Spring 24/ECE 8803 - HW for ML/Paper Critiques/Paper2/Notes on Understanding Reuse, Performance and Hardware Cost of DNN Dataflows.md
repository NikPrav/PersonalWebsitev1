# Abstract
The paper looks at data partitioning and schedule strategies employed by DNN accelerators, which directly impacts the performance and the energy efficiency. The impact of the choice of dataflows on the utilisaton and efficiency, along with the tools and methodologies used to help architects explore the design space is explored. 

A set of data-centric directives are introduced to concisely specify the dataflow space. These are then analysed for optimisation through hardware capabilities. An analytical cost model, called MAESTRO is codified that can estimate the various cost-benefit tradeoffs of a dataflow including execution time and energy efficiency. 
# Introduction
 Data reuse depends on how the computations are scheduled, and how they are mapped across PEs. The cost of computation is exceeded by the energy cost of moving data. It also depends on the target DNN model and its layer types/dimenstions, the dataflow and the available hardware resources and connectivity. 

The paper proposes a data-centric approach towards acceleration, as opposed to compute-centric approach followed before. It also shows how these directives can be used to optimise for data reuse better. This is used to define MAESTRO that takes in as input 
- a DNN model with a set of layers
- a dataflow description for each layer
- a hardware configuration
Maestro estimates the end-to-end execution time, energy, NoC costs and so on.
MAESTRO cost model can also be used to determine optimal params with given area, energy, or throughput budget.
# Background
## Tensors in DNN
Focuses on CONV2D. ==Are sparse matrices included in the compute costs?== ==What about transformers with a lot of sparse matrices?==
Supports a wide array of interconnects between PEs and shared L2 buffer.
# Describing Dataflows
4 key directives
- spatial
- temporal
- data movement order
- clusters

# Quantitative Dataflow Analysis
# Case Studies
# Future Work
* Co-optimising DNN accelerator micro architecture and its internal data flow is crucial for designers to achieve both higher performance and energy efficiency
* Data-centric directives are introduced to specify DNN dataflows, along with an analytical model to estimate execution time, energy efficiency and hw cost.


# Strengths
- Data centric flow helps in visualisation of the biggest bottleneck in accelerating LLMs - memory bandwidth, and helps in working around through smart usage of better L1 memory for data reuse through PE to PE interconnects
- Allows for effective design space exploration, highlighting design preferences according to layers which varies dramatically
# Weaknesses
* cannot model content of datacells apart from simpler methods; i.e. in case of transformers, wherein sparse layers are common, there might be a lot of compute involving zeros which are wasted compute that can be skipped
* performs comparison of dataflows, does not take into actual designs which may have custom blocks
* 
# Improvements

