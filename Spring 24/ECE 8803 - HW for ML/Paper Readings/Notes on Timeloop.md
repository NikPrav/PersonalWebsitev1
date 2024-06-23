---
annotation-target: Paper Readings/02_06_timeloop.pdf
annotation-target-type: pdf
---


>%%
>```annotation-json
>{"created":"2024-02-06T16:24:14.609Z","updated":"2024-02-06T16:24:14.609Z","document":{"title":"Timeloop: A Systematic Approach to DNN Accelerator Evaluation","link":[{"href":"urn:x-pdf:1203291ae20ed6dd78655fc430d376f6"},{"href":"vault:/Paper Readings/02_06_timeloop.pdf"}],"documentFingerprint":"1203291ae20ed6dd78655fc430d376f6"},"uri":"vault:/Paper Readings/02_06_timeloop.pdf","target":[{"source":"vault:/Paper Readings/02_06_timeloop.pdf","selector":[{"type":"TextPositionSelector","start":359,"end":455},{"type":"TextQuoteSelector","exact":"evaluating and exploring the architecture design space of deepneural network (DNN) accelerators.","prefix":" Timeloop, an infrastructure for","suffix":" Timeloop uses a concise andunif"}]}]}
>```
>%%
>*%%PREFIX%%Timeloop, an infrastructure for%%HIGHLIGHT%% ==evaluating and exploring the architecture design space of deepneural network (DNN) accelerators.== %%POSTFIX%%Timeloop uses a concise andunif*
>%%LINK%%[[#^biknz5l5ud|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^biknz5l5ud


>%%
>```annotation-json
>{"created":"2024-02-06T16:24:32.168Z","updated":"2024-02-06T16:24:32.168Z","document":{"title":"Timeloop: A Systematic Approach to DNN Accelerator Evaluation","link":[{"href":"urn:x-pdf:1203291ae20ed6dd78655fc430d376f6"},{"href":"vault:/Paper Readings/02_06_timeloop.pdf"}],"documentFingerprint":"1203291ae20ed6dd78655fc430d376f6"},"uri":"vault:/Paper Readings/02_06_timeloop.pdf","target":[{"source":"vault:/Paper Readings/02_06_timeloop.pdf","selector":[{"type":"TextPositionSelector","start":628,"end":862},{"type":"TextQuoteSelector","exact":"It can then emulate those topologies togenerate an accurate projection of performance and energyefficiency for a DNN workload through a mapper that finds thebest way to schedule operations and stage data on the specifiedarchitecture. ","prefix":"ad space ofhardware topologies. ","suffix":"This enables fair comparisons ac"}]}]}
>```
>%%
>*%%PREFIX%%ad space ofhardware topologies.%%HIGHLIGHT%% ==It can then emulate those topologies togenerate an accurate projection of performance and energyefficiency for a DNN workload through a mapper that finds thebest way to schedule operations and stage data on the specifiedarchitecture.== %%POSTFIX%%This enables fair comparisons ac*
>%%LINK%%[[#^ifpvfwb52qb|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^ifpvfwb52qb


>%%
>```annotation-json
>{"created":"2024-02-06T16:29:33.841Z","text":"Timeloop evaluates architectural design space of deep neural network accelerators, and is able to generate an accurate projection of performance and energy efficiency","updated":"2024-02-06T16:29:33.841Z","document":{"title":"Timeloop: A Systematic Approach to DNN Accelerator Evaluation","link":[{"href":"urn:x-pdf:1203291ae20ed6dd78655fc430d376f6"},{"href":"vault:/Paper Readings/02_06_timeloop.pdf"}],"documentFingerprint":"1203291ae20ed6dd78655fc430d376f6"},"uri":"vault:/Paper Readings/02_06_timeloop.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^bokwksgev9n|show annotation]]
>%%COMMENT%%
>Timeloop evaluates architectural design space of deep neural network accelerators, and is able to generate an accurate projection of performance and energy efficiency
>%%TAGS%%
>#Abstract
^bokwksgev9n


>%%
>```annotation-json
>{"created":"2024-02-06T16:30:45.727Z","text":"- How does it model architecture?\n- How does it model a DNN?\n- How does it optimise?","updated":"2024-02-06T16:30:45.727Z","document":{"title":"Timeloop: A Systematic Approach to DNN Accelerator Evaluation","link":[{"href":"urn:x-pdf:1203291ae20ed6dd78655fc430d376f6"},{"href":"vault:/Paper Readings/02_06_timeloop.pdf"}],"documentFingerprint":"1203291ae20ed6dd78655fc430d376f6"},"uri":"vault:/Paper Readings/02_06_timeloop.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^91gd008kixs|show annotation]]
>%%COMMENT%%
>- How does it model architecture?
>- How does it model a DNN?
>- How does it optimise?
>%%TAGS%%
>#qns
^91gd008kixs


>%%
>```annotation-json
>{"created":"2024-02-06T16:32:23.254Z","text":"how does it differentiate between different dataflows? is it a classification problem b/w different flows, or does it become somehow become a regression problem?\n","updated":"2024-02-06T16:32:23.254Z","document":{"title":"Timeloop: A Systematic Approach to DNN Accelerator Evaluation","link":[{"href":"urn:x-pdf:1203291ae20ed6dd78655fc430d376f6"},{"href":"vault:/Paper Readings/02_06_timeloop.pdf"}],"documentFingerprint":"1203291ae20ed6dd78655fc430d376f6"},"uri":"vault:/Paper Readings/02_06_timeloop.pdf","target":[{"source":"vault:/Paper Readings/02_06_timeloop.pdf","selector":[{"type":"TextPositionSelector","start":1188,"end":1312},{"type":"TextQuoteSelector","exact":"In particular, they reveal that dataflow andmemory hierarchy co-design plays a critical role in optimizingenergy efficiency.","prefix":"tate of DNNarchitecture design. ","suffix":" Also, there is currently still "}]}]}
>```
>%%
>*%%PREFIX%%tate of DNNarchitecture design.%%HIGHLIGHT%% ==In particular, they reveal that dataflow andmemory hierarchy co-design plays a critical role in optimizingenergy efficiency.== %%POSTFIX%%Also, there is currently still*
>%%LINK%%[[#^rghnyn28qb|show annotation]]
>%%COMMENT%%
>how does it differentiate between different dataflows? is it a classification problem b/w different flows, or does it become somehow become a regression problem?
>
>%%TAGS%%
>
^rghnyn28qb


>%%
>```annotation-json
>{"created":"2024-02-06T16:33:26.787Z","text":"this sounds like the paper does classifcation over a state space search. Why does it need ML? It would be interesting to see whether it becomes a regression problem\n","updated":"2024-02-06T16:33:26.787Z","document":{"title":"Timeloop: A Systematic Approach to DNN Accelerator Evaluation","link":[{"href":"urn:x-pdf:1203291ae20ed6dd78655fc430d376f6"},{"href":"vault:/Paper Readings/02_06_timeloop.pdf"}],"documentFingerprint":"1203291ae20ed6dd78655fc430d376f6"},"uri":"vault:/Paper Readings/02_06_timeloop.pdf","target":[{"source":"vault:/Paper Readings/02_06_timeloop.pdf","selector":[{"type":"TextPositionSelector","start":1313,"end":1590},{"type":"TextQuoteSelector","exact":"Also, there is currently still not a singlearchitecture that achieves the best performance and energyefficiency across a diverse set of workloads due to flexibilityand efficiency trade-offs. These results provide inspiration intopossible directions for DNN accelerator research","prefix":"in optimizingenergy efficiency. ","suffix":".Index Terms—modeling; accelerat"}]}]}
>```
>%%
>*%%PREFIX%%in optimizingenergy efficiency.%%HIGHLIGHT%% ==Also, there is currently still not a singlearchitecture that achieves the best performance and energyefficiency across a diverse set of workloads due to flexibilityand efficiency trade-offs. These results provide inspiration intopossible directions for DNN accelerator research== %%POSTFIX%%.Index Terms—modeling; accelerat*
>%%LINK%%[[#^to0mlznyuls|show annotation]]
>%%COMMENT%%
>this sounds like the paper does classifcation over a state space search. Why does it need ML? It would be interesting to see whether it becomes a regression problem
>
>%%TAGS%%
>
^to0mlznyuls


>%%
>```annotation-json
>{"created":"2024-02-06T16:34:38.916Z","text":"How do we distinguish b/w different mappings using numbers? The time it takes or the memory movement vs compute flow? How is parallelisation handled?","updated":"2024-02-06T16:34:38.916Z","document":{"title":"Timeloop: A Systematic Approach to DNN Accelerator Evaluation","link":[{"href":"urn:x-pdf:1203291ae20ed6dd78655fc430d376f6"},{"href":"vault:/Paper Readings/02_06_timeloop.pdf"}],"documentFingerprint":"1203291ae20ed6dd78655fc430d376f6"},"uri":"vault:/Paper Readings/02_06_timeloop.pdf","target":[{"source":"vault:/Paper Readings/02_06_timeloop.pdf","selector":[{"type":"TextPositionSelector","start":2912,"end":3067},{"type":"TextQuoteSelector","exact":"a flexible architecture may permit manydifferent ways of scheduling operations and staging data onthe same architecture, which we call different mappings [","prefix":"ven DNNlayer, i.e., a workload, ","suffix":"7],resulting in widely varying p"}]}]}
>```
>%%
>*%%PREFIX%%ven DNNlayer, i.e., a workload,%%HIGHLIGHT%% ==a flexible architecture may permit manydifferent ways of scheduling operations and staging data onthe same architecture, which we call different mappings [== %%POSTFIX%%7],resulting in widely varying p*
>%%LINK%%[[#^2i6hdqu2g0c|show annotation]]
>%%COMMENT%%
>How do we distinguish b/w different mappings using numbers? The time it takes or the memory movement vs compute flow? How is parallelisation handled?
>%%TAGS%%
>
^2i6hdqu2g0c


>%%
>```annotation-json
>{"created":"2024-02-06T16:35:34.607Z","text":"Classification problem?\n","updated":"2024-02-06T16:35:34.607Z","document":{"title":"Timeloop: A Systematic Approach to DNN Accelerator Evaluation","link":[{"href":"urn:x-pdf:1203291ae20ed6dd78655fc430d376f6"},{"href":"vault:/Paper Readings/02_06_timeloop.pdf"}],"documentFingerprint":"1203291ae20ed6dd78655fc430d376f6"},"uri":"vault:/Paper Readings/02_06_timeloop.pdf","target":[{"source":"vault:/Paper Readings/02_06_timeloop.pdf","selector":[{"type":"TextPositionSelector","start":3164,"end":3285},{"type":"TextQuoteSelector","exact":" search for a good mappingwithin the space of valid mappings, i.e., the mapspace, to fairlycharacterize the architecture.","prefix":"This results in a requirement to","suffix":" The need to do this search fore"}]}]}
>```
>%%
>*%%PREFIX%%This results in a requirement to%%HIGHLIGHT%% ==search for a good mappingwithin the space of valid mappings, i.e., the mapspace, to fairlycharacterize the architecture.== %%POSTFIX%%The need to do this search fore*
>%%LINK%%[[#^8py4gik14hm|show annotation]]
>%%COMMENT%%
>Classification problem?
>
>%%TAGS%%
>
^8py4gik14hm


>%%
>```annotation-json
>{"created":"2024-02-06T16:44:20.959Z","updated":"2024-02-06T16:44:20.959Z","document":{"title":"Timeloop: A Systematic Approach to DNN Accelerator Evaluation","link":[{"href":"urn:x-pdf:1203291ae20ed6dd78655fc430d376f6"},{"href":"vault:/Paper Readings/02_06_timeloop.pdf"}],"documentFingerprint":"1203291ae20ed6dd78655fc430d376f6"},"uri":"vault:/Paper Readings/02_06_timeloop.pdf","target":[{"source":"vault:/Paper Readings/02_06_timeloop.pdf","selector":[{"type":"TextPositionSelector","start":5215,"end":5365},{"type":"TextQuoteSelector","exact":"Timeloop provides a concise and unified way of de-scribing the key attributes of a diverse class of DNNarchitectures and their implementation features","prefix":" following key contributions:1) ","suffix":" as the3042019 IEEE Internationa"}]}]}
>```
>%%
>*%%PREFIX%%following key contributions:1)%%HIGHLIGHT%% ==Timeloop provides a concise and unified way of de-scribing the key attributes of a diverse class of DNNarchitectures and their implementation features== %%POSTFIX%%as the3042019 IEEE Internationa*
>%%LINK%%[[#^8jmztnptcvg|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^8jmztnptcvg


>%%
>```annotation-json
>{"created":"2024-02-06T16:44:28.696Z","text":"What is mapping? How does the mapping differ from a CPU, GPU and a TPU?\n","updated":"2024-02-06T16:44:28.696Z","document":{"title":"Timeloop: A Systematic Approach to DNN Accelerator Evaluation","link":[{"href":"urn:x-pdf:1203291ae20ed6dd78655fc430d376f6"},{"href":"vault:/Paper Readings/02_06_timeloop.pdf"}],"documentFingerprint":"1203291ae20ed6dd78655fc430d376f6"},"uri":"vault:/Paper Readings/02_06_timeloop.pdf","target":[{"source":"vault:/Paper Readings/02_06_timeloop.pdf","selector":[{"type":"TextPositionSelector","start":5801,"end":6001},{"type":"TextQuoteSelector","exact":"Timeloop is the first infrastructure to effectively combinethe exploration of a large design space with a mapperthat allows for finding the optimal mapping of anyworkload on the targeted architecture.","prefix":" wide range of architectures.2) ","suffix":" This enables faircomparisons be"}]}]}
>```
>%%
>*%%PREFIX%%wide range of architectures.2)%%HIGHLIGHT%% ==Timeloop is the first infrastructure to effectively combinethe exploration of a large design space with a mapperthat allows for finding the optimal mapping of anyworkload on the targeted architecture.== %%POSTFIX%%This enables faircomparisons be*
>%%LINK%%[[#^4bcldw2yczc|show annotation]]
>%%COMMENT%%
>What is mapping? How does the mapping differ from a CPU, GPU and a TPU?
>
>%%TAGS%%
>
^4bcldw2yczc


>%%
>```annotation-json
>{"created":"2024-02-06T16:45:36.380Z","text":"Similar to eyeriss?","updated":"2024-02-06T16:45:36.380Z","document":{"title":"Timeloop: A Systematic Approach to DNN Accelerator Evaluation","link":[{"href":"urn:x-pdf:1203291ae20ed6dd78655fc430d376f6"},{"href":"vault:/Paper Readings/02_06_timeloop.pdf"}],"documentFingerprint":"1203291ae20ed6dd78655fc430d376f6"},"uri":"vault:/Paper Readings/02_06_timeloop.pdf","target":[{"source":"vault:/Paper Readings/02_06_timeloop.pdf","selector":[{"type":"TextPositionSelector","start":52621,"end":52695},{"type":"TextQuoteSelector","exact":"comprehensively describe mappings us-ing a loop-nest-style representation,","prefix":"ds such asconvolutional layers, ","suffix":" and efficiently enumeratethe sp"}]}]}
>```
>%%
>*%%PREFIX%%ds such asconvolutional layers,%%HIGHLIGHT%% ==comprehensively describe mappings us-ing a loop-nest-style representation,== %%POSTFIX%%and efficiently enumeratethe sp*
>%%LINK%%[[#^fmyy3ld9xij|show annotation]]
>%%COMMENT%%
>Similar to eyeriss?
>%%TAGS%%
>
^fmyy3ld9xij


>%%
>```annotation-json
>{"created":"2024-02-06T16:45:56.211Z","text":"Loop over search space?\n","updated":"2024-02-06T16:45:56.211Z","document":{"title":"Timeloop: A Systematic Approach to DNN Accelerator Evaluation","link":[{"href":"urn:x-pdf:1203291ae20ed6dd78655fc430d376f6"},{"href":"vault:/Paper Readings/02_06_timeloop.pdf"}],"documentFingerprint":"1203291ae20ed6dd78655fc430d376f6"},"uri":"vault:/Paper Readings/02_06_timeloop.pdf","target":[{"source":"vault:/Paper Readings/02_06_timeloop.pdf","selector":[{"type":"TextPositionSelector","start":52701,"end":52804},{"type":"TextQuoteSelector","exact":"fficiently enumeratethe space of feasible mappings by combining workload andarchitectural constraints. ","prefix":"nest-style representation, and e","suffix":"We also described computationall"}]}]}
>```
>%%
>*%%PREFIX%%nest-style representation, and e%%HIGHLIGHT%% ==fficiently enumeratethe space of feasible mappings by combining workload andarchitectural constraints.== %%POSTFIX%%We also described computationall*
>%%LINK%%[[#^q4kjkeb9rc|show annotation]]
>%%COMMENT%%
>Loop over search space?
>
>%%TAGS%%
>
^q4kjkeb9rc




>%%
>```annotation-json
>{"created":"2024-02-06T16:51:28.054Z","text":"Timeloop can automatically determine mappings given a hardware configuration. How does one specify the HW configuration, does one just walk through all possible scenarios?\n\n","updated":"2024-02-06T16:51:28.054Z","document":{"title":"Timeloop: A Systematic Approach to DNN Accelerator Evaluation","link":[{"href":"urn:x-pdf:1203291ae20ed6dd78655fc430d376f6"},{"href":"vault:/Paper Readings/02_06_timeloop.pdf"}],"documentFingerprint":"1203291ae20ed6dd78655fc430d376f6"},"uri":"vault:/Paper Readings/02_06_timeloop.pdf","target":[{"source":"vault:/Paper Readings/02_06_timeloop.pdf","selector":[{"type":"TextPositionSelector","start":8910,"end":9005},{"type":"TextQuoteSelector","exact":"Section V how Timeloop systematically constructs a mapspaceand walks through the mappings in it","prefix":"v3 2 on an example architecture.","suffix":".A mapper needs a model. A mappe"}]}]}
>```
>%%
>*%%PREFIX%%v3 2 on an example architecture.%%HIGHLIGHT%% ==Section V how Timeloop systematically constructs a mapspaceand walks through the mappings in it== %%POSTFIX%%.A mapper needs a model. A mappe*
>%%LINK%%[[#^hi66yqxqdi|show annotation]]
>%%COMMENT%%
>Timeloop can automatically determine mappings given a hardware configuration. How does one specify the HW configuration, does one just walk through all possible scenarios?
>
>
>%%TAGS%%
>
^hi66yqxqdi
