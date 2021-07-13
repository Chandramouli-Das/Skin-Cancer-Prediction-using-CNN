# Skin-Cancer-Prediction-using-CNN

This project is all about to classify skin cancer. It is a multi class classification. 

The dataset is available in Kaggle 

I have done this project with my friend Akshay Manthekar.

The name of the project is Skin cancer classification using CNN architecture. We have some instructions that are needed to follow. As per the evaluation rubric, we need to perform dataset creation, visualization, data augmentation, handling data imbalance, etc. The dataset we got from Kaggle. First, we have created the path of the dataset, we have specified the image height and width along with the batch side. After that, we have splitter the dataset into train and validation dataset in 80:20 ratio. After that, we have done some data visualization to see the sample images and perform a couple of bar charts to understand the dataset. Now we have decided to run a CNN model with 3 convolutional layers. We have compiled with ADAM optimizer and sparse categorical cross-entropy loss function and got the result. We have plotted the loss and accuracy graph and found out there was high overfitting in the model. 



Then we have performed data augmentation. We have performed random flipping horizontally and also random rotation of 0.3. Then we again fed the data into the CNN model with 3 convolutional layers. After augmentation, the overfitting problem is gone but here we are getting an accuracy of 60%.



So, we have understood that we need to deal with the data imbalance problem. It is new for us to handle data imbalance in the image dataset. But we have found a way by using the Augmentor library. We have executed this library and made all our target classes with an equal number of images. Then we made the dataset path again and made a data frame which consists all the image path and corresponding labels. After that, we have called the ImagedataGenerator library and split out dataset into train and validation datasets. Before feeding to the CNN model, we decided to use the callback function to reduce the learning rate. Then we have made our final CNN model with 2 convolutional layers using some dropouts. We have compiled it with ADAM optimizer and sparse categorical cross-entropy loss function and got our desired result with good accuracy. 

