---
annotation-target: Paper Critiques/Paper3/osdi18-chen.pdf
annotation-target-type: pdf
---


>%%
>```annotation-json
>{"created":"2024-02-05T21:24:28.125Z","updated":"2024-02-05T21:24:28.125Z","document":{"title":"","link":[{"href":"urn:x-pdf:0868c3012f9446e0a477877b725e26cf"},{"href":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf"}],"documentFingerprint":"0868c3012f9446e0a477877b725e26cf"},"uri":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf","target":[{"source":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf","selector":[{"type":"TextPositionSelector","start":1545,"end":1723},{"type":"TextQuoteSelector","exact":"We propose TVM, a compiler that exposes graph-leveland operator-level optimizations to provide performanceportability to deep learning workloads across diversehardware back-ends.","prefix":"uires significant manual effort.","suffix":" TVM solves optimization chal-le"}]}]}
>```
>%%
>*%%PREFIX%%uires significant manual effort.%%HIGHLIGHT%% ==We propose TVM, a compiler that exposes graph-leveland operator-level optimizations to provide performanceportability to deep learning workloads across diversehardware back-ends.== %%POSTFIX%%TVM solves optimization chal-le*
>%%LINK%%[[#^v3a2c33y239|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^v3a2c33y239


>%%
>```annotation-json
>{"created":"2024-02-05T21:24:45.744Z","text":"Whaht is it learning? What is the cost function? Is there a NN?","updated":"2024-02-05T21:24:45.744Z","document":{"title":"","link":[{"href":"urn:x-pdf:0868c3012f9446e0a477877b725e26cf"},{"href":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf"}],"documentFingerprint":"0868c3012f9446e0a477877b725e26cf"},"uri":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf","target":[{"source":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf","selector":[{"type":"TextPositionSelector","start":1899,"end":2074},{"type":"TextQuoteSelector","exact":" automates optimiza-tion of low-level programs to hardware characteristics byemploying a novel, learning-based cost modeling methodfor rapid exploration of code optimizations.","prefix":"d memory latency hiding. It also","suffix":" Experimen-tal results show that"}]}]}
>```
>%%
>*%%PREFIX%%d memory latency hiding. It also%%HIGHLIGHT%% ==automates optimiza-tion of low-level programs to hardware characteristics byemploying a novel, learning-based cost modeling methodfor rapid exploration of code optimizations.== %%POSTFIX%%Experimen-tal results show that*
>%%LINK%%[[#^o2yljvzieht|show annotation]]
>%%COMMENT%%
>Whaht is it learning? What is the cost function? Is there a NN?
>%%TAGS%%
>
^o2yljvzieht


>%%
>```annotation-json
>{"created":"2024-02-05T21:26:25.133Z","text":"TVM is a compiler that can be used to optimize the running of DL Frameworks across a variety of HW. It automates this optimisation through a learning-based cost model.","updated":"2024-02-05T21:26:25.133Z","document":{"title":"","link":[{"href":"urn:x-pdf:0868c3012f9446e0a477877b725e26cf"},{"href":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf"}],"documentFingerprint":"0868c3012f9446e0a477877b725e26cf"},"uri":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^bnpsoa7pyt9|show annotation]]
>%%COMMENT%%
>TVM is a compiler that can be used to optimize the running of DL Frameworks across a variety of HW. It automates this optimisation through a learning-based cost model.
>%%TAGS%%
>
^bnpsoa7pyt9


>%%
>```annotation-json
>{"created":"2024-02-05T21:29:31.919Z","text":"TVM avoids graph optimisations (as employed by popular frameworks such as TensorFlow and PyTorch because they are too high level for hw level optimisation), and instead generates low-level optimized code from the high-level specification of the existing frameworks.","updated":"2024-02-05T21:29:31.919Z","document":{"title":"","link":[{"href":"urn:x-pdf:0868c3012f9446e0a477877b725e26cf"},{"href":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf"}],"documentFingerprint":"0868c3012f9446e0a477877b725e26cf"},"uri":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^p8p2p914g57|show annotation]]
>%%COMMENT%%
>TVM avoids graph optimisations (as employed by popular frameworks such as TensorFlow and PyTorch because they are too high level for hw level optimisation), and instead generates low-level optimized code from the high-level specification of the existing frameworks.
>%%TAGS%%
>#Introduction
^p8p2p914g57


>%%
>```annotation-json
>{"created":"2024-02-05T21:32:22.460Z","updated":"2024-02-05T21:32:22.460Z","document":{"title":"","link":[{"href":"urn:x-pdf:0868c3012f9446e0a477877b725e26cf"},{"href":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf"}],"documentFingerprint":"0868c3012f9446e0a477877b725e26cf"},"uri":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf","target":[{"source":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf","selector":[{"type":"TextPositionSelector","start":4972,"end":5109},{"type":"TextQuoteSelector","exact":"TVMneeds to offer performance competitive with the multi-tude of manually optimized operator libraries across di-verse hardware back-ends","prefix":"nds. To be attractive to users, ","suffix":". This goal requires addressingt"}]}]}
>```
>%%
>*%%PREFIX%%nds. To be attractive to users,%%HIGHLIGHT%% ==TVMneeds to offer performance competitive with the multi-tude of manually optimized operator libraries across di-verse hardware back-ends== %%POSTFIX%%. This goal requires addressingt*
>%%LINK%%[[#^eyrg44v3pf8|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^eyrg44v3pf8


>%%
>```annotation-json
>{"created":"2024-02-05T21:36:40.569Z","text":"- Can it work for any hw specification?\n- How complex of a hw model can it genereate?\n- What all does it account for, does it generate assembly level instructions? Does it account for parallelism, ooo etc?\n- How well can it leverage specific features such a a comples NOC a-la- Tushar Krishna Paper\n- How much can it search?\n- What ML model does it use to optimze searching?\n- How does it model scheduling, threading, memory management and dataflow?(eg: TPU)","updated":"2024-02-05T21:36:40.569Z","document":{"title":"","link":[{"href":"urn:x-pdf:0868c3012f9446e0a477877b725e26cf"},{"href":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf"}],"documentFingerprint":"0868c3012f9446e0a477877b725e26cf"},"uri":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^utyxl2co2ic|show annotation]]
>%%COMMENT%%
>- Can it work for any hw specification?
>- How complex of a hw model can it genereate?
>- What all does it account for, does it generate assembly level instructions? Does it account for parallelism, ooo etc?
>- How well can it leverage specific features such a a comples NOC a-la- Tushar Krishna Paper
>- How much can it search?
>- What ML model does it use to optimze searching?
>- How does it model scheduling, threading, memory management and dataflow?(eg: TPU)
>%%TAGS%%
>#Possible Issues
^utyxl2co2ic


>%%
>```annotation-json
>{"created":"2024-02-05T21:39:17.158Z","updated":"2024-02-05T21:39:17.158Z","document":{"title":"","link":[{"href":"urn:x-pdf:0868c3012f9446e0a477877b725e26cf"},{"href":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf"}],"documentFingerprint":"0868c3012f9446e0a477877b725e26cf"},"uri":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf","target":[{"source":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf","selector":[{"type":"TextPositionSelector","start":5564,"end":5655},{"type":"TextQuoteSelector","exact":"they dictate different data layouts; and they havespecial requirements for memory hierarchy","prefix":" with fixed or variablelengths; ","suffix":". The systemmust effectively exp"}]}]}
>```
>%%
>*%%PREFIX%%with fixed or variablelengths;%%HIGHLIGHT%% ==they dictate different data layouts; and they havespecial requirements for memory hierarchy== %%POSTFIX%%. The systemmust effectively exp*
>%%LINK%%[[#^axb9wsirtz9|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^axb9wsirtz9


>%%
>```annotation-json
>{"created":"2024-02-05T21:40:02.379Z","updated":"2024-02-05T21:40:02.379Z","document":{"title":"","link":[{"href":"urn:x-pdf:0868c3012f9446e0a477877b725e26cf"},{"href":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf"}],"documentFingerprint":"0868c3012f9446e0a477877b725e26cf"},"uri":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf","target":[{"source":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf","selector":[{"type":"TextPositionSelector","start":6799,"end":6965},{"type":"TextQuoteSelector","exact":"tensor expression languageto build operators and provide program transformationprimitives that generate different versions of the pro-gram with various optimizations.","prefix":"ey mod-ules. (1) We introduce a ","suffix":" This layer extendsHalide [32]’s"}]}]}
>```
>%%
>*%%PREFIX%%ey mod-ules. (1) We introduce a%%HIGHLIGHT%% ==tensor expression languageto build operators and provide program transformationprimitives that generate different versions of the pro-gram with various optimizations.== %%POSTFIX%%This layer extendsHalide [32]’s*
>%%LINK%%[[#^afyzzr0h62l|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^afyzzr0h62l


>%%
>```annotation-json
>{"created":"2024-02-05T21:42:58.896Z","text":"Uses *Tensor Expression Language* to describe operations better, and generate different versions of the program","updated":"2024-02-05T21:42:58.896Z","document":{"title":"","link":[{"href":"urn:x-pdf:0868c3012f9446e0a477877b725e26cf"},{"href":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf"}],"documentFingerprint":"0868c3012f9446e0a477877b725e26cf"},"uri":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^9eapg1uimb|show annotation]]
>%%COMMENT%%
>Uses *Tensor Expression Language* to describe operations better, and generate different versions of the program
>%%TAGS%%
>#info
^9eapg1uimb


>%%
>```annotation-json
>{"created":"2024-02-05T22:07:43.022Z","updated":"2024-02-05T22:07:43.022Z","document":{"title":"","link":[{"href":"urn:x-pdf:0868c3012f9446e0a477877b725e26cf"},{"href":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf"}],"documentFingerprint":"0868c3012f9446e0a477877b725e26cf"},"uri":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf","target":[{"source":"vault:/Paper Critiques/Paper3/osdi18-chen.pdf","selector":[{"type":"TextPositionSelector","start":14036,"end":14226},{"type":"TextQuoteSelector","exact":"(1) injective (one-to-onemap, e.g., add), (2) reduction (e.g., sum), (3) complex-out-fusable (can fuse element-wise map to output, e.g.,conv2d), and (4) opaque (cannot be fused, e.g., sort).","prefix":"rcategories of graph operators: ","suffix":" Weprovide generic rules to fuse"}]}]}
>```
>%%
>*%%PREFIX%%rcategories of graph operators:%%HIGHLIGHT%% ==(1) injective (one-to-onemap, e.g., add), (2) reduction (e.g., sum), (3) complex-out-fusable (can fuse element-wise map to output, e.g.,conv2d), and (4) opaque (cannot be fused, e.g., sort).== %%POSTFIX%%Weprovide generic rules to fuse*
>%%LINK%%[[#^20mwg7tvpgr|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^20mwg7tvpgr
