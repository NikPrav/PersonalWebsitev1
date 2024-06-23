Experimenting training a GPT-like model over single and multiple GPUs with various types of parallelism. Uses megatron-LM for generation of distributed runs.

# Single GPU Training
Uses a YAML file `single_gpu.yaml` to train the model for 1 epoch

# Multiple GPU Training
Generate YAML files for the following configs
- Tensor Parallelism
- Pipeline Parallelism
- Data Parallelism
- Tensor Parallelism + Activation Recomputation
- Pipeline Parallelism + Activation Recomputation
- Data Parallelism + Activation Recomputation