---
annotation-target: Paper Critiques/Paper5/MegatronLM.pdf
annotation-target-type: pdf
---


>%%
>```annotation-json
>{"created":"2024-02-26T16:40:02.113Z","updated":"2024-02-26T16:40:02.113Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","target":[{"source":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","selector":[{"type":"TextPositionSelector","start":453,"end":662},{"type":"TextQuoteSelector","exact":"we present our techniques for train-ing very large transformer models and implementa simple, efficient intra-layer model parallel ap-proach that enables training transformer modelswith billions of parameters. ","prefix":"emory constraints.In this work, ","suffix":"Our approach doesnot require a n"}]}]}
>```
>%%
>*%%PREFIX%%emory constraints.In this work,%%HIGHLIGHT%% ==we present our techniques for train-ing very large transformer models and implementa simple, efficient intra-layer model parallel ap-proach that enables training transformer modelswith billions of parameters.== %%POSTFIX%%Our approach doesnot require a n*
>%%LINK%%[[#^1ezj7zfotul|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^1ezj7zfotul


>%%
>```annotation-json
>{"created":"2024-02-26T16:40:04.732Z","text":"The paper introduces methods to train large transformer models using intra-later model parallelism. The methods introduced does not require compiler or pipeline changes, rather it can be implemented through the insertion of a few communication operations in PyTorch.\n\nThe paper also shows that external parameters such as placement of layer normalization affects performance.\n\nThe paper also scales existing model sizes after playing around with the above hyperparams, and showcases SOTA results on datasets","updated":"2024-02-26T16:40:04.732Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^pxkw6x7uv7b|show annotation]]
>%%COMMENT%%
>The paper introduces methods to train large transformer models using intra-later model parallelism. The methods introduced does not require compiler or pipeline changes, rather it can be implemented through the insertion of a few communication operations in PyTorch.
>
>The paper also shows that external parameters such as placement of layer normalization affects performance.
>
>The paper also scales existing model sizes after playing around with the above hyperparams, and showcases SOTA results on datasets
>%%TAGS%%
>#Abstract
^pxkw6x7uv7b


>%%
>```annotation-json
>{"created":"2024-02-26T16:47:26.689Z","text":"- What communication operations are being inserted? Compiler level? Specialized HW level? Is there hardware?\n- What's the innovation that allows it to sustain compute efficiency with GPUs?\n","updated":"2024-02-26T16:47:26.689Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^wzz9jnsml4|show annotation]]
>%%COMMENT%%
>- What communication operations are being inserted? Compiler level? Specialized HW level? Is there hardware?
>- What's the innovation that allows it to sustain compute efficiency with GPUs?
>
>%%TAGS%%
>#qns
^wzz9jnsml4


>%%
>```annotation-json
>{"created":"2024-02-26T16:49:37.074Z","updated":"2024-02-26T16:49:37.074Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","target":[{"source":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","selector":[{"type":"TextPositionSelector","start":2880,"end":2925},{"type":"TextQuoteSelector","exact":"require additional memorymanagement technique","prefix":"limit of modern processors, and ","suffix":"s such as activation checkpointi"}]}]}
>```
>%%
>*%%PREFIX%%limit of modern processors, and%%HIGHLIGHT%% ==require additional memorymanagement technique== %%POSTFIX%%s such as activation checkpointi*
>%%LINK%%[[#^820irsmamik|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^820irsmamik


>%%
>```annotation-json
>{"created":"2024-02-26T16:49:53.770Z","updated":"2024-02-26T16:49:53.770Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","target":[{"source":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","selector":[{"type":"TextPositionSelector","start":3238,"end":3371},{"type":"TextQuoteSelector","exact":"partitioning the model such that the weights and their asso-ciated optimizer state do not need to reside concurrently onthe processor","prefix":"rallelism overcome this limit by","suffix":". For example, GPipe (Huang et a"}]}]}
>```
>%%
>*%%PREFIX%%rallelism overcome this limit by%%HIGHLIGHT%% ==partitioning the model such that the weights and their asso-ciated optimizer state do not need to reside concurrently onthe processor== %%POSTFIX%%. For example, GPipe (Huang et a*
>%%LINK%%[[#^pfbrvt1kgmf|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^pfbrvt1kgmf


>%%
>```annotation-json
>{"created":"2024-02-26T16:50:08.233Z","text":"if i was to optimise transformers:\n- matrix multiplication to generate Q and K can be parallelised\n- subsequent Q and K multiplication can also be parallelised\n- Multiple attention heads, can also be parallelised\n\nWhat about intra layer?\n- QKV calculation parallelised?","updated":"2024-02-26T16:50:08.233Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^f6ltfmfelsv|show annotation]]
>%%COMMENT%%
>if i was to optimise transformers:
>- matrix multiplication to generate Q and K can be parallelised
>- subsequent Q and K multiplication can also be parallelised
>- Multiple attention heads, can also be parallelised
>
>What about intra layer?
>- QKV calculation parallelised?
>%%TAGS%%
>
^f6ltfmfelsv


>%%
>```annotation-json
>{"created":"2024-02-26T16:53:46.523Z","updated":"2024-02-26T16:53:46.523Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","target":[{"source":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","selector":[{"type":"TextPositionSelector","start":5416,"end":5455},{"type":"TextQuoteSelector","exact":"model degradation as the size increases","prefix":"ing BERT architectureresults in ","suffix":". We over-come this challenge by"}]}]}
>```
>%%
>*%%PREFIX%%ing BERT architectureresults in%%HIGHLIGHT%% ==model degradation as the size increases== %%POSTFIX%%. We over-come this challenge by*
>%%LINK%%[[#^wldtipaxis|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^wldtipaxis


>%%
>```annotation-json
>{"created":"2024-02-26T16:53:50.423Z","updated":"2024-02-26T16:53:50.423Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","target":[{"source":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","selector":[{"type":"TextPositionSelector","start":5457,"end":5602},{"type":"TextQuoteSelector","exact":"We over-come this challenge by rearranging the layer normalizationand residual connection in the transformer layers and showthat with this change","prefix":"radation as the size increases. ","suffix":", results for the downstream tas"}]}]}
>```
>%%
>*%%PREFIX%%radation as the size increases.%%HIGHLIGHT%% ==We over-come this challenge by rearranging the layer normalizationand residual connection in the transformer layers and showthat with this change== %%POSTFIX%%, results for the downstream tas*
>%%LINK%%[[#^ndrq5lh3va|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^ndrq5lh3va


>%%
>```annotation-json
>{"created":"2024-02-26T17:00:26.295Z","updated":"2024-02-26T17:00:26.295Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","target":[{"source":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","selector":[{"type":"TextPositionSelector","start":10173,"end":10227},{"type":"TextQuoteSelector","exact":" a training minibatchis split across multiple workers,","prefix":"arallelism (Valiant, 1990) where","suffix":" and model parallelism inwhich t"}]}]}
>```
>%%
>*%%PREFIX%%arallelism (Valiant, 1990) where%%HIGHLIGHT%% ==a training minibatchis split across multiple workers,== %%POSTFIX%%and model parallelism inwhich t*
>%%LINK%%[[#^8tdw78a39gb|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^8tdw78a39gb


>%%
>```annotation-json
>{"created":"2024-02-26T17:00:37.266Z","updated":"2024-02-26T17:00:37.266Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","target":[{"source":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","selector":[{"type":"TextPositionSelector","start":10341,"end":10507},{"type":"TextQuoteSelector","exact":"By increasing the mini-batch size proportionally to the number of available work-ers (i.e. weak scaling), one observes near linear scalingin training data throughput.","prefix":"ibuted across multiple workers. ","suffix":" However, large batch train-ing "}]}]}
>```
>%%
>*%%PREFIX%%ibuted across multiple workers.%%HIGHLIGHT%% ==By increasing the mini-batch size proportionally to the number of available work-ers (i.e. weak scaling), one observes near linear scalingin training data throughput.== %%POSTFIX%%However, large batch train-ing*
>%%LINK%%[[#^4zsnnjgfu49|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^4zsnnjgfu49


>%%
>```annotation-json
>{"created":"2024-02-26T17:01:00.928Z","updated":"2024-02-26T17:01:00.928Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","target":[{"source":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","selector":[{"type":"TextPositionSelector","start":11013,"end":11152},{"type":"TextQuoteSelector","exact":"activation checkpointing: recomputing activations in thebackward pass without storing them in the forward pass toreduce memory requirements","prefix":"s combined data parallelism with","suffix":".However, these techniques have "}]}]}
>```
>%%
>*%%PREFIX%%s combined data parallelism with%%HIGHLIGHT%% ==activation checkpointing: recomputing activations in thebackward pass without storing them in the forward pass toreduce memory requirements== %%POSTFIX%%.However, these techniques have*
>%%LINK%%[[#^wnzfymgaick|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^wnzfymgaick


>%%
>```annotation-json
>{"created":"2024-02-26T17:02:30.523Z","text":"The approach is to look at each compute, and parallelise","updated":"2024-02-26T17:02:30.523Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","target":[{"source":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","selector":[{"type":"TextPositionSelector","start":14487,"end":14583},{"type":"TextQuoteSelector","exact":"parallelize the GEMM is to split the weightmatrix A along its rows and input X along its columns","prefix":"y:Y = GeLU(XA) (1)One option to ","suffix":" as:X = [X1,X2], A =[A1A2]. (2)T"}]}]}
>```
>%%
>*%%PREFIX%%y:Y = GeLU(XA) (1)One option to%%HIGHLIGHT%% ==parallelize the GEMM is to split the weightmatrix A along its rows and input X along its columns== %%POSTFIX%%as:X = [X1,X2], A =[A1A2]. (2)T*
>%%LINK%%[[#^h369a6b0wm|show annotation]]
>%%COMMENT%%
>The approach is to look at each compute, and parallelise
>%%TAGS%%
>
^h369a6b0wm


>%%
>```annotation-json
>{"created":"2024-02-26T17:03:35.646Z","updated":"2024-02-26T17:03:35.646Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","target":[{"source":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","selector":[{"type":"TextPositionSelector","start":15101,"end":15306},{"type":"TextQuoteSelector","exact":"we partition the first GEMM in this column parallelfashion and split the second GEMM along its rows so it takesthe output of the GeLU layer directly without requiring anycommunication as shown in Figure 3a","prefix":" a synchronization point.Hence, ","suffix":". The output of thesecond GEMM i"}]}]}
>```
>%%
>*%%PREFIX%%a synchronization point.Hence,%%HIGHLIGHT%% ==we partition the first GEMM in this column parallelfashion and split the second GEMM along its rows so it takesthe output of the GeLU layer directly without requiring anycommunication as shown in Figure 3a== %%POSTFIX%%. The output of thesecond GEMM i*
>%%LINK%%[[#^tvebivcorws|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^tvebivcorws


>%%
>```annotation-json
>{"created":"2024-02-26T17:04:27.644Z","updated":"2024-02-26T17:04:27.644Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","target":[{"source":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","selector":[{"type":"TextPositionSelector","start":16424,"end":16619},{"type":"TextQuoteSelector","exact":"partitioning the GEMMs associated with key (K), query(Q), and value (V ) in a column parallel fashion such thatthe matrix multiply corresponding to each attention head isdone locally on one GPU. ","prefix":"e multihead attention operation,","suffix":"This allows us to split per atte"}]}]}
>```
>%%
>*%%PREFIX%%e multihead attention operation,%%HIGHLIGHT%% ==partitioning the GEMMs associated with key (K), query(Q), and value (V ) in a column parallel fashion such thatthe matrix multiply corresponding to each attention head isdone locally on one GPU.== %%POSTFIX%%This allows us to split per atte*
>%%LINK%%[[#^k5hapks902n|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^k5hapks902n


>%%
>```annotation-json
>{"created":"2024-02-26T17:04:49.640Z","updated":"2024-02-26T17:04:49.640Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","target":[{"source":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","selector":[{"type":"TextPositionSelector","start":16805,"end":16995},{"type":"TextQuoteSelector","exact":" the outputlinear layer (after self attention) is parallelized along itsrows and takes the output of the parallel attention layer di-rectly, without requiring communication between the GPUs.","prefix":"ention. The subsequent GEMM from","suffix":"This approach for both the MLP a"}]}]}
>```
>%%
>*%%PREFIX%%ention. The subsequent GEMM from%%HIGHLIGHT%% ==the outputlinear layer (after self attention) is parallelized along itsrows and takes the output of the parallel attention layer di-rectly, without requiring communication between the GPUs.== %%POSTFIX%%This approach for both the MLP a*
>%%LINK%%[[#^yjcmdl3a7|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^yjcmdl3a7


>%%
>```annotation-json
>{"created":"2024-02-26T17:05:33.349Z","text":"## Parellisation of GEMM\n- splits weights along column\n- splits activation along rows","updated":"2024-02-26T17:05:33.349Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^bzpnv66tryt|show annotation]]
>%%COMMENT%%
>## Parellisation of GEMM
>- splits weights along column
>- splits activation along rows
>%%TAGS%%
>
^bzpnv66tryt


>%%
>```annotation-json
>{"created":"2024-02-26T17:21:17.047Z","updated":"2024-02-26T17:21:17.047Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","target":[{"source":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","selector":[{"type":"TextPositionSelector","start":19103,"end":19293},{"type":"TextQuoteSelector","exact":" Rather than having one GPUcompute part of the dropout, layer normalization, or residualconnections and broadcast the results to other GPUs, wechoose to duplicate the computation across GPUs","prefix":"keep-ing the GPUs compute bound.","suffix":". Specifi-cally, we maintain dup"}]}]}
>```
>%%
>*%%PREFIX%%keep-ing the GPUs compute bound.%%HIGHLIGHT%% ==Rather than having one GPUcompute part of the dropout, layer normalization, or residualconnections and broadcast the results to other GPUs, wechoose to duplicate the computation across GPUs== %%POSTFIX%%. Specifi-cally, we maintain dup*
>%%LINK%%[[#^g4891gb1ej|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^g4891gb1ej


>%%
>```annotation-json
>{"created":"2024-02-26T17:21:26.445Z","updated":"2024-02-26T17:21:26.445Z","document":{"title":"Megatron-LM: Training Multi-Billion Parameter Language Models Using Model Parallelism","link":[{"href":"urn:x-pdf:be2eea8cb47b938c67107a4c6fe461a4"},{"href":"vault:/Paper Critiques/Paper5/MegatronLM.pdf"}],"documentFingerprint":"be2eea8cb47b938c67107a4c6fe461a4"},"uri":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","target":[{"source":"vault:/Paper Critiques/Paper5/MegatronLM.pdf","selector":[{"type":"TextPositionSelector","start":19322,"end":19551},{"type":"TextQuoteSelector","exact":"duplicate copies of layer normalizationparameters on each GPU, and take the output of the modelparallel region and run dropout and residual connectionon these tensors before feeding them as input to the nextmodel parallel regions","prefix":"PUs. Specifi-cally, we maintain ","suffix":". To optimize the model we allow"}]}]}
>```
>%%
>*%%PREFIX%%PUs. Specifi-cally, we maintain%%HIGHLIGHT%% ==duplicate copies of layer normalizationparameters on each GPU, and take the output of the modelparallel region and run dropout and residual connectionon these tensors before feeding them as input to the nextmodel parallel regions== %%POSTFIX%%. To optimize the model we allow*
>%%LINK%%[[#^svlroy9i89r|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^svlroy9i89r
