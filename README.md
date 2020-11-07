# Quora-Question-Challenge
### This repository consists of an XGBoost Model; trained using the Data from Quora Question Challenge: A Competition where we had to find out the score of redundant questions asked on Quora.

#### The goal behind this prediction model is to identify whether the question which is being posted by a user is already been asked by another user; which will help to provide quicker resolutions and answers. We have to predict whether a pair of questions given are duplicates or not.

##### The Image below describes the training data provided in the challenge

![ScreenShot](https://github.com/uttasarga9067/Quora-Question-Challenge/blob/main/1.PNG)

##### This describes about the various insights of the training data on which we will build our model.

![ScreenShot](https://github.com/uttasarga9067/Quora-Question-Challenge/blob/main/2.PNG)

##### Number of times, total Questions occured (Histogram)

![ScreenShot](https://github.com/uttasarga9067/Quora-Question-Challenge/blob/main/3.PNG)

#### We observe that there is 37% of positive class in the Data set. This positive class is the total number of questions which are repeated. LogLoss from sklearn looks at the actual predictions (is_duplicate in our case) as opposed to the order in which the predictions are, we get a decent score by creating a submission predicting mean value of the label.

##### Here, we are exploring the test data set and looking at the variables present in the same.

![ScreenShot](https://github.com/uttasarga9067/Quora-Question-Challenge/blob/main/4.PNG)


#### We are provided with row ids and the questions which we have to check the redundancy for. We dont have any particular id for each question as we had for our training data set.

##### The distribution of Character count in both the training and test set.

![ScreenShot](https://github.com/uttasarga9067/Quora-Question-Challenge/blob/main/5.PNG)

#### Most of the questions have around 15 to 150 characters in them, while the steep cut-off at 150 Characters is the assumed character limit while posting a question on Quora.
#### The next histogram is for word count in the whole data set. I am using spaces between two words to split them and count the words present.

![ScreenShot](https://github.com/uttasarga9067/Quora-Question-Challenge/blob/main/6.PNG)

#### The Word Cloud Package helps us to showcase the words according to their frequency in the Data.

![ScreenShot](https://github.com/uttasarga9067/Quora-Question-Challenge/blob/main/7.PNG)

#### The Analysis below is for the questions in training set.

![ScreenShot](https://github.com/uttasarga9067/Quora-Question-Challenge/blob/main/8.PNG)


## Finally, the XGBoost Model for predicting the score of reduncancy in several questions on the test set.

![ScreenShot](https://github.com/uttasarga9067/Quora-Question-Challenge/blob/main/9.PNG)



