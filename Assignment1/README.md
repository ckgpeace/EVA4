Q1. What are Channels and Kernels (according to EVA)?

1.1 Filters/Kernels: Filters/Kernels are feature extractors which are designed to extract basic features/building blocks in an image such as edges
1.2 Channels: Each channel consists of a particular features of given image

Q2. Why should we (nearly) always use 3x3 kernels?

2.1 3x3 kernels are used mostly because it computaionally efficient, it may be due to it is optimized for current proceesing power(CPU and GPU) and it seems to work best

Q3. How many times to we need to perform 3x3 convolutions operations to reach close to 1x1 from 199x199 (type each layer output like 199x199 > 197x197...)

3.1 99

199 > 197	> 195	193	191	189	187	185	183	181	179	177	175	173	171	169	167	165	163	161	159	157	155	153	151	149	147	145	143	141	139	137	135	133	131	129	127	125	123	121	119	117	115	113	111	109	107	105	103	101	99	97	95	93	91	89	87	85	83	81	79	77	75	73	71	69	67	65	63	61	59	57	55	53	51	49	47	45	43	41	39	37	35	33	31	29	27	25	23	21	19	17	15	13	11	9	7	5	3	> 1

4. How are kernels initialized? 

4.1 For initial layers we initialize kernels to detect edges. We can randomly initialize kernels with smaller values except all zeros. Back propogation will take care of the kernels as we train the model

5. What happens during the training of a DNN?

5.1 Input image > Layer1 - Layer2 - ... > final layer > softmax > output
5.2 During training weights of each node of the DNN are adjusted based on the change in the loss values
5.3 Back propagation takes the information from output layer to minimize loss
5.4 Networks keep training till termination crriteria is met or there is no change in the loss
