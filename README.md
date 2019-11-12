## EVA SESSION-1 ASSIGNMENT

# Assignment 1A
The file consists of demonstration of simple Image Processing like Edge detection, image blurring, sharpening etc
# Assignment 1B

## 1.What are Channels and Kernels (according to EVA)?
   A channel represents a particular feature or characteristic of an image. ex: all the vertical edges.	
   A Channel is extracted from an image by convolving it with a Feature Extractor or Kernel.

## 2. Why should we only (well mostly) use 3x3 Kernels?
   To understand this first we have to understand as to why we use only odd kernel. Odd kernels have a line of symmetry 
   which even kernels dont and when we convolve an image with a kernel the resultant pixel is placed at a position corresponding
   to the cetral pixel of the kernel which isn't possible if we have even kernel. Now convolving an image twice using a 3x3 kernel
   is equivalent to convolving the image once with a 5x5 kernel interms of the rreceptive field of the resulting image, but a 5x5 kernel
   has 25 parameters and a 2 layer 3x3 kernel has 2 x (9)=18 parameters, this comparison holds good for other higher odd numbers. Thus interms
   of computer resources using 3x3 kernel is optimal. further the current hardware are optimised for 3x3 kernels.

## 3. How many times do we need to perform 3x3 convolution operation to reach 1x1 from 199x199 (show calculations)
   99 times

199	x	199
197	x	197
195	x	195
193	x	193
191	x	191
189	x	189
187	x	187
185	x	185
183	x	183
181	x	181
179	x	179
177	x	177
175	x	175
173	x	173
171	x	171
169	x	169
167	x	167
165	x	165
163	x	163
161	x	161
159	x	159
157	x	157
155	x	155
153	x	153
151	x	151
149	x	149
147	x	147
145	x	145
143	x	143
141	x	141
139	x	139
137	x	137
135	x	135
133	x	133
131	x	131
129	x	129
127	x	127
125	x	125
123	x	123
121	x	121
119	x	119
117	x	117
115	x	115
113	x	113
111	x	111
109	x	109
107	x	107
105	x	105
103	x	103
101	x	101
99	x	99
97	x	97
95	x	95
93	x	93
91	x	91
89	x	89
87	x	87
85	x	85
83	x	83
81	x	81
79	x	79
77	x	77
75	x	75
73	x	73
71	x	71
69	x	69
67	x	67
65	x	65
63	x	63
61	x	61
59	x	59
57	x	57
55	x	55
53	x	53
51	x	51
49	x	49
47	x	47
45	x	45
43	x	43
41	x	41
39	x	39
37	x	37
35	x	35
33	x	33
31	x	31
29	x	29
27	x	27
25	x	25
23	x	23
21	x	21
19	x	19
17	x	17
15	x	15
13	x	13
11	x	11
9	x	9
7	x	7
5	x	5
3	x	3
1	x	1
