# X-RayImage-classification-DL
Chest X-Ray Image Classification using Deep Learning Models

## Project Overview
* The dataset for this project is the Chest X-Ray Images (Pneumonia), published by Daniel et al., (2018), and available on Kaggle by Paul Mooney.
* Implemented simple CNN and transfer Learning Models using python. 
* Total of five models were implemented for this project - CNN Model 1, CNN Model 2, CNN Model 3, VGG16 and VGG19.
* Performed data preparation for images (Image Scaling, Image Augmentation), Exploratory Data Analysis.
* Fine Tuned the models to decide the best performing models.
* Accuracy for the five models are as follows:
* CNN Model 1: 94.17
* CNN Model 2: 95.13
* CNN Model 3: 92.48
* VGG16: 82.85
* VGG19: 84.45

## Code and Resources Used

* Google Colaboratory
* Libraries: keras, tensorflow
* [Dataset](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia)


## EDA

#### Visualizing the Augmented Image Data
![image](https://user-images.githubusercontent.com/72705368/151664297-1856e997-be8b-4b4f-98f3-671f86674313.png)

## Model Implementation and Performance
First, I did research and decided the models that I will be implementing for this project. Then, I studied the dataset by performing EDA. The dataset had two subfolders under training and testing folders as Normal and Pneumonia.

I tried 5 deep learning model variations and evaluated the performance using Accuracy Score.

| No.|	Experiment |	Model |
| ---| ----------- | ------ |
| 1. |	CNN – 5 Convolutional layers, MaxPooling after each convolutional layer, three dense layer, optimizer = Adam |	CNN Model 1
| 2. |	CNN – 3 Convolutional layers, MaxPooling and dropout (0.2) after each convolutional layer, two dense layers, optimizer = RMSprop |	CNN Model 2
| 3. |	CNN – 6 Convolutional layer, MaxPooling layer after each convolutional layer, dropout (0.2) after every two convolutional layer, three dense layer - dropout (0.3) & BatchNormalization after each dense layer |	CNN Model 3
| 4. | VGG16 – All the layers were frozen except the output layer. Activation function - sigmoid |	VGG16
| 5. |	VGG19 – All implementations were the same as the VGG16 model |	VGG19


## Conclusion 
* In this study, several deep learning models were studied among which the CNN Model 2 gave the best performance based on accuracy. 


## Future Recommendations
* Other transfer learning models can be tried and implemented in order to further improve the models performance. 









