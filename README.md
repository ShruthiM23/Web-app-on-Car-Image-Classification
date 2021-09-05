# Web-app-on-Car-Image-Classification

# Problem Statement:
According to the study conducted by "Mordor Intelligence" on the Indian used car market was valued at USD 27 billion in 2020, and it is expected to reach USD 50 Billion by 2026. Link to the article: https://www.mordorintelligence.com/industry-reports/india-used-car-market

Sometimes when people see any car on the road and like it but not sure of the model to further enquire about it, then they can take a snap of it and use our app link to know about the car model. They can consult the used cars dealership.

# Demo:

Deployed using gradio: https://www.gradio.app/ml_examples


https://user-images.githubusercontent.com/85027425/132135320-828e05f6-c5a1-4e25-96e7-2de5e2bdde4b.mp4


![image](https://user-images.githubusercontent.com/85027425/129476008-95a8c8c5-2312-4f09-b13d-9ef6054b1e07.png)

# Class Labels:

Creta<br>
Innova<br>
Nano<br>
Scorpio<br>
Range Rover<br>

# Project Pipeline/Work Flow:
1. Data Collection(Web Scraped)<br>
2. Image Visualization with their class labels<br>
3. Model Building 3.1 Base Model(CNN Based)<br>
3.2 Model 1(CNN + Image Augmentation)<br>
3.3 Model 2(CNN +Image Augmentation + Batch Normalization)<br>
3.4 Model 3(CNN + Image Augmentation + Drop Out)<br>
3.5 Final Model(Transfer Learning + callbacks)<br>
4. Visualize the predictions<br>
5. Analysis of the accuracy and loss of all the models built<br>
6. Deployment(using gradio)<br>

# Steps to handle overfitting:

1. Use of Image Augmentation to make the model learn of the different versions of the training data.<br>
2. Use of L1/L2 regularization, Drop out, Batch Normalization.<br>
3. Use of callbacks such as Early Stopping.<br>
4. Varying the learning rate of the optimizer.<br>

# Steps taken to arrive at the best and final model:

1. Use of pre-trained weights from MobileNet for the 70 convolutional layers.<br>
2. Open up covolutional layers from 71st layer to train with a dense hidden layer of 512 neurons.<br>
3. These layers account for optimization of weights through backpropagation.<br>
4. Use of GlobalAveragePooling2D.<br>
5. Use of "adam" optimizer.<br>
6. Use of callbacks(EarlyStopping, ModelCheckpoint, CSVLogger).

![image](https://user-images.githubusercontent.com/85027425/129476103-d9ce4d55-c696-4e35-9d45-cf7a987a2621.png)

# Visualize the predictions:

![image](https://user-images.githubusercontent.com/85027425/129476114-689e6a3c-de9f-4f4f-ab82-87f3042d68b4.png)




