# Text type Submission:  

#### Question-1: What are Channels and Kernels  
**Channel:** is like a container which contains a fixed type of information, for example if we want to extract e from different set of images , then the collection of all the es will be called as a channel.  
**Kernel:** Suppose we want to extract a single feature from an image , like extracting e from a set of images , we would be using a e extractor , this is called a filter or a feature extractor or a kernel.  

#### Question-2: Why should we (nearly) always use 3x3 kernels?  
Because it has a axis of symmetry , and combination of 3x3 can be used to construct different size of kernels with lesser parameters, which further accelerate the training.  

#### Question-3: How many times to we need to perform 3x3 convolutions operations to reach close to 1x1 from 199x199 (type each layer output like 199x199 > 197x197...)  
100, The series of convolutions using 3X3 kernels are as follows:  

199x199>197x197>195x195>193x193>191x191>189x189>187x187>185x185>183x183>181x181>179x179>177x177>175x175>173x173>171x171>169x169>167x167>165x165>163x163>161x161>159x159>157x157>155x155>153x153>151x151>149x149>147x147>145x145>143x143>141x141>139x139>137x137>135x135>133x133>131x131>129x129>127x127>125x125>123x123>121x121>119x119>117x117>115x115>113x113>111x111>109x109>107x107>105x105>103x103>101x101>99x99>97x97>95x95>93x93>91x91>89x89>87x87>85x85>83x83>81x81>79x79>77x77>75x75>73x73>71x71>69x69>67x67>65x65>63x63>61x61>59x59>57x57>55x55>53x53>51x51>49x49>47x47>45x45>43x43>41x41>39x39>37x37>35x35>33x33>31x31>29x29>27x27>25x25>23x23>21x21>19x19>17x17>15x15>13x13>11x11>9x9>7x7>5x5>3x3>1x1  

#### Question-4: How are kernels initialized?  
Kernels are initialized randomly.  

#### Question-5: What happens during the training of DNN?  
While training a model we do this (following things happen):

1. Choose activation function.  

2. Choose a kernel and randomly initialize weights.  

3. Decide number of input, hidden and output layers - these are hyperparameters (Build a custom DNN architecture).  

4. Choose an optimal learning rate.  

5. Running Forward Propagation and Backward propagations on loop (1 cycle ~ 1 epoch) with hyper parameter tuning until model convergence.  

6.  Check Training and test errors.  
