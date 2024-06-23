---
annotation-target: Paper Readings/23_01_Eyeriss.pdf
annotation-target-type: pdf
---


>%%
>```annotation-json
>{"text":"SIMD: Single-Instruction, Multiple Data. The same instruction is run on multiple PEs \nSIMT: Single-Instruction, Multiple Threads. SIMD combined with multiple threading. Used in GPUs. \n\nEach of the SIMT core might have different stack pointers, while SIMD cores are just part of an ALU that knows nothing about memory per se.\n\nIn case of a RAW(data) hazard, GPUs tend to switch threads over CPU methods such as branch prediction","target":[{"source":"vault:/Paper Readings/23_01_Eyeriss.pdf","selector":[{"type":"TextPositionSelector","start":595,"end":647},{"type":"TextQuoteSelector","exact":"highly-parallel compute paradigms, such as SIMD/SIMT","prefix":"mount of data movement. Although","suffix":", effec-tively address the compu"}]}],"created":"2024-01-23T15:54:12.145Z","updated":"2024-01-23T15:54:12.145Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf"}
>```
>%%
>*%%PREFIX%%mount of data movement. Although%%HIGHLIGHT%% ==highly-parallel compute paradigms, such as SIMD/SIMT== %%POSTFIX%%, effec-tively address the compu*
>%%LINK%%[[#^7nhwv3h19cv|show annotation]]
>%%COMMENT%%
>SIMD: Single-Instruction, Multiple Data. The same instruction is run on multiple PEs 
>SIMT: Single-Instruction, Multiple Threads. SIMD combined with multiple threading. Used in GPUs. 
>
>Each of the SIMT core might have different stack pointers, while SIMD cores are just part of an ALU that knows nothing about memory per se.
>
>In case of a RAW(data) hazard, GPUs tend to switch threads over CPU methods such as branch prediction
>%%TAGS%%
>#Defn
^7nhwv3h19cv


>%%
>```annotation-json
>{"created":"2024-01-23T15:54:48.840Z","updated":"2024-01-23T15:54:48.840Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf","target":[{"source":"vault:/Paper Readings/23_01_Eyeriss.pdf","selector":[{"type":"TextPositionSelector","start":1172,"end":1354},{"type":"TextQuoteSelector","exact":"x-ploiting local data reuse of filter weights and feature mappixels, i.e., activations, in the high-dimensional convolutions,and minimizing data movement of partial sum accumulations","prefix":"hitecture. This is realized by e","suffix":".Unlike dataflows used in existi"}]}]}
>```
>%%
>*%%PREFIX%%hitecture. This is realized by e%%HIGHLIGHT%% ==x-ploiting local data reuse of filter weights and feature mappixels, i.e., activations, in the high-dimensional convolutions,and minimizing data movement of partial sum accumulations== %%POSTFIX%%.Unlike dataflows used in existi*
>%%LINK%%[[#^b3yhbslksxq|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^b3yhbslksxq


>%%
>```annotation-json
>{"created":"2024-01-23T15:55:24.621Z","updated":"2024-01-23T15:55:24.621Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf","target":[{"source":"vault:/Paper Readings/23_01_Eyeriss.pdf","selector":[{"type":"TextPositionSelector","start":1753,"end":1868},{"type":"TextQuoteSelector","exact":" an analysis frameworkthat compares energy cost under the same hardware areaand processing parallelism constraints.","prefix":" different dataflows, we propose","suffix":" Experiments using theCNN config"}]}]}
>```
>%%
>*%%PREFIX%%different dataflows, we propose%%HIGHLIGHT%% ==an analysis frameworkthat compares energy cost under the same hardware areaand processing parallelism constraints.== %%POSTFIX%%Experiments using theCNN config*
>%%LINK%%[[#^aepb6e7qjc7|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^aepb6e7qjc7


>%%
>```annotation-json
>{"created":"2024-01-23T15:58:07.623Z","text":"The paper aims to present a novel dataflow calles *row_stationary*, tjat minimises datamovement through exploiting local data reuse and **activations** for convoltions and minimises data movement for partial sum accumulation.\n\nThe paper also proposes an analysis framework to compare energy cost under the same hardware area and processing parallelism constraints.","updated":"2024-01-23T15:58:07.623Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^e65oex3pfrl|show annotation]]
>%%COMMENT%%
>The paper aims to present a novel dataflow calles *row_stationary*, tjat minimises datamovement through exploiting local data reuse and **activations** for convoltions and minimises data movement for partial sum accumulation.
>
>The paper also proposes an analysis framework to compare energy cost under the same hardware area and processing parallelism constraints.
>%%TAGS%%
>#Abstract
^e65oex3pfrl


>%%
>```annotation-json
>{"created":"2024-01-23T16:00:50.088Z","text":"The focus is on convolutions, and evaluation of performance under the same hardware resource constraints, maximizing for energy efficiency","updated":"2024-01-23T16:00:50.088Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^f9b7quh6njr|show annotation]]
>%%COMMENT%%
>The focus is on convolutions, and evaluation of performance under the same hardware resource constraints, maximizing for energy efficiency
>%%TAGS%%
>
^f9b7quh6njr


>%%
>```annotation-json
>{"created":"2024-01-23T16:01:54.167Z","updated":"2024-01-23T16:01:54.167Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf","target":[{"source":"vault:/Paper Readings/23_01_Eyeriss.pdf","selector":[{"type":"TextPositionSelector","start":4265,"end":4456},{"type":"TextQuoteSelector","exact":"categorize the datamovements in a spatial architecture into several levels ofhierarchy according to their energy cost, and then analyzeeach dataflow to assess the data movement at each level.","prefix":"evaluate energy consumption, we ","suffix":"This analysis framework provides"}]}]}
>```
>%%
>*%%PREFIX%%evaluate energy consumption, we%%HIGHLIGHT%% ==categorize the datamovements in a spatial architecture into several levels ofhierarchy according to their energy cost, and then analyzeeach dataflow to assess the data movement at each level.== %%POSTFIX%%This analysis framework provides*
>%%LINK%%[[#^v6yl6uxpnck|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^v6yl6uxpnck


>%%
>```annotation-json
>{"created":"2024-01-23T16:13:23.630Z","updated":"2024-01-23T16:13:23.630Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf","target":[{"source":"vault:/Paper Readings/23_01_Eyeriss.pdf","selector":[{"type":"TextPositionSelector","start":5545,"end":6517},{"type":"TextQuoteSelector","exact":"• A taxonomy that classifies existing CNN dataflows fromprevious research. (Section IV)• A spatial architecture based on a new CNN dataflow,called row stationary, which is optimized for throughputand energy efficiency. It works on both convolutional andfully-connected layers, and optimizes all types of datamovement in the storage hierarchy. This dataflow hasalso been demonstrated on a fabricated chip. (Section V)• An analysis framework that can quantify the energyefficiency of different CNN dataflows under the samehardware constraints. It can also search for the mostenergy efficient mapping for each dataflow. The analyti-cal model uses energy/area numbers from a commercial65nm process and all R/W numbers are exact basedon real CNN shape configurations, i.e., AlexNet. (Sec-tion VI-C)• For a variety of CNN dataflows, we present a compar-ative analysis of the energy costs associated with datamovement and the impact of different types of datareuse. (Section VII)","prefix":"ntributions of this workinclude:","suffix":"II. SPATIAL ARCHITECTURESpatial "}]}]}
>```
>%%
>*%%PREFIX%%ntributions of this workinclude:%%HIGHLIGHT%% ==• A taxonomy that classifies existing CNN dataflows fromprevious research. (Section IV)• A spatial architecture based on a new CNN dataflow,called row stationary, which is optimized for throughputand energy efficiency. It works on both convolutional andfully-connected layers, and optimizes all types of datamovement in the storage hierarchy. This dataflow hasalso been demonstrated on a fabricated chip. (Section V)• An analysis framework that can quantify the energyefficiency of different CNN dataflows under the samehardware constraints. It can also search for the mostenergy efficient mapping for each dataflow. The analyti-cal model uses energy/area numbers from a commercial65nm process and all R/W numbers are exact basedon real CNN shape configurations, i.e., AlexNet. (Sec-tion VI-C)• For a variety of CNN dataflows, we present a compar-ative analysis of the energy costs associated with datamovement and the impact of different types of datareuse. (Section VII)== %%POSTFIX%%II. SPATIAL ARCHITECTURESpatial*
>%%LINK%%[[#^hu6g5pq6k8b|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^hu6g5pq6k8b


>%%
>```annotation-json
>{"created":"2024-01-23T16:22:40.106Z","updated":"2024-01-23T16:22:40.106Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf","target":[{"source":"vault:/Paper Readings/23_01_Eyeriss.pdf","selector":[{"type":"TextPositionSelector","start":6644,"end":6727},{"type":"TextQuoteSelector","exact":"direct commu-nication between an array of relatively simple processingengines (PEs)","prefix":" high compute parallelism using ","suffix":". They can be designed or progra"}]}]}
>```
>%%
>*%%PREFIX%%high compute parallelism using%%HIGHLIGHT%% ==direct commu-nication between an array of relatively simple processingengines (PEs)== %%POSTFIX%%. They can be designed or progra*
>%%LINK%%[[#^s7n6o5923r|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^s7n6o5923r


>%%
>```annotation-json
>{"created":"2024-01-23T16:22:45.794Z","text":"SIMD?","updated":"2024-01-23T16:22:45.794Z","document":{"title":""},"references":["s7n6o5923r"],"target":[{"source":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^unv6zl8dc1s|show annotation]]
>%%COMMENT%%
>SIMD?
>%%TAGS%%
>#Qn
^unv6zl8dc1s


>%%
>```annotation-json
>{"created":"2024-01-23T16:23:33.595Z","updated":"2024-01-23T16:23:33.595Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf","target":[{"source":"vault:/Paper Readings/23_01_Eyeriss.pdf","selector":[{"type":"TextPositionSelector","start":7079,"end":7252},{"type":"TextQuoteSelector","exact":"coarse-grained SAs that consist oftiled arrays of ALU-style PEs connected together via on-chipnetworks [27–29], and fine-grained SAs that are usually inthe form of an FPGA. ","prefix":"of PEs.SAs come in two flavors: ","suffix":"The expected performance advanta"}]}]}
>```
>%%
>*%%PREFIX%%of PEs.SAs come in two flavors:%%HIGHLIGHT%% ==coarse-grained SAs that consist oftiled arrays of ALU-style PEs connected together via on-chipnetworks [27–29], and fine-grained SAs that are usually inthe form of an FPGA.== %%POSTFIX%%The expected performance advanta*
>%%LINK%%[[#^f038mg5axl|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^f038mg5axl


>%%
>```annotation-json
>{"created":"2024-01-23T16:24:54.569Z","text":"what is the difference b/w this and an SIMD architecture(GPU)","updated":"2024-01-23T16:24:54.569Z","document":{"title":""},"references":["s7n6o5923r"],"target":[{"source":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^v6z6ir18h2p|show annotation]]
>%%COMMENT%%
>what is the difference b/w this and an SIMD architecture(GPU)
>%%TAGS%%
>
^v6z6ir18h2p


>%%
>```annotation-json
>{"text":"The page talks about Spatial Architecture, and how it contributes to efficiency\n\nSA accelerator is composed of global buffers and an array of PEs. The PE interconnects (NoC) design depends on the dataflow requirements. It includes an ALU datapath, a register file as scratchpad, and a PE FIFO to control the traffic going in and out of the ALU\n\nThe focus is on the NoC, which is determined by the compute required by the DNN. There are 4 levels of storage heirarchy for data access, including DRAM, global buffer, array(within PEs) and RF. The difference in levels incurs a different energy cost","created":"2024-01-23T16:35:15.533Z","updated":"2024-01-23T16:35:15.533Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^y6jsoli01o|show annotation]]
>%%COMMENT%%
>The page talks about Spatial Architecture, and how it contributes to efficiency
>
>SA accelerator is composed of global buffers and an array of PEs. The PE interconnects (NoC) design depends on the dataflow requirements. It includes an ALU datapath, a register file as scratchpad, and a PE FIFO to control the traffic going in and out of the ALU
>
>The focus is on the NoC, which is determined by the compute required by the DNN. There are 4 levels of storage heirarchy for data access, including DRAM, global buffer, array(within PEs) and RF. The difference in levels incurs a different energy cost
>%%TAGS%%
>#spatial architecture
^y6jsoli01o


>%%
>```annotation-json
>{"created":"2024-01-25T15:46:19.059Z","updated":"2024-01-25T15:46:19.059Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf","target":[{"source":"vault:/Paper Readings/23_01_Eyeriss.pdf","selector":[{"type":"TextPositionSelector","start":9203,"end":9236},{"type":"TextQuoteSelector","exact":" globalbuffer and an array of PEs","prefix":"rator is primarily composed of a","suffix":". The DRAM, global buffer andPE "}]}]}
>```
>%%
>*%%PREFIX%%rator is primarily composed of a%%HIGHLIGHT%% ==globalbuffer and an array of PEs== %%POSTFIX%%. The DRAM, global buffer andPE*
>%%LINK%%[[#^cyx310u6z5|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^cyx310u6z5


>%%
>```annotation-json
>{"created":"2024-01-25T15:47:44.515Z","updated":"2024-01-25T15:47:44.515Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf","target":[{"source":"vault:/Paper Readings/23_01_Eyeriss.pdf","selector":[{"type":"TextPositionSelector","start":9572,"end":9689},{"type":"TextQuoteSelector","exact":"The PEs in the array are connected via anetwork on chip (NoC), and the NoC design depends on thedataflow requirements","prefix":"cceleration isaround 100–300kB. ","suffix":". The PE includes an ALU datapat"}]}]}
>```
>%%
>*%%PREFIX%%cceleration isaround 100–300kB.%%HIGHLIGHT%% ==The PEs in the array are connected via anetwork on chip (NoC), and the NoC design depends on thedataflow requirements== %%POSTFIX%%. The PE includes an ALU datapat*
>%%LINK%%[[#^ckpoaoqhw9a|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^ckpoaoqhw9a


>%%
>```annotation-json
>{"created":"2024-01-25T15:54:57.990Z","updated":"2024-01-25T15:54:57.990Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf","target":[{"source":"vault:/Paper Readings/23_01_Eyeriss.pdf","selector":[{"type":"TextPositionSelector","start":13586,"end":13767},{"type":"TextQuoteSelector","exact":" Processing of POOL layers can sharethe same compute scheme used for CONV layers since itscomputation is a degenerate form of Eq. (1), where the MACis replaced with a MAX operation.","prefix":"NV/FC layer.impact of FC layers.","suffix":" Computation of ACTlayers is tri"}]}]}
>```
>%%
>*%%PREFIX%%NV/FC layer.impact of FC layers.%%HIGHLIGHT%% ==Processing of POOL layers can sharethe same compute scheme used for CONV layers since itscomputation is a degenerate form of Eq. (1), where the MACis replaced with a MAX operation.== %%POSTFIX%%Computation of ACTlayers is tri*
>%%LINK%%[[#^58iv5z4pq6l|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^58iv5z4pq6l


>%%
>```annotation-json
>{"created":"2024-01-25T15:55:36.037Z","updated":"2024-01-25T15:55:36.037Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf","target":[{"source":"vault:/Paper Readings/23_01_Eyeriss.pdf","selector":[{"type":"TextPositionSelector","start":12930,"end":13087},{"type":"TextQuoteSelector","exact":"Even thoughFC layers use most of the filter weights, a recent study hasdemonstrated that these weights are largely compressible to1–5% of their original size","prefix":" and energy efficiency of CNNs. ","suffix":" [38], which greatly reduces the"}]}]}
>```
>%%
>*%%PREFIX%%and energy efficiency of CNNs.%%HIGHLIGHT%% ==Even thoughFC layers use most of the filter weights, a recent study hasdemonstrated that these weights are largely compressible to1–5% of their original size== %%POSTFIX%%[38], which greatly reduces the*
>%%LINK%%[[#^m053kg4m7h|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^m053kg4m7h


>%%
>```annotation-json
>{"created":"2024-01-25T15:59:33.381Z","updated":"2024-01-25T15:59:33.381Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf","target":[{"source":"vault:/Paper Readings/23_01_Eyeriss.pdf","selector":[{"type":"TextPositionSelector","start":14796,"end":14948},{"type":"TextQuoteSelector","exact":"Each filter weightis reused E2 times in the same ifmap plane, and eachifmap pixel, i.e., activation, is usually reused R2 timesin the same filter plane.","prefix":" shared across many operations. ","suffix":" FC layers, however, do not have"}]}]}
>```
>%%
>*%%PREFIX%%shared across many operations.%%HIGHLIGHT%% ==Each filter weightis reused E2 times in the same ifmap plane, and eachifmap pixel, i.e., activation, is usually reused R2 timesin the same filter plane.== %%POSTFIX%%FC layers, however, do not have*
>%%LINK%%[[#^t4um3rvshcl|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^t4um3rvshcl


>%%
>```annotation-json
>{"created":"2024-01-25T15:52:50.998Z","text":"When it comes to CNNs, the challenges involve streamlining convolution as most of the models are made up of 90 percent CONV layers. There are 2 main challenges involved in CONV and FC layers:\n\n1. Data Handling: Naive parallelism is not the answer due to storage and bandwidth limitations. Hence, data reuse has to be implemented through:   \n    a. convolutional reuse: weights are shared in CONV layer, does not impact FC layers\n    b. filter reuse: The filter weights can be reused across N ifmaps\n    c. ifmap reuse: Each pixel is reused across M filters in both CONV and FC layers\n\n2. Adaptive processing: dataflow must be efficient for different shapes","updated":"2024-01-25T15:52:50.998Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^ra8b7rgk98j|show annotation]]
>%%COMMENT%%
>When it comes to CNNs, the challenges involve streamlining convolution as most of the models are made up of 90 percent CONV layers. There are 2 main challenges involved in CONV and FC layers:
>
>1. Data Handling: Naive parallelism is not the answer due to storage and bandwidth limitations. Hence, data reuse has to be implemented through:   
>    a. convolutional reuse: weights are shared in CONV layer, does not impact FC layers
>    b. filter reuse: The filter weights can be reused across N ifmaps
>    c. ifmap reuse: Each pixel is reused across M filters in both CONV and FC layers
>
>2. Adaptive processing: dataflow must be efficient for different shapes
>%%TAGS%%
>
^ra8b7rgk98j


>%%
>```annotation-json
>{"created":"2024-01-25T16:11:04.460Z","text":"Row Stationary dataflow breaks a high dimensional convolution down to 1D convolution primitives that can run in parallel., each primitive operates on one row of filter weights anf one row of ifmap pixels.","updated":"2024-01-25T16:11:04.460Z","document":{"title":"Eyeriss: A Spatial Architecture for Energy-Efficient Dataflow for Convolutional Neural Networks","link":[{"href":"urn:x-pdf:4a1b97d282990344399b4bc1d541cb1f"},{"href":"vault:/Paper Readings/23_01_Eyeriss.pdf"}],"documentFingerprint":"4a1b97d282990344399b4bc1d541cb1f"},"uri":"vault:/Paper Readings/23_01_Eyeriss.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^2lx1hexyxu3|show annotation]]
>%%COMMENT%%
>Row Stationary dataflow breaks a high dimensional convolution down to 1D convolution primitives that can run in parallel., each primitive operates on one row of filter weights anf one row of ifmap pixels.
>%%TAGS%%
>
^2lx1hexyxu3
