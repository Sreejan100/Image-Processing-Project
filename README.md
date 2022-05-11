# Image-Processing-Project
This repository contains the project details, code and a small video demo on the project related to our course Image processing


Our project is mainly a comparison of IncrptionNetV3 deep learning model, MobileNetV2 deep learning and our custom CNN model on brain tumour classification

**Setup procedure:**

**Step 1:**

Download the dataset from the given link: https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection

**Step 2:**

Load the three workbooks in local anaconda jupyter notebook or in Google colab.

**Step 3:**

Load the datasets in all the three workbooks by configuring the path location

**Step 4:**

Create new folders for storing the augmented images

**Step 5:**

Run the code cells one by one and see the result



**Software Requirements:**

Google Colab or Anaconda software with Tensoflow(Version - 2.5.x), keras(version - 2.7.x) and opencv(version - 4.5.5) libraries installed.

**Hardware Requirements:**

Good Graphical Processing Unit(GPU).

**Working flow for first model.**

Ihe first model that we trained is MobileNetV2 model. It is a predefined deep learning model from tensorflow. At first all the important libraries are being imported. After importing the libraries we import the data into google colab from google drive. The total count of images from the dataset were found out to be around 300 which is very less. Therefore, we first augment the dataset and increase the count of images trom 300 to 3000 images. After augmnentation we create our model for training and testing purpose. First we download the MobileNetV2 architecture from the tensorflow library and then configure it to classify the data with 2 classes. After creation of the model we compile the model. After compilation of the model we divide the dataset into train, validation and test set in the ratio 80:10:10 respectively. After division of the dataset we fit the model for training. After training for 25-30 epochs we create the confusion matrix and classification report. Classification report tells us that MobileNet model has achieved an accuracy of 94%.

**Working flow for second model.**

The second model that we trained is InceptionNetV3 model. It is also a predefined deep learning model. At first all important libraries have been imported. After importing the libraries we import the data into google colab from google drive. After importing the dataset we augment the data so that the count of the data changes from 300 t0 4000 images. After augmentation we create our model for for training and testing purposes. First we download the InceptionNetV3 deep learning model from the tensorflow library and then configure it to classify two classes. After creation of the model we compile the model. After compilation of the model we divide the dataset in the ration 80:10:10 ratio respectively. Then we fit the model fpr training. After training the model for 25-30 epochs. After training is completed we we create the confusion matrix and the classification report. The classification report tells us that the model has achieved an accuracy of 59%.

**Working flow for third model.**

The second model that we trained is our custom CNN  model. It is also a custom made deep learning model. At first all important libraries have been imported. After importing the libraries we import the data into google colab from google drive. After importing the dataset we augment the data so that the count of the data changes from 300 t0 4000 images. After augmentation we create our model for for training and testing purposes. First we download all the required layers from the tensorflow library required for model creation. We use normal convolution layers, dense layers, MaxPooling Layer, DropOut Layer and BatchNormalization Layer. We then create the model by adding the layers sequentially and then configure it to classify two classes. After creation of the model we compile the model. After compilation of the model we divide the dataset in the ration 80:10:10 ratio respectively. Then we fit the model fpr training. After training the model for 25-30 epochs. After training is completed we we create the confusion matrix and the classification report. The classification report tells us that the model has achieved an accuracy of 59%.
