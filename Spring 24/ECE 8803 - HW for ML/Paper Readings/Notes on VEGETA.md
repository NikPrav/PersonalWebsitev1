---
annotation-target: Paper Readings/02_13_VEGETA.pdf
annotation-target-type: pdf
---


>%%
>```annotation-json
>{"created":"2024-02-13T16:33:09.373Z","text":"The paper introduces a set of ISA and microarchitecture extensions over dense matrix engines for better calculation of sparse workloads through supporting flexible structured sparsity for CPUs. The performance is then compared to CPUs and the potential acceleration gained","updated":"2024-02-13T16:33:09.373Z","document":{"title":"VEGETA: Vertically-Integrated Extensions for Sparse/Dense GEMM Tile Acceleration on CPUs","link":[{"href":"urn:x-pdf:abcfd1e9ae1317ca19b200e720464beb"},{"href":"vault:/Paper Readings/02_13_VEGETA.pdf"}],"documentFingerprint":"abcfd1e9ae1317ca19b200e720464beb"},"uri":"vault:/Paper Readings/02_13_VEGETA.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^7gzr2qp60ol|show annotation]]
>%%COMMENT%%
>The paper introduces a set of ISA and microarchitecture extensions over dense matrix engines for better calculation of sparse workloads through supporting flexible structured sparsity for CPUs. The performance is then compared to CPUs and the potential acceleration gained
>%%TAGS%%
>#Abstract
^7gzr2qp60ol


>%%
>```annotation-json
>{"created":"2024-02-13T16:36:43.750Z","text":"as opposed to? structured v/s unstructured sparsity","updated":"2024-02-13T16:36:43.750Z","document":{"title":"VEGETA: Vertically-Integrated Extensions for Sparse/Dense GEMM Tile Acceleration on CPUs","link":[{"href":"urn:x-pdf:abcfd1e9ae1317ca19b200e720464beb"},{"href":"vault:/Paper Readings/02_13_VEGETA.pdf"}],"documentFingerprint":"abcfd1e9ae1317ca19b200e720464beb"},"uri":"vault:/Paper Readings/02_13_VEGETA.pdf","target":[{"source":"vault:/Paper Readings/02_13_VEGETA.pdf","selector":[{"type":"TextPositionSelector","start":1149,"end":1177},{"type":"TextQuoteSelector","exact":"flexible structured sparsity","prefix":"dense matrix engines to support ","suffix":" forCPUs, enabling programmable "}]}]}
>```
>%%
>*%%PREFIX%%dense matrix engines to support%%HIGHLIGHT%% ==flexible structured sparsity== %%POSTFIX%%forCPUs, enabling programmable*
>%%LINK%%[[#^qi038612g0c|show annotation]]
>%%COMMENT%%
>as opposed to? structured v/s unstructured sparsity
>%%TAGS%%
>#Qn
^qi038612g0c


>%%
>```annotation-json
>{"created":"2024-02-13T16:37:40.225Z","text":"VEGETA focuses on edge devices?","updated":"2024-02-13T16:37:40.225Z","document":{"title":"VEGETA: Vertically-Integrated Extensions for Sparse/Dense GEMM Tile Acceleration on CPUs","link":[{"href":"urn:x-pdf:abcfd1e9ae1317ca19b200e720464beb"},{"href":"vault:/Paper Readings/02_13_VEGETA.pdf"}],"documentFingerprint":"abcfd1e9ae1317ca19b200e720464beb"},"uri":"vault:/Paper Readings/02_13_VEGETA.pdf","target":[{"source":"vault:/Paper Readings/02_13_VEGETA.pdf","selector":[{"type":"TextPositionSelector","start":2364,"end":2422},{"type":"TextQuoteSelector","exact":"edgedevices with tight area/power budget [46] prefer CPUs ","prefix":"l networks (DNNs). For example, ","suffix":"sinceGPUs/accelerators cannot be"}]}]}
>```
>%%
>*%%PREFIX%%l networks (DNNs). For example,%%HIGHLIGHT%% ==edgedevices with tight area/power budget [46] prefer CPUs== %%POSTFIX%%sinceGPUs/accelerators cannot be*
>%%LINK%%[[#^4j0biz4bwtu|show annotation]]
>%%COMMENT%%
>VEGETA focuses on edge devices?
>%%TAGS%%
>
^4j0biz4bwtu


>%%
>```annotation-json
>{"created":"2024-02-13T16:38:12.974Z","updated":"2024-02-13T16:38:12.974Z","document":{"title":"VEGETA: Vertically-Integrated Extensions for Sparse/Dense GEMM Tile Acceleration on CPUs","link":[{"href":"urn:x-pdf:abcfd1e9ae1317ca19b200e720464beb"},{"href":"vault:/Paper Readings/02_13_VEGETA.pdf"}],"documentFingerprint":"abcfd1e9ae1317ca19b200e720464beb"},"uri":"vault:/Paper Readings/02_13_VEGETA.pdf","target":[{"source":"vault:/Paper Readings/02_13_VEGETA.pdf","selector":[{"type":"TextPositionSelector","start":2751,"end":2887},{"type":"TextQuoteSelector","exact":"offloading a modest-size task toan accelerator or a GPU might not be the best option ifthe offloading overhead is relatively substantial","prefix":"xityand cost [18]. Furthermore, ","suffix":" [48]. Finally,§ Sana Damani and"}]}]}
>```
>%%
>*%%PREFIX%%xityand cost [18]. Furthermore,%%HIGHLIGHT%% ==offloading a modest-size task toan accelerator or a GPU might not be the best option ifthe offloading overhead is relatively substantial== %%POSTFIX%%[48]. Finally,§ Sana Damani and*
>%%LINK%%[[#^0werzmq4a1jp|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^0werzmq4a1jp


>%%
>```annotation-json
>{"created":"2024-02-13T16:41:44.478Z","updated":"2024-02-13T16:41:44.478Z","document":{"title":"VEGETA: Vertically-Integrated Extensions for Sparse/Dense GEMM Tile Acceleration on CPUs","link":[{"href":"urn:x-pdf:abcfd1e9ae1317ca19b200e720464beb"},{"href":"vault:/Paper Readings/02_13_VEGETA.pdf"}],"documentFingerprint":"abcfd1e9ae1317ca19b200e720464beb"},"uri":"vault:/Paper Readings/02_13_VEGETA.pdf","target":[{"source":"vault:/Paper Readings/02_13_VEGETA.pdf","selector":[{"type":"TextPositionSelector","start":3661,"end":4021},{"type":"TextQuoteSelector","exact":"Recent research has focused on adding hardware support inDNN accelerators to handle sparsity as it can be used to im-prove power and performance by skipping or gating ineffectualcomputations (since anything multiplied by zero is zero) andto reduce memory capacity and bandwidth requirements bysaving only non-zero values and their indices in a compressedmanner","prefix":"/vector engines over many years.","suffix":" [13], [23], [42], [43]. CPUs, h"}]}]}
>```
>%%
>*%%PREFIX%%/vector engines over many years.%%HIGHLIGHT%% ==Recent research has focused on adding hardware support inDNN accelerators to handle sparsity as it can be used to im-prove power and performance by skipping or gating ineffectualcomputations (since anything multiplied by zero is zero) andto reduce memory capacity and bandwidth requirements bysaving only non-zero values and their indices in a compressedmanner== %%POSTFIX%%[13], [23], [42], [43]. CPUs, h*
>%%LINK%%[[#^ob5sw4hof5s|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^ob5sw4hof5s


>%%
>```annotation-json
>{"created":"2024-02-13T16:41:51.720Z","text":"# Why CPUs\n- CPUs are preferred by EDGE devices\n- Running small models are easier on CPUs due to the overhead when it comes to offloading data","updated":"2024-02-13T16:41:51.720Z","document":{"title":"VEGETA: Vertically-Integrated Extensions for Sparse/Dense GEMM Tile Acceleration on CPUs","link":[{"href":"urn:x-pdf:abcfd1e9ae1317ca19b200e720464beb"},{"href":"vault:/Paper Readings/02_13_VEGETA.pdf"}],"documentFingerprint":"abcfd1e9ae1317ca19b200e720464beb"},"uri":"vault:/Paper Readings/02_13_VEGETA.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^t0w4v1unr89|show annotation]]
>%%COMMENT%%
># Why CPUs
>- CPUs are preferred by EDGE devices
>- Running small models are easier on CPUs due to the overhead when it comes to offloading data
>%%TAGS%%
>
^t0w4v1unr89


>%%
>```annotation-json
>{"created":"2024-02-13T16:42:59.972Z","text":"Does the normal stuff that speed up a CPU also speed this up? Can they be leveraged for the CPUs advantage here?\n","updated":"2024-02-13T16:42:59.972Z","document":{"title":"VEGETA: Vertically-Integrated Extensions for Sparse/Dense GEMM Tile Acceleration on CPUs","link":[{"href":"urn:x-pdf:abcfd1e9ae1317ca19b200e720464beb"},{"href":"vault:/Paper Readings/02_13_VEGETA.pdf"}],"documentFingerprint":"abcfd1e9ae1317ca19b200e720464beb"},"uri":"vault:/Paper Readings/02_13_VEGETA.pdf","target":[{"source":"vault:/Paper Readings/02_13_VEGETA.pdf","selector":[{"type":"TextPositionSelector","start":4106,"end":4468},{"type":"TextQuoteSelector","exact":"(i) Being general-purpose,CPUs are particularly sensitive to the amount of hardwaredevoted to improving a subset of workloads. (ii) At the sametime, new functional units in CPUs need to be able to supporta wide variety of use cases. (iii) CPUs need programmabilitysupport to handle sparsity unlike offload accelerators withcustom DMA engines for sparse accesses.","prefix":"ollowing additional challenges. ","suffix":"In this paper, we introduce VEGE"}]}]}
>```
>%%
>*%%PREFIX%%ollowing additional challenges.%%HIGHLIGHT%% ==(i) Being general-purpose,CPUs are particularly sensitive to the amount of hardwaredevoted to improving a subset of workloads. (ii) At the sametime, new functional units in CPUs need to be able to supporta wide variety of use cases. (iii) CPUs need programmabilitysupport to handle sparsity unlike offload accelerators withcustom DMA engines for sparse accesses.== %%POSTFIX%%In this paper, we introduce VEGE*
>%%LINK%%[[#^n6uqbdfiebb|show annotation]]
>%%COMMENT%%
>Does the normal stuff that speed up a CPU also speed this up? Can they be leveraged for the CPUs advantage here?
>
>%%TAGS%%
>
^n6uqbdfiebb


>%%
>```annotation-json
>{"created":"2024-02-13T16:44:20.172Z","updated":"2024-02-13T16:44:20.172Z","document":{"title":"VEGETA: Vertically-Integrated Extensions for Sparse/Dense GEMM Tile Acceleration on CPUs","link":[{"href":"urn:x-pdf:abcfd1e9ae1317ca19b200e720464beb"},{"href":"vault:/Paper Readings/02_13_VEGETA.pdf"}],"documentFingerprint":"abcfd1e9ae1317ca19b200e720464beb"},"uri":"vault:/Paper Readings/02_13_VEGETA.pdf","target":[{"source":"vault:/Paper Readings/02_13_VEGETA.pdf","selector":[{"type":"TextPositionSelector","start":5344,"end":5385},{"type":"TextQuoteSelector","exact":"Sparsity-aware NPU in a Samsung Mobile AP","prefix":" in NVIDIA’s Ampere GPU [39]and ","suffix":" [28].978-1-6654-7652-2/23/$31.0"}]}]}
>```
>%%
>*%%PREFIX%%in NVIDIA’s Ampere GPU [39]and%%HIGHLIGHT%% ==Sparsity-aware NPU in a Samsung Mobile AP== %%POSTFIX%%[28].978-1-6654-7652-2/23/$31.0*
>%%LINK%%[[#^58fe4pp80t|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^58fe4pp80t


>%%
>```annotation-json
>{"created":"2024-02-13T16:44:52.085Z","text":"here, a DNN accelerator is extended. Is the accelerator with the extension used in tandem with the CPU? Does the accelerator matter once the data is offloaded?","updated":"2024-02-13T16:44:52.085Z","document":{"title":"VEGETA: Vertically-Integrated Extensions for Sparse/Dense GEMM Tile Acceleration on CPUs","link":[{"href":"urn:x-pdf:abcfd1e9ae1317ca19b200e720464beb"},{"href":"vault:/Paper Readings/02_13_VEGETA.pdf"}],"documentFingerprint":"abcfd1e9ae1317ca19b200e720464beb"},"uri":"vault:/Paper Readings/02_13_VEGETA.pdf","target":[{"source":"vault:/Paper Readings/02_13_VEGETA.pdf","selector":[{"type":"TextPositionSelector","start":6020,"end":6048},{"type":"TextQuoteSelector","exact":"new architectural extensions","prefix":"tware optimizations.•We propose ","suffix":" to a systolic-array-based matri"}]}]}
>```
>%%
>*%%PREFIX%%tware optimizations.•We propose%%HIGHLIGHT%% ==new architectural extensions== %%POSTFIX%%to a systolic-array-based matri*
>%%LINK%%[[#^mzv5llz7je|show annotation]]
>%%COMMENT%%
>here, a DNN accelerator is extended. Is the accelerator with the extension used in tandem with the CPU? Does the accelerator matter once the data is offloaded?
>%%TAGS%%
>
^mzv5llz7je


>%%
>```annotation-json
>{"created":"2024-02-13T16:51:16.260Z","updated":"2024-02-13T16:51:16.260Z","document":{"title":"VEGETA: Vertically-Integrated Extensions for Sparse/Dense GEMM Tile Acceleration on CPUs","link":[{"href":"urn:x-pdf:abcfd1e9ae1317ca19b200e720464beb"},{"href":"vault:/Paper Readings/02_13_VEGETA.pdf"}],"documentFingerprint":"abcfd1e9ae1317ca19b200e720464beb"},"uri":"vault:/Paper Readings/02_13_VEGETA.pdf","target":[{"source":"vault:/Paper Readings/02_13_VEGETA.pdf","selector":[{"type":"TextPositionSelector","start":8282,"end":8381},{"type":"TextQuoteSelector","exact":"Weight (static) sparsity is derivedby pruning some edges in a DNN with a small sacrifice inaccuracy","prefix":"ainsources of sparsity in DNNs. ","suffix":" [19], [20]. This leads to zeros"}]}]}
>```
>%%
>*%%PREFIX%%ainsources of sparsity in DNNs.%%HIGHLIGHT%% ==Weight (static) sparsity is derivedby pruning some edges in a DNN with a small sacrifice inaccuracy== %%POSTFIX%%[19], [20]. This leads to zeros*
>%%LINK%%[[#^k9ujn7c7w6f|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^k9ujn7c7w6f


>%%
>```annotation-json
>{"created":"2024-02-13T16:51:30.808Z","updated":"2024-02-13T16:51:30.808Z","document":{"title":"VEGETA: Vertically-Integrated Extensions for Sparse/Dense GEMM Tile Acceleration on CPUs","link":[{"href":"urn:x-pdf:abcfd1e9ae1317ca19b200e720464beb"},{"href":"vault:/Paper Readings/02_13_VEGETA.pdf"}],"documentFingerprint":"abcfd1e9ae1317ca19b200e720464beb"},"uri":"vault:/Paper Readings/02_13_VEGETA.pdf","target":[{"source":"vault:/Paper Readings/02_13_VEGETA.pdf","selector":[{"type":"TextPositionSelector","start":8436,"end":8510},{"type":"TextQuoteSelector","exact":"nput (dynamic) sparsity is usually induced by a popularactivation function","prefix":" to zeros in the weight matrix.I","suffix":", Rectified Linear Unit (ReLU), "}]}]}
>```
>%%
>*%%PREFIX%%to zeros in the weight matrix.I%%HIGHLIGHT%% ==nput (dynamic) sparsity is usually induced by a popularactivation function== %%POSTFIX%%, Rectified Linear Unit (ReLU),*
>%%LINK%%[[#^wbmwbz41ski|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^wbmwbz41ski


>%%
>```annotation-json
>{"created":"2024-02-13T16:54:08.164Z","updated":"2024-02-13T16:54:08.164Z","document":{"title":"VEGETA: Vertically-Integrated Extensions for Sparse/Dense GEMM Tile Acceleration on CPUs","link":[{"href":"urn:x-pdf:abcfd1e9ae1317ca19b200e720464beb"},{"href":"vault:/Paper Readings/02_13_VEGETA.pdf"}],"documentFingerprint":"abcfd1e9ae1317ca19b200e720464beb"},"uri":"vault:/Paper Readings/02_13_VEGETA.pdf","target":[{"source":"vault:/Paper Readings/02_13_VEGETA.pdf","selector":[{"type":"TextPositionSelector","start":11704,"end":11830},{"type":"TextQuoteSelector","exact":"A matrix engine canprovide power-efficient high compute throughput via simplecontrol logic and significant internal data reuse","prefix":"es inside CPUs [9], [24], [26]. ","suffix":". For example,in Intel’s upcomin"}]}]}
>```
>%%
>*%%PREFIX%%es inside CPUs [9], [24], [26].%%HIGHLIGHT%% ==A matrix engine canprovide power-efficient high compute throughput via simplecontrol logic and significant internal data reuse== %%POSTFIX%%. For example,in Intel’s upcomin*
>%%LINK%%[[#^f6pzx174ez|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^f6pzx174ez


>%%
>```annotation-json
>{"created":"2024-02-13T16:55:25.132Z","updated":"2024-02-13T16:55:25.132Z","document":{"title":"VEGETA: Vertically-Integrated Extensions for Sparse/Dense GEMM Tile Acceleration on CPUs","link":[{"href":"urn:x-pdf:abcfd1e9ae1317ca19b200e720464beb"},{"href":"vault:/Paper Readings/02_13_VEGETA.pdf"}],"documentFingerprint":"abcfd1e9ae1317ca19b200e720464beb"},"uri":"vault:/Paper Readings/02_13_VEGETA.pdf","target":[{"source":"vault:/Paper Readings/02_13_VEGETA.pdf","selector":[{"type":"TextPositionSelector","start":14328,"end":14414},{"type":"TextQuoteSelector","exact":"The irregular nature of unstructured sparsitymeans we cannot know tile sizes a priori,","prefix":"rating on fixedsize tiles [17]. ","suffix":" and further, theymay all be dif"}]}]}
>```
>%%
>*%%PREFIX%%rating on fixedsize tiles [17].%%HIGHLIGHT%% ==The irregular nature of unstructured sparsitymeans we cannot know tile sizes a priori,== %%POSTFIX%%and further, theymay all be dif*
>%%LINK%%[[#^ohyr7vth73p|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^ohyr7vth73p


>%%
>```annotation-json
>{"created":"2024-02-13T16:56:15.113Z","text":"**Structured Sparsity:** Given a DNN, each block with M elements have at most N zeros\n\n**Unstructured Sparsity:** No such pattern exists","updated":"2024-02-13T16:56:15.113Z","document":{"title":"VEGETA: Vertically-Integrated Extensions for Sparse/Dense GEMM Tile Acceleration on CPUs","link":[{"href":"urn:x-pdf:abcfd1e9ae1317ca19b200e720464beb"},{"href":"vault:/Paper Readings/02_13_VEGETA.pdf"}],"documentFingerprint":"abcfd1e9ae1317ca19b200e720464beb"},"uri":"vault:/Paper Readings/02_13_VEGETA.pdf","target":[{"source":"vault:/Paper Readings/02_13_VEGETA.pdf","selector":[{"type":"TextPositionSelector","start":9886,"end":10149},{"type":"TextQuoteSelector","exact":"The non-zeros for a DNN may have apattern, such as certain channels of weights being all zero(through channel pruning) or each block with M elementshaving at most N non-zeros (often called N:M sparsity [52]).“Unstructured sparsity” indicates the lack of a pattern","prefix":"ned atruntime.Sparsity pattern. ","suffix":".Sparsity granularity. Sparsity "}]}]}
>```
>%%
>*%%PREFIX%%ned atruntime.Sparsity pattern.%%HIGHLIGHT%% ==The non-zeros for a DNN may have apattern, such as certain channels of weights being all zero(through channel pruning) or each block with M elementshaving at most N non-zeros (often called N:M sparsity [52]).“Unstructured sparsity” indicates the lack of a pattern== %%POSTFIX%%.Sparsity granularity. Sparsity*
>%%LINK%%[[#^5hx25hh658s|show annotation]]
>%%COMMENT%%
>**Structured Sparsity:** Given a DNN, each block with M elements have at most N zeros
>
>**Unstructured Sparsity:** No such pattern exists
>%%TAGS%%
>#info
^5hx25hh658s


>%%
>```annotation-json
>{"created":"2024-02-13T16:58:31.469Z","text":"The focus is on structured sparsity due to\n- Progammability for unstructured sparsity is low since the tile sizes are not known beforehand\n- The overheads in storing sparse matrices as opposed to dense ones are high since indices and values are stored separately\n\nUnstructured sparsity can be supported through transforming the target matrix using row-wise N:M sparsity","updated":"2024-02-13T16:58:31.469Z","document":{"title":"VEGETA: Vertically-Integrated Extensions for Sparse/Dense GEMM Tile Acceleration on CPUs","link":[{"href":"urn:x-pdf:abcfd1e9ae1317ca19b200e720464beb"},{"href":"vault:/Paper Readings/02_13_VEGETA.pdf"}],"documentFingerprint":"abcfd1e9ae1317ca19b200e720464beb"},"uri":"vault:/Paper Readings/02_13_VEGETA.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^gcmt5tlgrps|show annotation]]
>%%COMMENT%%
>The focus is on structured sparsity due to
>- Progammability for unstructured sparsity is low since the tile sizes are not known beforehand
>- The overheads in storing sparse matrices as opposed to dense ones are high since indices and values are stored separately
>
>Unstructured sparsity can be supported through transforming the target matrix using row-wise N:M sparsity
>%%TAGS%%
>
^gcmt5tlgrps
