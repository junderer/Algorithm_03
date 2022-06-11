
#### 1. Model

### MODEL 1 : 3 Layers with 1 Convolution layer
----------
``` Python
        model_1 = keras.models.Sequential([
                    keras.layers.Conv2D(32, (3,3), activation = 'relu', input_shape = (28, 28,1)),  # layer 1 
                    keras.layers.MaxPool2D((2,2)),                                                  # layer 2 
                    keras.layers.Flatten(),
                    keras.layers.Dense(10, activation = 'softmax')])                                # layer 3

```


#### 2. Training with Training loss
### Training Step
### Training for 5 epochs.
```Python
model_1.fit(train_images, train_labels, epochs = 5)
```
![epoch1](https://user-images.githubusercontent.com/66125576/173198839-c2b4ba75-0c9f-4bbf-b413-993280b86de9.PNG)




#### 3. Test Accuracy
### Perform Test with Test data

![perform11](https://user-images.githubusercontent.com/66125576/173198905-09c716ea-8fd9-4a13-be6c-993e50d6316e.PNG)


#### 4. Images and corresponding probability that predicted Right
![perform1](https://user-images.githubusercontent.com/66125576/173198873-89f3ea60-5ca4-4e0e-996a-be1ea1391625.PNG)

#### 5. Images and corresponding probability that predicted Wrong
![wrong1](https://user-images.githubusercontent.com/66125576/173198915-8832a1b3-0783-40e8-bdab-3f6ecdefd98e.PNG)


#
#
#
#

#### 1. Model

### MODEL 2 : 5 Layers with 2 Convolution layer
----------
``` Python
         model_2 = keras.models.Sequential([
                    keras.layers.Conv2D(32, (3,3), activation = 'relu', input_shape=(28,28,1)),     # layer 1 
                    keras.layers.MaxPool2D((2,2)),                                                  # layer 2
                    keras.layers.Conv2D(64, (3,3), activation = 'relu'),                            # layer 3 
                    keras.layers.MaxPool2D((2,2)),                                                  # layer 4
                    keras.layers.Flatten(),
                    keras.layers.Dense(10, activation = 'softmax')])                                # layer 5

```


#### 2. Training with Training loss
### Training Step
### Training for 5 epochs.
```Python
model_2.fit(train_images, train_labels, epochs = 5)
```
![epoch2](https://user-images.githubusercontent.com/66125576/173199109-e8995e68-c269-49c7-be38-c5c5b6e4328c.PNG)





#### 3. Test Accuracy
### Perform Test with Test data
![perform2](https://user-images.githubusercontent.com/66125576/173199123-c6798ad3-0af5-4f94-9895-e791cb48ea14.PNG)




#### 4. Images and corresponding probability that predicted Right
![right2](https://user-images.githubusercontent.com/66125576/173199141-89639eb8-48a9-4361-a0cb-e47217c4a569.PNG)


#### 5. Images and corresponding probability that predicted Wrong

![wrong2](https://user-images.githubusercontent.com/66125576/173199149-7d019efc-f12d-496d-99fd-e983c54d6667.PNG)


#
#
#
#


#### 1. Model

### MODEL 3 : 7 Layers with 4 Convolution layer
----------
``` Python
     model_3 = keras.models.Sequential([
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
```Python
model_3.fit(train_images, train_labels, epochs = 5)
```
![epoch](https://user-images.githubusercontent.com/66125576/173174477-c4fcf9c8-2100-4b41-9fb1-f7bd37b512fd.PNG)


#### 3. Test Accuracy
### Perform Test with Test data
![perform3](https://user-images.githubusercontent.com/66125576/173178224-83e70659-f71e-4b33-aa22-ca1658fb139f.PNG)

#### 4. Images and corresponding probability that predicted Right
![predicted Right3](https://user-images.githubusercontent.com/66125576/173178257-d55a0800-8e2c-463a-9f19-806e5c58aae0.PNG)

#### 5. Images and corresponding probability that predicted Wrong
![53](https://user-images.githubusercontent.com/66125576/173178282-4e27b793-595c-4e62-8058-091b544a23f0.PNG)
