
#### 1. Model

### MODEL 3 : 7 Layers with 4 Convolution layer
----------
``` Python
     model = keras.models.Sequential([
                    keras.layers.Conv2D(32, (3,3), activation = 'relu', input_shape = (28, 28,1)),  # layer 1
                    keras.layers.MaxPool2D((2,2)),                                                  # layer 2
                    keras.layers.Conv2D(64, (3,3), activation = 'relu'),                            # layer 3
                    keras.layers.Conv2D(64, (3,3), activation = 'relu'),                            # layer 4
                    keras.layers.MaxPool2D((2,2)),                                                  # layer 5
                    keras.layers.Conv2D(128, (3,3), activation = 'relu'),                           # layer 6
                    keras.layers.Flatten(),
                    keras.layers.Dense(10, activation = 'softmax')])   
```


#### 2. Training with Training loss
### Training Step
### Training for 5 epochs.
![epoch](https://user-images.githubusercontent.com/66125576/173174477-c4fcf9c8-2100-4b41-9fb1-f7bd37b512fd.PNG)


#### 3. Test Accuracy
### Perform Test with Test data
![perform3](https://user-images.githubusercontent.com/66125576/173178224-83e70659-f71e-4b33-aa22-ca1658fb139f.PNG)

#### 4. Images and corresponding probability that predicted Right
![predicted Right3](https://user-images.githubusercontent.com/66125576/173178257-d55a0800-8e2c-463a-9f19-806e5c58aae0.PNG)

#### 5. Images and corresponding probability that predicted Wrong
![53](https://user-images.githubusercontent.com/66125576/173178282-4e27b793-595c-4e62-8058-091b544a23f0.PNG)
