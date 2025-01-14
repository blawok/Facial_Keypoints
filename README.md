[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/blawok/Facial_Keypoints/blob/master/facial_keypoint_detection.ipynb)

# Facial_Keypoints
In this project we are predicting 15 key features on human faces. The dataset consists of 7039 images - all in size of 96x96 pixels with 30 coordinates of those features for each image (images are predictors).

![predictors](https://user-images.githubusercontent.com/41793223/81468350-361fa700-91df-11ea-8ba6-ef3a39e00b4b.JPG)

## Data
For only 4 of those features we have data in all observations and in the rest we've got around 2200 observations (as you can see below).

![missing_data](https://user-images.githubusercontent.com/41793223/81406906-bd670f00-913a-11ea-910c-620168cafa15.JPG)

Data can be download from:
https://www.kaggle.com/c/facial-keypoints-detection/data

## Transfer Learning
We trained the network on the whole data for those 4 features (8 coordinates) and then use the layers from it to train the target network with all features by adding few layers on top of the initial one. This solution outperforms all others that we've tried.

![tf](https://user-images.githubusercontent.com/41793223/81468297-de813b80-91de-11ea-8df4-31b6057d32e7.JPG)

## Results 
```
RMSE (in pixels): 1.556
```

It works quite well but it is not perfect :)

![indeks](https://user-images.githubusercontent.com/41793223/81406970-d96ab080-913a-11ea-81d3-d95ac64fc76c.png)
