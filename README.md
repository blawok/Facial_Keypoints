[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/blawok/Facial_Keypoints/blob/master/facial_keypoint_detection.ipynb)

# Facial_Keypoints
In this project we are predicting 15 key features on human faces. The dataset consists of 7039 images - all in size of 96x96 pixels with 30 coordinates of those features for each image (images are predictors).

For only 4 of those features we have data in all observations and in the rest we've got around 2200 observations. We first train the network on the whole data for those 4 features (8 coordinates) and then use the layers from it to train the target network with all features by adding few layers on top of the initial one. This solution outperforms all others that we've tried.

Data can be download from:
https://www.kaggle.com/c/facial-keypoints-detection/data
