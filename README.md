# Image Classification for Parkinson's Disease Detection
Image classification for detecting Parkinson's using Hand-Drawn Spiral Images using **Conv>

## Data Structure
Structure your data in the following way:
```
data/
        training/
                healthy/
                        img01/
                        img02/
                        ...
                parkinson/
                        img01/
                        img02/
                        ...
        testing/
                healthy/
                        img01/
                        img02/
                        ...
                parkinson/
                        img01/
                        img02/
                        ...
        validation/
                healthy/
                        img01/
                        img02/
                        ...
                parkinson/
                        img01/
                        img02/
                        ...

```
## Models:
### Model 1 - LeNet

Model: "sequential_17"
_________________________________________________________________
 Layer (type)                Output Shape              Param #   
=================================================================
 sequential_16 (Sequential)  (None, 64, 64, 3)         0         
                                                                 
 rescaling_3 (Rescaling)     (None, 64, 64, 3)         0         
                                                                 
 conv2d_52 (Conv2D)          (None, 60, 60, 6)         456       
                                                                 
 average_pooling2d_18 (Avera  (None, 30, 30, 6)        0         
 gePooling2D)                                                    
                                                                 
 conv2d_53 (Conv2D)          (None, 26, 26, 6)         906       
                                                                 
 average_pooling2d_19 (Avera  (None, 13, 13, 6)        0         
 gePooling2D)                                                    
                                                                 
 dense_42 (Dense)            (None, 13, 13, 120)       840       
                                                                 
 flatten_14 (Flatten)        (None, 20280)             0         
                                                                 
 dense_43 (Dense)            (None, 84)                1703604   
                                                                 
 dense_44 (Dense)            (None, 1)                 85        
                                                                 
=================================================================
Total params: 1,705,891
Trainable params: 1,705,891
Non-trainable params: 0
_________________________________________________________________
