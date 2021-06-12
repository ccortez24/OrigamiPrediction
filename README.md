# Origami Prediction Analysis Description

The purpose of this project is to predict both how many people will take an online origami class and how many people will complete the origami activity during class.

# Step by Step Process

Step 1: Data Cleaning

First we clean the data and modify data fields to ensure we have meaningful data. The data used includes the following fields:

* TC ID
* Gender
* Country
* Average time spent on academics
* Average time spent on extra curriculars
* Technology used for class
* Internet speed
* Whether students enjoy arts and crafts
* Whether students find origami to be a relaxing activity
* Student assessment of the quality of instruction
* Preferred instruction format for origami
* Completion of activitites 

Next, each of the categorical values were converted from character type data into factor type data. 

Step 2: Data Analysis 

Training and testing set were split at 75% and 25% respectively. Once the sets were split, two models were chosen to train the sets on:

* Cart Tree Model
* Conditional Inference Model (Refer the RMD file)

For the cart tree model, a basic and fitted model were created for both prediction questions to understand if a fitted model gave better results than the basic model. Both models gave an accuracy of 60% and 80% respectively. The branches from the classification trees for predicting the completion of the online origami activity are technology used, internet speed, and time spent on weekly academics and extracurriculars. For predicting if an online origami class would be chosen in the future by students, the branch was course format. From the models we have an accuracy of 60% for the prediction of completion of the online origami activity and an accuracy of 80% for the prediction of choosing an online format for origami class. 

The results for each of the prediction questions were the same from the conditional inference models as well. The reason for similar results could be the small size of data and lack of continuous (non-categorical) data, which could have caused slight differences within the two models.

Please note that we are not doing the C50 because there is no continuous data.

# Reference

Statistical Machine Learning Essentials (http://www.sthda.com/english/articles/35-statistical-machine-learning-essentials/141-cart-model-decision-tree-essentials/#example-of-data-set)
