---
annotation-target: Paper Critiques/Paper4/1708.04485.pdf
annotation-target-type: pdf
---


>%%
>```annotation-json
>{"created":"2024-02-14T20:45:25.661Z","text":"Sparse CNN accelerator architecture that employs a compressed data format for the sparse weights and activations, eleminating unnecessary data transfers and reduces storage requirements. It also provides an efficient NoC that facilitates efficient delivery of the weights and activations to the PE array and focuses on its reuse. The accumulation is then performed through a novel accumulation array","updated":"2024-02-14T20:45:25.661Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^oa66wgxncgj|show annotation]]
>%%COMMENT%%
>Sparse CNN accelerator architecture that employs a compressed data format for the sparse weights and activations, eleminating unnecessary data transfers and reduces storage requirements. It also provides an efficient NoC that facilitates efficient delivery of the weights and activations to the PE array and focuses on its reuse. The accumulation is then performed through a novel accumulation array
>%%TAGS%%
>#Abstract
^oa66wgxncgj


>%%
>```annotation-json
>{"created":"2024-02-14T20:51:16.609Z","text":"Things to focus on\n- Sparse matrices data format\n- NoC for efficient deleviery to PEs\n- Accumulator for effective addition of these values","updated":"2024-02-14T20:51:16.609Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^gblj1vbeljd|show annotation]]
>%%COMMENT%%
>Things to focus on
>- Sparse matrices data format
>- NoC for efficient deleviery to PEs
>- Accumulator for effective addition of these values
>%%TAGS%%
>
^gblj1vbeljd



>%%
>```annotation-json
>{"created":"2024-02-14T21:08:10.697Z","text":"- How do they do for activations, is there something after the accumulator that compresses the data?\n- size/sparsity limitations","updated":"2024-02-14T21:08:10.697Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^wan6cwc9|show annotation]]
>%%COMMENT%%
>- How do they do for activations, is there something after the accumulator that compresses the data?
>- size/sparsity limitations
>%%TAGS%%
>#qns
^wan6cwc9


>%%
>```annotation-json
>{"created":"2024-02-14T21:10:16.823Z","updated":"2024-02-14T21:10:16.823Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":4349,"end":4380},{"type":"TextQuoteSelector","exact":"typicallyranges from 20% to 80%","prefix":"es widely across the layers but ","suffix":" [15], [14]. Eliminating weights"}]}]}
>```
>%%
>*%%PREFIX%%es widely across the layers but%%HIGHLIGHT%% ==typicallyranges from 20% to 80%== %%POSTFIX%%[15], [14]. Eliminating weights*
>%%LINK%%[[#^th8jy7ck06|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^th8jy7ck06


>%%
>```annotation-json
>{"created":"2024-02-14T21:10:55.485Z","updated":"2024-02-14T21:10:55.485Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":4928,"end":4973},{"type":"TextQuoteSelector","exact":"50–70% of the activations are clamped tozero.","prefix":"hows that fortypical data sets, ","suffix":" Since the multiplication of wei"}]}]}
>```
>%%
>*%%PREFIX%%hows that fortypical data sets,%%HIGHLIGHT%% ==50–70% of the activations are clamped tozero.== %%POSTFIX%%Since the multiplication of wei*
>%%LINK%%[[#^24zz6glnge|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^24zz6glnge


>%%
>```annotation-json
>{"created":"2024-02-14T21:11:28.958Z","updated":"2024-02-14T21:11:28.958Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":6525,"end":6678},{"type":"TextQuoteSelector","exact":" SCNN dataflow only deliversweights and activations to the multiplier array that can allbe multiplied by one another in the manner of a Cartesianproduct.","prefix":"aflows [5], [11], [7], [25], the","suffix":" Furthermore, the activation vec"}]}]}
>```
>%%
>*%%PREFIX%%aflows [5], [11], [7], [25], the%%HIGHLIGHT%% ==SCNN dataflow only deliversweights and activations to the multiplier array that can allbe multiplied by one another in the manner of a Cartesianproduct.== %%POSTFIX%%Furthermore, the activation vec*
>%%LINK%%[[#^fupq5yymo47|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^fupq5yymo47


>%%
>```annotation-json
>{"created":"2024-02-14T21:11:47.702Z","updated":"2024-02-14T21:11:47.702Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":6692,"end":6816},{"type":"TextQuoteSelector","exact":"the activation vectors are reused inan input stationary [6] fashion against a number of weightvectors to reduce data accesse","prefix":" Cartesianproduct. Furthermore, ","suffix":"s. Finally, only non-zero weight"}]}]}
>```
>%%
>*%%PREFIX%%Cartesianproduct. Furthermore,%%HIGHLIGHT%% ==the activation vectors are reused inan input stationary [6] fashion against a number of weightvectors to reduce data accesse== %%POSTFIX%%s. Finally, only non-zero weight*
>%%LINK%%[[#^5i7n025brnl|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^5i7n025brnl


>%%
>```annotation-json
>{"created":"2024-02-14T21:11:51.832Z","updated":"2024-02-14T21:11:51.832Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":6827,"end":6944},{"type":"TextQuoteSelector","exact":" only non-zero weightsand activations are fetched from the input storage arrays anddelivered to the multiplier array.","prefix":"o reduce data accesses. Finally,","suffix":" As with any CNN accelerator,SCN"}]}]}
>```
>%%
>*%%PREFIX%%o reduce data accesses. Finally,%%HIGHLIGHT%% ==only non-zero weightsand activations are fetched from the input storage arrays anddelivered to the multiplier array.== %%POSTFIX%%As with any CNN accelerator,SCN*
>%%LINK%%[[#^9z78o1upq8q|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^9z78o1upq8q


>%%
>```annotation-json
>{"created":"2024-02-14T21:12:58.738Z","updated":"2024-02-14T21:12:58.738Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":7142,"end":7291},{"type":"TextQuoteSelector","exact":" SCNN tracksthe output coordinates associated with each multiplication andsends the coordinate and product to a scatter accumulator arrayfor summing.","prefix":"not be directly summed together,","suffix":"To increase parallelism beyond a"}]}]}
>```
>%%
>*%%PREFIX%%not be directly summed together,%%HIGHLIGHT%% ==SCNN tracksthe output coordinates associated with each multiplication andsends the coordinate and product to a scatter accumulator arrayfor summing.== %%POSTFIX%%To increase parallelism beyond a*
>%%LINK%%[[#^v3ke8zskhw|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^v3ke8zskhw


>%%
>```annotation-json
>{"created":"2024-02-14T21:13:07.415Z","updated":"2024-02-14T21:13:07.415Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":7335,"end":7430},{"type":"TextQuoteSelector","exact":"multiple PEscan be run in parallel with each working on a disjoint 3D tileof input activations.","prefix":"parallelism beyond a single PE, ","suffix":" Because of the end-to-end compr"}]}]}
>```
>%%
>*%%PREFIX%%parallelism beyond a single PE,%%HIGHLIGHT%% ==multiple PEscan be run in parallel with each working on a disjoint 3D tileof input activations.== %%POSTFIX%%Because of the end-to-end compr*
>%%LINK%%[[#^x5g4l1oo5wg|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^x5g4l1oo5wg


>%%
>```annotation-json
>{"created":"2024-02-14T21:25:22.464Z","text":"model to evaulate how efficent the model is\n- how comprehensive is the model?\n- Are there improvements to be made in the model? ","updated":"2024-02-14T21:25:22.464Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^jtihlplrqu|show annotation]]
>%%COMMENT%%
>model to evaulate how efficent the model is
>- how comprehensive is the model?
>- Are there improvements to be made in the model? 
>%%TAGS%%
>
^jtihlplrqu


>%%
>```annotation-json
>{"created":"2024-02-14T21:27:59.181Z","updated":"2024-02-14T21:27:59.181Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":11035,"end":11125},{"type":"TextQuoteSelector","exact":"The primary technique for creatingweight sparsity is to prune the network during training.","prefix":"t andinput activation matrices. ","suffix":" Han,et al. developed a pruning "}]}]}
>```
>%%
>*%%PREFIX%%t andinput activation matrices.%%HIGHLIGHT%% ==The primary technique for creatingweight sparsity is to prune the network during training.== %%POSTFIX%%Han,et al. developed a pruning*
>%%LINK%%[[#^k3g1gwv279l|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^k3g1gwv279l


>%%
>```annotation-json
>{"created":"2024-02-14T21:28:10.016Z","updated":"2024-02-14T21:28:10.016Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":11201,"end":11310},{"type":"TextQuoteSelector","exact":"First, any weight with an absolute value thatis close to zero (e.g. below a defined threshold) is set tozero.","prefix":"at operates in two2phases [15]. ","suffix":" This process has the effect of "}]}]}
>```
>%%
>*%%PREFIX%%at operates in two2phases [15].%%HIGHLIGHT%% ==First, any weight with an absolute value thatis close to zero (e.g. below a defined threshold) is set tozero.== %%POSTFIX%%This process has the effect of*
>%%LINK%%[[#^lb4oin6b7on|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^lb4oin6b7on


>%%
>```annotation-json
>{"created":"2024-02-14T21:28:20.483Z","updated":"2024-02-14T21:28:20.483Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":11452,"end":11540},{"type":"TextQuoteSelector","exact":" the remaining network is retrained,to regain the accuracy lost through na ̈ıve pruning.","prefix":"ion toalways to be zero. Second,","suffix":" The resultis a smaller network "}]}]}
>```
>%%
>*%%PREFIX%%ion toalways to be zero. Second,%%HIGHLIGHT%% ==the remaining network is retrained,to regain the accuracy lost through na ̈ıve pruning.== %%POSTFIX%%The resultis a smaller network*
>%%LINK%%[[#^uedx8wd99l|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^uedx8wd99l


>%%
>```annotation-json
>{"created":"2024-02-14T21:30:04.642Z","updated":"2024-02-14T21:30:04.642Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":11715,"end":11822},{"type":"TextQuoteSelector","exact":"Activation sparsity occurs dynamically during inference andis highly dependent on the data being processed.","prefix":"size while maintaining accuracy.","suffix":" Specifically,the rectified line"}]}]}
>```
>%%
>*%%PREFIX%%size while maintaining accuracy.%%HIGHLIGHT%% ==Activation sparsity occurs dynamically during inference andis highly dependent on the data being processed.== %%POSTFIX%%Specifically,the rectified line*
>%%LINK%%[[#^l6xgkcjvt3|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^l6xgkcjvt3


>%%
>```annotation-json
>{"created":"2024-02-14T21:31:36.836Z","updated":"2024-02-14T21:31:36.836Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":13687,"end":13851},{"type":"TextQuoteSelector","exact":"Encoding the sparse weights and/oractivations provides an architecture an opportunity toreduce the amount of data that must be moved throughoutthe memory hierarchy.","prefix":"ptimization:• Compressing data: ","suffix":" It also reduces the data footpr"}]}]}
>```
>%%
>*%%PREFIX%%ptimization:• Compressing data:%%HIGHLIGHT%% ==Encoding the sparse weights and/oractivations provides an architecture an opportunity toreduce the amount of data that must be moved throughoutthe memory hierarchy.== %%POSTFIX%%It also reduces the data footpr*
>%%LINK%%[[#^zvlpb7mry6j|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^zvlpb7mry6j


>%%
>```annotation-json
>{"created":"2024-02-14T21:31:43.117Z","updated":"2024-02-14T21:31:43.117Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":13984,"end":14139},{"type":"TextQuoteSelector","exact":"For multiplications that havea zero weight and/or activation operand, the operationcan be data gated or the operands might never be sent tothe multiplier. ","prefix":"ture.• Eliminating computation: ","suffix":"This can save energy consumption"}]}]}
>```
>%%
>*%%PREFIX%%ture.• Eliminating computation:%%HIGHLIGHT%% ==For multiplications that havea zero weight and/or activation operand, the operationcan be data gated or the operands might never be sent tothe multiplier.== %%POSTFIX%%This can save energy consumption*
>%%LINK%%[[#^rc4ggf23wle|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^rc4ggf23wle


>%%
>```annotation-json
>{"created":"2024-02-14T21:32:02.058Z","updated":"2024-02-14T21:32:02.058Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":14991,"end":15088},{"type":"TextQuoteSelector","exact":"novel dataflow that deliversonly those densely encoded weights and activations to themultipliers.","prefix":".activations. Second, it uses a ","suffix":"III. SCNN DATAFLOWThe core opera"}]}]}
>```
>%%
>*%%PREFIX%%.activations. Second, it uses a%%HIGHLIGHT%% ==novel dataflow that deliversonly those densely encoded weights and activations to themultipliers.== %%POSTFIX%%III. SCNN DATAFLOWThe core opera*
>%%LINK%%[[#^7btm1lbuivc|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^7btm1lbuivc


>%%
>```annotation-json
>{"created":"2024-02-14T21:35:33.299Z","text":"- planar tiled - partitions the WxH element actication plane to tiles allowing each PE to work independently\n- input stationary - input activation is held stationary at the PEs\n- CartesianProduct-sparse - ","updated":"2024-02-14T21:35:33.299Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":17489,"end":17540},{"type":"TextQuoteSelector","exact":"PlanarTiled-InputStationary-CartesianProduct-sparse","prefix":"esent a specific dataflow called","suffix":" (or PT-IS-CP-sparse). After exa"}]}]}
>```
>%%
>*%%PREFIX%%esent a specific dataflow called%%HIGHLIGHT%% ==PlanarTiled-InputStationary-CartesianProduct-sparse== %%POSTFIX%%(or PT-IS-CP-sparse). After exa*
>%%LINK%%[[#^d79waz7f7m4|show annotation]]
>%%COMMENT%%
>- planar tiled - partitions the WxH element actication plane to tiles allowing each PE to work independently
>- input stationary - input activation is held stationary at the PEs
>- CartesianProduct-sparse - 
>%%TAGS%%
>
^d79waz7f7m4


>%%
>```annotation-json
>{"created":"2024-02-14T22:15:53.627Z","updated":"2024-02-14T22:15:53.627Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":22360,"end":22468},{"type":"TextQuoteSelector","exact":"employa tiling strategy to spread the work across an array of PEsso that each PE can operate independently. ","prefix":"nd buffer sizes within a PE, we ","suffix":"PT-IS-CP-densepartitions the W ×"}]}]}
>```
>%%
>*%%PREFIX%%nd buffer sizes within a PE, we%%HIGHLIGHT%% ==employa tiling strategy to spread the work across an array of PEsso that each PE can operate independently.== %%POSTFIX%%PT-IS-CP-densepartitions the W ×*
>%%LINK%%[[#^nu4xch2jpej|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^nu4xch2jpej


>%%
>```annotation-json
>{"created":"2024-02-14T22:16:31.541Z","updated":"2024-02-14T22:16:31.541Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":22482,"end":22559},{"type":"TextQuoteSelector","exact":"partitions the W ×H element activation plane into smallerWt ×Ht element tiles","prefix":"te independently. PT-IS-CP-dense","suffix":" that are distributed across the"}]}]}
>```
>%%
>*%%PREFIX%%te independently. PT-IS-CP-dense%%HIGHLIGHT%% ==partitions the W ×H element activation plane into smallerWt ×Ht element tiles== %%POSTFIX%%that are distributed across the*
>%%LINK%%[[#^c0jqqykilf|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^c0jqqykilf


>%%
>```annotation-json
>{"created":"2024-02-14T22:18:41.945Z","text":"# Tiling Strategy and Halos\nThe activation plane is broken down into smaller tiles. However, this introduces cross-tile dependencies for convolution as it is a sliding operation. this is called halos. they can be resolved in 2 ways:\n1) Input halos - i/p buffers are sized larger to accomodate halos. Replicated i/p values are usually multicast when loading\n2) o/p halos: o/p buffers sized larger. Incomplete partial sums are then communicated with the neighbour PEs for accumulation","updated":"2024-02-14T22:18:41.945Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^g4ymtujq4n9|show annotation]]
>%%COMMENT%%
># Tiling Strategy and Halos
>The activation plane is broken down into smaller tiles. However, this introduces cross-tile dependencies for convolution as it is a sliding operation. this is called halos. they can be resolved in 2 ways:
>1) Input halos - i/p buffers are sized larger to accomodate halos. Replicated i/p values are usually multicast when loading
>2) o/p halos: o/p buffers sized larger. Incomplete partial sums are then communicated with the neighbour PEs for accumulation
>%%TAGS%%
>
^g4ymtujq4n9


>%%
>```annotation-json
>{"created":"2024-02-14T22:32:02.695Z","text":"sending coordinates along with non-zero weights may not be optimal","updated":"2024-02-14T22:32:02.695Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":25539,"end":25647},{"type":"TextQuoteSelector","exact":"delivers a vector of F non-zero filter weights along with each of their coordinates withinthe Kc×R×S region.","prefix":" each access, the weight buffer ","suffix":" Similarly, the input buffer del"}]}]}
>```
>%%
>*%%PREFIX%%each access, the weight buffer%%HIGHLIGHT%% ==delivers a vector of F non-zero filter weights along with each of their coordinates withinthe Kc×R×S region.== %%POSTFIX%%Similarly, the input buffer del*
>%%LINK%%[[#^5yanabfx55w|show annotation]]
>%%COMMENT%%
>sending coordinates along with non-zero weights may not be optimal
>%%TAGS%%
>
^5yanabfx55w


>%%
>```annotation-json
>{"created":"2024-02-14T22:38:03.803Z","updated":"2024-02-14T22:38:03.803Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":29490,"end":29705},{"type":"TextQuoteSelector","exact":"Each PE’s state machine operates on the weight and in-put activations in the order defined by the PT-IS-CP-sparsedataflow to produce an output-channel group of Kc ×Wt ×Htpartial sums inside the accumulation buffers.","prefix":". 5. Complete SCNN architecture.","suffix":" First, a vector Fof compressed "}]}]}
>```
>%%
>*%%PREFIX%%. 5. Complete SCNN architecture.%%HIGHLIGHT%% ==Each PE’s state machine operates on the weight and in-put activations in the order defined by the PT-IS-CP-sparsedataflow to produce an output-channel group of Kc ×Wt ×Htpartial sums inside the accumulation buffers.== %%POSTFIX%%First, a vector Fof compressed*
>%%LINK%%[[#^mdrz005eezi|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^mdrz005eezi


>%%
>```annotation-json
>{"created":"2024-02-14T22:43:11.441Z","text":"what is being sent to PEs?\n- PEs have a weight buffer, i/o activation RAMs. multiplier array, accumulator buffers and post-processing unit\n- input is broken down and streamed to IARAM of each PE. \n- sparse-compressed o/p is distributed across the OARAMs. \n- When possible, activations are held in the IARAMs/OARAMs, not relying on the DRAM\n\nHow many multiplier does each PE have?\n- each PE has a multiplier array\n- special accumulator buffer for each PE, followed by a PPU to compress and deal with halos before storing to OARAM.\n","updated":"2024-02-14T22:43:11.441Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^8ojvthywjp3|show annotation]]
>%%COMMENT%%
>what is being sent to PEs?
>- PEs have a weight buffer, i/o activation RAMs. multiplier array, accumulator buffers and post-processing unit
>- input is broken down and streamed to IARAM of each PE. 
>- sparse-compressed o/p is distributed across the OARAMs. 
>- When possible, activations are held in the IARAMs/OARAMs, not relying on the DRAM
>
>How many multiplier does each PE have?
>- each PE has a multiplier array
>- special accumulator buffer for each PE, followed by a PPU to compress and deal with halos before storing to OARAM.
>
>%%TAGS%%
>
^8ojvthywjp3


>%%
>```annotation-json
>{"created":"2024-02-14T22:51:37.881Z","updated":"2024-02-14T22:51:37.881Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":31084,"end":31162},{"type":"TextQuoteSelector","exact":"simple compressed-sparse encoding approachbased on run-length encoding scheme.","prefix":"them into the OARAM.SCNN uses a ","suffix":" The index vectorencodes the num"}]}]}
>```
>%%
>*%%PREFIX%%them into the OARAM.SCNN uses a%%HIGHLIGHT%% ==simple compressed-sparse encoding approachbased on run-length encoding scheme.== %%POSTFIX%%The index vectorencodes the num*
>%%LINK%%[[#^cvo7ou78lep|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^cvo7ou78lep


>%%
>```annotation-json
>{"created":"2024-02-14T22:51:47.674Z","updated":"2024-02-14T22:51:47.674Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":31498,"end":31586},{"type":"TextQuoteSelector","exact":"Four bits per index allows for upto 15 zeros to appear between any two non-zero elements","prefix":"spacecurrently being processed. ","suffix":".Non-zero elements that are furt"}]}]}
>```
>%%
>*%%PREFIX%%spacecurrently being processed.%%HIGHLIGHT%% ==Four bits per index allows for upto 15 zeros to appear between any two non-zero elements== %%POSTFIX%%.Non-zero elements that are furt*
>%%LINK%%[[#^rsj7zmhykzi|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^rsj7zmhykzi


>%%
>```annotation-json
>{"created":"2024-02-14T22:53:07.040Z","updated":"2024-02-14T22:53:07.040Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":34032,"end":34107},{"type":"TextQuoteSelector","exact":"SCNN design includes a totalof 1,024 multipliers and 1MB of activation RAM.","prefix":"7.9sparse format. In total, the ","suffix":" At thesynthesized clock speed o"}]}]}
>```
>%%
>*%%PREFIX%%7.9sparse format. In total, the%%HIGHLIGHT%% ==SCNN design includes a totalof 1,024 multipliers and 1MB of activation RAM.== %%POSTFIX%%At thesynthesized clock speed o*
>%%LINK%%[[#^evqzvnxjbqf|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^evqzvnxjbqf


>%%
>```annotation-json
>{"created":"2024-02-14T23:00:47.946Z","updated":"2024-02-14T23:00:47.946Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":35955,"end":36089},{"type":"TextQuoteSelector","exact":"TimeLoop, a detailed analytical modelfor CNN accelerators to enable an exploration of the designspace of dense and sparse architecture","prefix":" architecture.We also developed ","suffix":"s. TimeLoop can modela wide rang"}]}]}
>```
>%%
>*%%PREFIX%%architecture.We also developed%%HIGHLIGHT%% ==TimeLoop, a detailed analytical modelfor CNN accelerators to enable an exploration of the designspace of dense and sparse architecture== %%POSTFIX%%s. TimeLoop can modela wide rang*
>%%LINK%%[[#^wtburupxfyq|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^wtburupxfyq


>%%
>```annotation-json
>{"created":"2024-02-16T16:42:03.557Z","updated":"2024-02-16T16:42:03.557Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":27302,"end":27583},{"type":"TextQuoteSelector","exact":"nstead of a dense vector fetches, (B) and (D)fetch the compressed sparse input activations and weights,respectively. In addition, the coordinates of the non-zero valuesin the compressed-sparse form of these data structures must befetched from their respective buffers (not shown). ","prefix":" small adjustmentsof Figure 4. I","suffix":"After thatthe accumulator buffer"}]}]}
>```
>%%
>*%%PREFIX%%small adjustmentsof Figure 4. I%%HIGHLIGHT%% ==nstead of a dense vector fetches, (B) and (D)fetch the compressed sparse input activations and weights,respectively. In addition, the coordinates of the non-zero valuesin the compressed-sparse form of these data structures must befetched from their respective buffers (not shown).== %%POSTFIX%%After thatthe accumulator buffer*
>%%LINK%%[[#^n8t3b5xkeos|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^n8t3b5xkeos


>%%
>```annotation-json
>{"created":"2024-02-16T16:39:42.516Z","text":"## Possible issues\n1) The tiling methodology introduces halos, which cuts down data reuse as the same data has to be held by multiple PEs, decreasing compute effectiveness\n2) Works only on CNNs as every value of the filter gets multiplied with the input at some point of time; for normal matrix multiplications, the partial sums generated may not be useful all the time since it first computes it and then decides which all outputs require the value.","updated":"2024-02-16T16:39:42.516Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^muil4emr51d|show annotation]]
>%%COMMENT%%
>## Possible issues
>1) The tiling methodology introduces halos, which cuts down data reuse as the same data has to be held by multiple PEs, decreasing compute effectiveness
>2) Works only on CNNs as every value of the filter gets multiplied with the input at some point of time; for normal matrix multiplications, the partial sums generated may not be useful all the time since it first computes it and then decides which all outputs require the value.
>%%TAGS%%
>
^muil4emr51d


>%%
>```annotation-json
>{"created":"2024-02-16T16:45:11.901Z","updated":"2024-02-16T16:45:11.901Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":27593,"end":27711},{"type":"TextQuoteSelector","exact":"the accumulator buffer (F) must be indexed with the computedoutput coordinates from the sparse weight and activations.","prefix":" buffers (not shown). After that","suffix":"Finally, when the computation fo"}]}]}
>```
>%%
>*%%PREFIX%%buffers (not shown). After that%%HIGHLIGHT%% ==the accumulator buffer (F) must be indexed with the computedoutput coordinates from the sparse weight and activations.== %%POSTFIX%%Finally, when the computation fo*
>%%LINK%%[[#^tlewpnge0o|show annotation]]
>%%COMMENT%%
>
>%%TAGS%%
>
^tlewpnge0o


>%%
>```annotation-json
>{"created":"2024-02-16T16:43:12.127Z","text":"## Positives\n1) Computations are cut down as opposed to a dense multiplier, provided the arrays are sparse enough (which they are through factors such as dropout)\n2) Sparse encoding frees up bandwidth to PE","updated":"2024-02-16T16:43:12.127Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}
>```
>%%
>*%%PREFIX%%%%HIGHLIGHT%% ==== %%POSTFIX%%*
>%%LINK%%[[#^sk4d9wuugy|show annotation]]
>%%COMMENT%%
>## Positives
>1) Computations are cut down as opposed to a dense multiplier, provided the arrays are sparse enough (which they are through factors such as dropout)
>2) Sparse encoding frees up bandwidth to PE
>%%TAGS%%
>
^sk4d9wuugy


>%%
>```annotation-json
>{"created":"2024-02-16T16:49:10.187Z","text":"what is a cartesian product of vectors?","updated":"2024-02-16T16:49:10.187Z","document":{"title":"1708.04485.pdf","link":[{"href":"urn:x-pdf:66bf3c14c1a1c58575f14454d4699e3f"},{"href":"vault:/Paper Critiques/Paper4/1708.04485.pdf"}],"documentFingerprint":"66bf3c14c1a1c58575f14454d4699e3f"},"uri":"vault:/Paper Critiques/Paper4/1708.04485.pdf","target":[{"source":"vault:/Paper Critiques/Paper4/1708.04485.pdf","selector":[{"type":"TextPositionSelector","start":29834,"end":29955},{"type":"TextQuoteSelector","exact":"Thesevectors are distributed into the F ×I multiplier array whichcomputes a form of the cartesian product of the vectors.","prefix":" from their respective buffers. ","suffix":" Atthe same time, the indices fr"}]}]}
>```
>%%
>*%%PREFIX%%from their respective buffers.%%HIGHLIGHT%% ==Thesevectors are distributed into the F ×I multiplier array whichcomputes a form of the cartesian product of the vectors.== %%POSTFIX%%Atthe same time, the indices fr*
>%%LINK%%[[#^mk9dr71e8ln|show annotation]]
>%%COMMENT%%
>what is a cartesian product of vectors?
>%%TAGS%%
>
^mk9dr71e8ln
