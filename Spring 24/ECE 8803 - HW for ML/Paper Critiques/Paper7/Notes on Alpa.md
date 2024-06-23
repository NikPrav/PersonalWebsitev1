---
annotation-target: Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf
annotation-target-type: pdf
---


>%%
>```annotation-json
>{"created":"2024-04-02T18:48:37.228Z","text":"Automates model training by generation of execution plans that takes care of data, operator and pipeline parallelism. It distributes parallelisation into two layers: intra-operator and inter-operator, which is then used to create a new heirarchical space for model execution plans","updated":"2024-04-02T18:48:37.228Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^0g35lqsuurrp|show annotation]]
>%%COMMENT%%
>Automates model training by generation of execution plans that takes care of data, operator and pipeline parallelism. It distributes parallelisation into two layers: intra-operator and inter-operator, which is then used to create a new heirarchical space for model execution plans
>%%TAGS%%
>#abstract
^0g35lqsuurrp


>%%
>```annotation-json
>{"created":"2024-04-02T18:56:48.752Z","updated":"2024-04-02T18:56:48.752Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":3867,"end":4010},{"type":"TextQuoteSelector","exact":"Alpa constructs a hierarchical spaceand uses a set of compilation passes to derive efficient parallelexecution plans at each parallelism level.","prefix":"nd inter-operator parallelisms. ","suffix":" Alpa orchestratesthe parallel e"}]}]}
>```
>%%
>*%%PREFIX%%nd inter-operator parallelisms.%%HIGHLIGHT%% ==Alpa constructs a hierarchical spaceand uses a set of compilation passes to derive efficient parallelexecution plans at each parallelism level.== %%POSTFIX%%Alpa orchestratesthe parallel e*
>%%LINK%%[[#^wdoo4y205q7|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^wdoo4y205q7


>%%
>```annotation-json
>{"created":"2024-04-02T18:57:08.155Z","text":"## Questions\nWhat h/w does it optimise to?\nDoes it take into account special h/w features?\nWhen it comes to parallelism, what all does that include?","updated":"2024-04-02T18:57:08.155Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^4419theih0w|show annotation]]
>%%COMMENT%%
>## Questions
>What h/w does it optimise to?
>Does it take into account special h/w features?
>When it comes to parallelism, what all does that include?
>%%TAGS%%
>#qns
^4419theih0w


>%%
>```annotation-json
>{"created":"2024-04-02T19:29:38.107Z","updated":"2024-04-02T19:29:38.107Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":902,"end":1235},{"type":"TextQuoteSelector","exact":"intra-operator parallelism has better device utilization, but resultsin communicating at every split and merge of partitionedoperators, per training iteration; whereas inter-operator par-allelism only communicates between adjacent stages, whichcan be light if sliced properly, but incurs device idle time dueto scheduling constraints","prefix":"ature distinct characteristics: ","suffix":". We can harness the asymmetricn"}]}]}
>```
>%%
>*%%PREFIX%%ature distinct characteristics:%%HIGHLIGHT%% ==intra-operator parallelism has better device utilization, but resultsin communicating at every split and merge of partitionedoperators, per training iteration; whereas inter-operator par-allelism only communicates between adjacent stages, whichcan be light if sliced properly, but incurs device idle time dueto scheduling constraints== %%POSTFIX%%. We can harness the asymmetricn*
>%%LINK%%[[#^3liq649ohr4|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^3liq649ohr4


>%%
>```annotation-json
>{"created":"2024-04-02T19:30:01.590Z","updated":"2024-04-02T19:30:01.590Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":1244,"end":1299},{"type":"TextQuoteSelector","exact":"harness the asymmetricnature of communication bandwidth","prefix":" scheduling constraints. We can ","suffix":" in a compute cluster,and map in"}]}]}
>```
>%%
>*%%PREFIX%%scheduling constraints. We can%%HIGHLIGHT%% ==harness the asymmetricnature of communication bandwidth== %%POSTFIX%%in a compute cluster,and map in*
>%%LINK%%[[#^r2yx2bgvirh|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^r2yx2bgvirh


>%%
>```annotation-json
>{"created":"2024-04-02T19:30:06.594Z","updated":"2024-04-02T19:30:06.594Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":1324,"end":1528},{"type":"TextQuoteSelector","exact":" map intra-operator parallelism to devices connected withhigh communication bandwidth, while orchestrating the inter-operator parallelism between distant devices with relativelylower bandwidth in between.","prefix":"ndwidth in a compute cluster,and","suffix":" Second, this hierarchical desig"}]}]}
>```
>%%
>*%%PREFIX%%ndwidth in a compute cluster,and%%HIGHLIGHT%% ==map intra-operator parallelism to devices connected withhigh communication bandwidth, while orchestrating the inter-operator parallelism between distant devices with relativelylower bandwidth in between.== %%POSTFIX%%Second, this hierarchical desig*
>%%LINK%%[[#^ghv200o4sut|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^ghv200o4sut


>%%
>```annotation-json
>{"created":"2024-04-02T19:50:34.920Z","updated":"2024-04-02T19:50:34.920Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":2479,"end":2628},{"type":"TextQuoteSelector","exact":"We construct a two-level parallel execution plan space(Fig. 1e) where plans are specified hierarchically using inter-and intra-operator parallelisms.","prefix":"e the following contributions:• ","suffix":"•We design tractable optimizatio"}]}]}
>```
>%%
>*%%PREFIX%%e the following contributions:•%%HIGHLIGHT%% ==We construct a two-level parallel execution plan space(Fig. 1e) where plans are specified hierarchically using inter-and intra-operator parallelisms.== %%POSTFIX%%•We design tractable optimizatio*
>%%LINK%%[[#^wssv30x5ws|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^wssv30x5ws


>%%
>```annotation-json
>{"created":"2024-04-02T19:50:40.681Z","updated":"2024-04-02T19:50:40.681Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":2629,"end":2725},{"type":"TextQuoteSelector","exact":"We design tractable optimization algorithms to derive near-optimal execution plans at each level","prefix":"nd intra-operator parallelisms.•","suffix":".•We implement Alpa, a compiler "}]}]}
>```
>%%
>*%%PREFIX%%nd intra-operator parallelisms.•%%HIGHLIGHT%% ==We design tractable optimization algorithms to derive near-optimal execution plans at each level== %%POSTFIX%%.•We implement Alpa, a compiler*
>%%LINK%%[[#^wwwxikvjtpp|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^wwwxikvjtpp


>%%
>```annotation-json
>{"created":"2024-04-02T19:50:45.365Z","updated":"2024-04-02T19:50:45.365Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":2727,"end":3121},{"type":"TextQuoteSelector","exact":"We implement Alpa, a compiler system for distributed DLon GPU clusters. Alpa features: (1) a set of compilation passesthat generate execution plans using the hierarchical optimiza-tion algorithms, (2) a new runtime architecture that orches-trates the inter-op parallelism between device meshes, and (3)a number of system optimizations that improve compilationand address cross-mesh communicatio","prefix":" execution plans at each level.•","suffix":"n.A B DCA B DC...A B DCA B DCA B"}]}]}
>```
>%%
>*%%PREFIX%%execution plans at each level.•%%HIGHLIGHT%% ==We implement Alpa, a compiler system for distributed DLon GPU clusters. Alpa features: (1) a set of compilation passesthat generate execution plans using the hierarchical optimiza-tion algorithms, (2) a new runtime architecture that orches-trates the inter-op parallelism between device meshes, and (3)a number of system optimizations that improve compilationand address cross-mesh communicatio== %%POSTFIX%%n.A B DCA B DC...A B DCA B DCA B*
>%%LINK%%[[#^y5k4o4wnwt|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^y5k4o4wnwt


>%%
>```annotation-json
>{"created":"2024-04-02T19:50:51.337Z","updated":"2024-04-02T19:50:51.337Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":3835,"end":3905},{"type":"TextQuoteSelector","exact":"We evaluate Alpa on training large models with billionsof parameters. ","prefix":"d inter-operator parallelisms.• ","suffix":"We compare Alpa with state-of-th"}]}]}
>```
>%%
>*%%PREFIX%%d inter-operator parallelisms.•%%HIGHLIGHT%% ==We evaluate Alpa on training large models with billionsof parameters.== %%POSTFIX%%We compare Alpa with state-of-th*
>%%LINK%%[[#^8kep8jo5tka|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^8kep8jo5tka


>%%
>```annotation-json
>{"created":"2024-04-02T19:56:31.743Z","updated":"2024-04-02T19:56:31.743Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":5309,"end":5546},{"type":"TextQuoteSelector","exact":". An operator works on multi-dimensional tensors. We can partition the tensor along somedimensions, assign the resulting partitioned computations tomultiple devices, and let them execute different portions ofthe operator at the same time","prefix":"lisms.Intra-operator parallelism","suffix":". We define all parallelizationa"}]}]}
>```
>%%
>*%%PREFIX%%lisms.Intra-operator parallelism%%HIGHLIGHT%% ==. An operator works on multi-dimensional tensors. We can partition the tensor along somedimensions, assign the resulting partitioned computations tomultiple devices, and let them execute different portions ofthe operator at the same time== %%POSTFIX%%. We define all parallelizationa*
>%%LINK%%[[#^7ye1f0gs7kk|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^7ye1f0gs7kk


>%%
>```annotation-json
>{"created":"2024-04-02T19:56:41.076Z","updated":"2024-04-02T19:56:41.076Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":3527,"end":3541},{"type":"TextQuoteSelector","exact":"3D Parallelism","prefix":"e models, which isalso known as ","suffix":". By assuming the model has thes"}]}]}
>```
>%%
>*%%PREFIX%%e models, which isalso known as%%HIGHLIGHT%% ==3D Parallelism== %%POSTFIX%%. By assuming the model has thes*
>%%LINK%%[[#^5uauft8qsxk|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^5uauft8qsxk


>%%
>```annotation-json
>{"created":"2024-04-02T19:56:50.458Z","updated":"2024-04-02T19:56:50.458Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":3808,"end":3884},{"type":"TextQuoteSelector","exact":"manual plan cannot generalize to different models or differentcluster setups","prefix":"irement of strong expertise, the","suffix":" (§8.1).Automatic combination of"}]}]}
>```
>%%
>*%%PREFIX%%irement of strong expertise, the%%HIGHLIGHT%% ==manual plan cannot generalize to different models or differentcluster setups== %%POSTFIX%%(§8.1).Automatic combination of*
>%%LINK%%[[#^8wl5ujorci|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^8wl5ujorci


>%%
>```annotation-json
>{"created":"2024-04-02T19:59:19.521Z","updated":"2024-04-02T19:59:19.521Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":204,"end":412},{"type":"TextQuoteSelector","exact":" We define inter-operator paral-lelism as the orthogonal class of approaches that do not per-form operator partitioning, but instead, assign different opera-tors of the graph to execute on distributed devices","prefix":"ices.Inter-operator parallelism.","suffix":".Fig. 2d illustrates the batch-s"}]}]}
>```
>%%
>*%%PREFIX%%ices.Inter-operator parallelism.%%HIGHLIGHT%% ==We define inter-operator paral-lelism as the orthogonal class of approaches that do not per-form operator partitioning, but instead, assign different opera-tors of the graph to execute on distributed devices== %%POSTFIX%%.Fig. 2d illustrates the batch-s*
>%%LINK%%[[#^7jhr9z62z2u|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^7jhr9z62z2u


>%%
>```annotation-json
>{"created":"2024-04-02T19:59:48.717Z","updated":"2024-04-02T19:59:48.717Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":1972,"end":2158},{"type":"TextQuoteSelector","exact":" At the intra-op level,Alpa minimizes the cost of executing a stage (i.e., subgraph)of the computational graph, with respect to its intra-operatorparallelism plan, on a given device mesh","prefix":"tra-op and inter-op parallelism.","suffix":", which is a set ofdevices that "}]}]}
>```
>%%
>*%%PREFIX%%tra-op and inter-op parallelism.%%HIGHLIGHT%% ==At the intra-op level,Alpa minimizes the cost of executing a stage (i.e., subgraph)of the computational graph, with respect to its intra-operatorparallelism plan, on a given device mesh== %%POSTFIX%%, which is a set ofdevices that*
>%%LINK%%[[#^rsslg917ova|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^rsslg917ova


>%%
>```annotation-json
>{"created":"2024-04-02T19:59:57.976Z","updated":"2024-04-02T19:59:57.976Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":2370,"end":2570},{"type":"TextQuoteSelector","exact":"At the inter-op level, Alpa minimizes theinter-op parallelization latency, with respect to how to slicethe model and device cluster into stages and device meshesand how to map them as stage-mesh pairs","prefix":"ording to theworkload assigned. ","suffix":". The inter-op op-timization dep"}]}]}
>```
>%%
>*%%PREFIX%%ording to theworkload assigned.%%HIGHLIGHT%% ==At the inter-op level, Alpa minimizes theinter-op parallelization latency, with respect to how to slicethe model and device cluster into stages and device meshesand how to map them as stage-mesh pairs== %%POSTFIX%%. The inter-op op-timization dep*
>%%LINK%%[[#^ue0ml5k4d8b|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^ue0ml5k4d8b


>%%
>```annotation-json
>{"created":"2024-04-02T20:30:49.074Z","updated":"2024-04-02T20:30:49.074Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":1848,"end":1939},{"type":"TextQuoteSelector","exact":"partitions operators evenly across devices andexecutes the same instructions on all devices","prefix":"ra-op parallelism[31, 57] which ","suffix":", as per the factthat devices wi"}]}]}
>```
>%%
>*%%PREFIX%%ra-op parallelism[31, 57] which%%HIGHLIGHT%% ==partitions operators evenly across devices andexecutes the same instructions on all devices== %%POSTFIX%%, as per the factthat devices wi*
>%%LINK%%[[#^8vmdmkkn519|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^8vmdmkkn519


>%%
>```annotation-json
>{"created":"2024-04-02T20:31:03.748Z","updated":"2024-04-02T20:31:03.748Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":899,"end":1013},{"type":"TextQuoteSelector","exact":". Our optimization goalis to minimize the end-to-end pipeline execution latency forthe entire computational graph.","prefix":"ce cluster into stage-mesh pairs","suffix":" Previous works [17, 33] havecon"}]}]}
>```
>%%
>*%%PREFIX%%ce cluster into stage-mesh pairs%%HIGHLIGHT%% ==. Our optimization goalis to minimize the end-to-end pipeline execution latency forthe entire computational graph.== %%POSTFIX%%Previous works [17, 33] havecon*
>%%LINK%%[[#^3kdl1uts0wf|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^3kdl1uts0wf


>%%
>```annotation-json
>{"created":"2024-04-02T21:11:17.772Z","updated":"2024-04-02T21:11:17.772Z","document":{"title":"","link":[{"href":"urn:x-pdf:0dd0806989cfe7a43612f3ef9e2d50c5"},{"href":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf"}],"documentFingerprint":"0dd0806989cfe7a43612f3ef9e2d50c5"},"uri":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","target":[{"source":"vault:/Paper Critiques/Paper7/osdi22-zheng-lianmin.pdf","selector":[{"type":"TextPositionSelector","start":21222,"end":22201},{"type":"TextQuoteSelector","exact":" Alpa implements three novel compilationpasses as Fig. 3 shows. Given a model description, in theform of a Jax [9] intermediate representation (IR), and a clus-ter configuration, the inter-op compilation pass slices the IRinto a number of stages, and slices the device cluster into anumber of device meshes. The inter-op pass uses a DynamicProgramming (DP) algorithm to assign stages to meshes andinvokes the intra-op compilation pass on each stage-mesh pair,to query the execution cost of this assignment. Once invoked,the intra-op pass optimizes the intra-op parallel executionplan of the stage running on its assigned mesh, by minimizingits execution cost using an Integer Linear Programming (ILP)formulation, and reports the cost back to the inter-op pass. Byrepeatedly querying the intra-op pass for each allocation ofa stage-mesh pair, the inter-op pass uses the DP to minimizethe inter-op parallel execution latency and obtains the bestslicing scheme of stages and meshes.","prefix":"f the hierarchy.To achieve this,","suffix":"Given the output hierarchical pl"}]}]}
>```
>%%
>*%%PREFIX%%f the hierarchy.To achieve this,%%HIGHLIGHT%% ==Alpa implements three novel compilationpasses as Fig. 3 shows. Given a model description, in theform of a Jax [9] intermediate representation (IR), and a clus-ter configuration, the inter-op compilation pass slices the IRinto a number of stages, and slices the device cluster into anumber of device meshes. The inter-op pass uses a DynamicProgramming (DP) algorithm to assign stages to meshes andinvokes the intra-op compilation pass on each stage-mesh pair,to query the execution cost of this assignment. Once invoked,the intra-op pass optimizes the intra-op parallel executionplan of the stage running on its assigned mesh, by minimizingits execution cost using an Integer Linear Programming (ILP)formulation, and reports the cost back to the inter-op pass. Byrepeatedly querying the intra-op pass for each allocation ofa stage-mesh pair, the inter-op pass uses the DP to minimizethe inter-op parallel execution latency and obtains the bestslicing scheme of stages and meshes.== %%POSTFIX%%Given the output hierarchical pl*
>%%LINK%%[[#^2vygvt9ez4z|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^2vygvt9ez4z
