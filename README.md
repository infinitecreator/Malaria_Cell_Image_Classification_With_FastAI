# Malaria_Cell_Image_Classification_With_FastAI
A binary image classification on Kaggle Malaria Cell Images Dataset with FastAI library with an accuracy of approx 97%

# About the classfication
The dataset was divided into two classes of infected and uninfected cell images of which we have to create
a model which can classify from between two.

# About Architecture
I used Transfer Learning method with Resnet34 weights to train with additional fully connected nn layers
and again by unfreezing( to train my images with the whole architecture from the scratch) to get an
accuracy of 97%

# Pixel Degradation Trick
Initially I reduced the size of original pixel to half and used transfer learning with resnet on that cropped pixel
dataset, after that I again used transfer learning method with cropped pixel trained model weights to train
my new original sized images dataset which did the trick without overfitting

# About the dataset
The dataset was obtained from kaggle dataset 
Website: https://www.kaggle.com/iarunava/cell-images-for-detecting-malaria
