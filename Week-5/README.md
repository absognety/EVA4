## Model Interpretation and Steps:  
- In the first attempt, I added convolution layers and played around with kernel dimensions without any batch norm or Dropout 
and trained the model for 15 epochs.  
  + The best training accuracy is 99.28%  
  + The best test accuracy is 98.94%  
  + Total parameters used: 12,564.  
    
- In the second attempt, I added Batch normalization layer along with dropout layer to handle regularization for overfitting.  
  + The best training accuracy is 99.12%  
  + The best test accuracy is 99.28%  
  + Total parameters used: 17,716  
    
- In third attempt, I added global average pooling and removed one of the convolution layers to decrease number of parameters.  
  + The best training accuracy is 99.10%  
  + The best test accuracy is 99.36%  
  + Total parameters used: 10,706  
  
- In the fourth and final attempt, I included image augmentation strategy which includes the transform of rotating images in 
training set by +/- 7 degrees.  
  + The best training accuracy is 98.77%  
  + The best test accuracy is 99.44%  
  + Total parametere used: 9934 < 10k which is expected.
