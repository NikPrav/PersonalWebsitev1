https://colorlesscube.com/uvm-guide-for-beginners/
[The Textbook](https://dl.acm.org/doi/pdf/10.5555/2843495)
1) Verification as a part of the pipeline
2) The Verification Flow
3) Fundamentals of Sim-Based Verification
4) The Verification plan
5) Simulation Engines
6) Creating Environments for Verification
7) Strategies for Sim-Based Stimulus Generation
8) Result-checking strategies for Sim-Based Verification
9) Pervasive Function Verification
10) System Simulation
11) Formal Verification
# Why Verification
As Digital Systems become more complex, verification methodologies get more essential as
- making changes to post-silicon hardware is insanely expensive as compared to pre-silicon
- verification is essentially modelling hardware through code
# How Verification
[[UVM]] methodology simplifies the process of automating test vectors, along with very modular code that can be transferred across projects and ips.

Formal Verification uses mathematical models and induction to "prove" that a given DUT adheres to specifications. These specifications are defined through the use of SystemVerilog Assertions and the testing environment is constrained through SystemVerilog Assumptions

I have been exploring how to automate SystemVerilog Assertions through the use of LLMs, mostly via prompting existing LLMs. My gut feeling is that prompting is not the best way of going about this, there must be better ways of training LLMs to generate more robust and reliable code


